# Guía: extraer fórmulas de un PDF y convertirlas a LaTeX para Markdown

Esta guía documenta el procedimiento utilizado para recuperar las fórmulas matemáticas del artículo **At the Origins of Electroculture: A Retrodictive Modelling of Bertholon's 18th-Century Electrovegetometer in the Pre-Corona Regime** y conservarlas correctamente al convertir el documento a Markdown y, posteriormente, a LaTeX.

Los archivos relacionados se encuentran en esta misma carpeta:

- `arXiv-Origins-Electroculture-Bertholon-Electrovegetometer.pdf`: documento original.
- `arXiv-Origins-Electroculture-Bertholon-Electrovegetometer.docx`: conversión de PDF a Word realizada con iLovePDF.
- `arXiv-Origins-Electroculture-Bertholon-Electrovegetometer-EN.md`: conversión inglesa a Markdown.
- `arXiv-Origins-Electroculture-Bertholon-Electrovegetometer-ES.md`: traducción española en Markdown.

## 1. El problema

Las herramientas convencionales como `pdftotext` pueden extraer letras y símbolos de un PDF, pero no necesariamente recuperan la estructura matemática. Una fracción, por ejemplo, está compuesta visualmente por un numerador, una línea horizontal y un denominador. El PDF puede almacenar esos elementos como glifos colocados en coordenadas independientes, sin conservar la información de que forman un `\frac{}{}`.

En este artículo aparecen además dos dificultades:

- El documento original usa un diseño de dos columnas, que puede alterar el orden de lectura durante la extracción.
- Las ecuaciones usan la fuente `CambriaMath` y contienen fracciones, vectores, subíndices, exponentes y evaluaciones en los límites.

Una conversión convencional puede producir fragmentos como estos:

```text
𝜎air
(𝑧) = 𝜎~0~
exp ( ) {5}
```

Ese texto no es una ecuación LaTeX y se descompone todavía más al convertir el Markdown a `.tex`.

Instalar TeX Live, XeLaTeX o LuaLaTeX resuelve la etapa de **compilación**, pero no reconstruye la semántica matemática perdida durante la extracción del PDF. Para ello es necesario utilizar reconocimiento matemático de imágenes o reconstruir manualmente las fórmulas.

## 2. Por qué el DOCX convertido no resuelve las fórmulas

El archivo DOCX de esta carpeta fue obtenido mediante:

<https://www.ilovepdf.com/es/pdf_a_word>

Puede ser útil para recuperar texto ordinario, imágenes y parte de la distribución visual. Sin embargo, una inspección interna del archivo mostró que contiene:

- 0 objetos matemáticos de Word en formato OMML (`m:oMath` o `m:oMathPara`).
- 8 archivos de imagen.
- Numerosas formas y cuadros de texto usados para reproducir la disposición de las páginas.

Por tanto, este flujo:

```text
PDF → iLovePDF → DOCX → Pandoc → Markdown
```

no recupera las ecuaciones como objetos matemáticos editables. Pandoc recibe caracteres y elementos visuales fragmentados y no puede deducir de manera fiable su estructura original.

Esto sería diferente si se dispusiera del DOCX original del autor y sus ecuaciones estuvieran almacenadas como objetos matemáticos OMML. En ese caso, Pandoc podría convertirlas directamente a LaTeX.

## 3. Estrategia recomendada para este artículo

Debido a que el documento contiene solamente 21 ecuaciones principales, el procedimiento más controlable es:

1. Conservar el texto y las figuras del Markdown existente.
2. Renderizar a alta resolución las páginas que contienen ecuaciones.
3. Recortar cada ecuación como una imagen PNG independiente.
4. Procesar cada recorte con una herramienta de reconocimiento matemático.
5. Revisar el LaTeX comparándolo visualmente con el PDF.
6. Insertar las ecuaciones corregidas en el Markdown.
7. Normalizar también las expresiones matemáticas incluidas dentro de los párrafos.
8. Validar el Markdown con Pandoc y compilarlo con XeLaTeX.

No existe una conversión PDF → Markdown que garantice una exactitud matemática del 100 %. La revisión visual sigue siendo necesaria, especialmente en un documento científico.

## 4. Localización de las ecuaciones

Las ecuaciones numeradas están distribuidas en las siguientes páginas reales del archivo PDF:

| Página del PDF | Ecuaciones |
|---:|:---|
| 3 | (1) |
| 5 | (2)–(8) |
| 6 | (9)–(13) |
| 7 | (14)–(21) |

La página 4 queda entre las páginas necesarias, pero no contiene ecuaciones numeradas.

## 5. Renderizar las páginas como imágenes

### 5.1. Instalar la herramienta

`pdftoppm` forma parte del paquete `poppler-utils`:

```bash
sudo apt update
sudo apt install poppler-utils
```

### 5.2. Crear imágenes PNG a 400 dpi

Desde la raíz del repositorio:

```bash
cd /home/wachin/Dev3/electrocultura-christofleau

mkdir -p formulas/pages

pdftoppm \
  -png \
  -r 400 \
  -f 3 \
  -l 7 \
  docs/studies/arXiv-Origins-Electroculture-Bertholon-Electrovegetometer/arXiv-Origins-Electroculture-Bertholon-Electrovegetometer.pdf \
  formulas/pages/page
```

El parámetro `-r 400` produce imágenes a 400 dpi. Esta resolución ayuda a distinguir subíndices, exponentes, letras griegas y líneas finas de fracción.

Se recomienda PNG en lugar de JPEG, porque PNG no introduce artefactos de compresión alrededor de los símbolos.

Si se desea renderizar únicamente una página, por ejemplo la página 6:

```bash
pdftoppm \
  -png \
  -r 400 \
  -f 6 \
  -l 6 \
  docs/studies/arXiv-Origins-Electroculture-Bertholon-Electrovegetometer/arXiv-Origins-Electroculture-Bertholon-Electrovegetometer.pdf \
  formulas/pages/page-6
```

`pdfimages` no es adecuado para esta tarea. Las fórmulas no están almacenadas como imágenes independientes dentro del PDF; son texto y glifos posicionados. Por eso primero debe renderizarse la página completa.

## 6. Recortar una ecuación por imagen

Cada recorte debe contener:

- Una sola ecuación.
- Todos sus subíndices, exponentes y símbolos.
- Su número, si se desea usarlo como referencia durante la revisión.
- Un pequeño margen blanco alrededor.
- Ninguna línea de texto o ecuación vecina.

### Opción A: GNOME Screenshot

```bash
gnome-screenshot -a
```

La opción `-a` permite seleccionar un área de la pantalla.

### Opción B: Flameshot

```bash
sudo apt install flameshot
flameshot gui
```

### Nombres sugeridos

```text
formulas/
├── equation-01.png
├── equation-02.png
├── equation-03.png
├── ...
└── equation-21.png
```

No se deben reducir las imágenes después de recortarlas. Una imagen demasiado pequeña puede hacer que el reconocedor confunda caracteres como `1`, `l`, `I`, `z` y `2`.

## 7. Convertir las imágenes a LaTeX

### 7.1. Mathpix Snip

[Mathpix Snip](https://website.mathpix.com/docs/snip/create-snips) permite seleccionar una ecuación directamente desde la pantalla o subir una imagen y copiar el resultado en LaTeX. Dispone de aplicación para Linux.

Con Mathpix puede evitarse incluso la etapa de guardar los recortes: se abre el PDF con suficiente ampliación, se activa la captura de Mathpix y se selecciona una ecuación.

Procedimiento:

1. Abrir el PDF y ampliar la página entre 200 % y 400 %.
2. Activar la captura de Mathpix Snip.
3. Seleccionar exclusivamente la ecuación.
4. Copiar el resultado LaTeX.
5. Pegarlo en un archivo temporal.
6. Comparar la previsualización de Mathpix con la ecuación original.

Mathpix es un servicio externo. Las capturas pueden enviarse a sus servidores y algunas funciones pueden requerir una cuenta o un plan de pago.

### 7.2. SimpleTex

[SimpleTex](https://doc.simpletex.cn/en/) permite subir una imagen de una fórmula impresa y obtener LaTeX, MathML o una ecuación de Word.

Se puede utilizar como segunda opinión cuando Mathpix produzca un resultado dudoso. También es un servicio externo, por lo que se deben considerar la privacidad del documento y sus condiciones de uso.

### 7.3. pix2tex/LaTeX-OCR local

[pix2tex](https://github.com/lukas-blecher/LaTeX-OCR) es una alternativa de código abierto que puede ejecutarse localmente. Para evitar incompatibilidades con Python 3.13 se recomienda crear un entorno con Python 3.11:

```bash
cd /home/wachin/Dev3/electrocultura-christofleau

uv python install 3.11
uv venv --python 3.11 .venv-pix2tex
source .venv-pix2tex/bin/activate

uv pip install "pix2tex[gui]"
latexocr
```

Los modelos se descargan durante el primer uso. La ejecución en CPU es más lenta que con GPU, pero procesar una ecuación individual requiere muchos menos recursos que convertir el PDF científico completo.

Para salir del entorno virtual:

```bash
deactivate
```

## 8. Formato correcto de las ecuaciones en Markdown

### 8.1. Ecuaciones independientes

Las ecuaciones que ocupan una línea propia deben delimitarse con `$$`:

```markdown
$$
\left.\frac{\partial V}{\partial z}\right|_{z=0}
=
-\frac{J_{0,\mathrm{atm}}}{\sigma(0)}
\tag{9}
$$
```

La ecuación se mostrará así:

$$
\left.\frac{\partial V}{\partial z}\right|_{z=0}
=
-\frac{J_{0,\mathrm{atm}}}{\sigma(0)}
\tag{9}
$$

Se recomienda colocar los delimitadores en líneas independientes. No debe existir una línea en blanco entre el `$$` inicial, la fórmula y el `$$` final.

Para la numeración se debe usar:

```latex
\tag{9}
```

No se recomienda escribir:

```latex
\quad \{9\}
```

La segunda forma solamente dibuja el número entre llaves y no representa una etiqueta matemática real.

### 8.2. Matemática dentro de un párrafo

Las expresiones incluidas dentro de una oración deben usar un solo dólar:

```markdown
La conductividad $\sigma(z)$ aumenta con la altitud y la densidad de corriente satisface $\vec{J}=\sigma\vec{E}$.
```

No se debe encerrar cada símbolo matemático entre `$$`, porque eso crea ecuaciones independientes y rompe los párrafos.

### 8.3. Evitar símbolos matemáticos Unicode estilizados

Se debe reemplazar texto como:

```text
𝐸~0,𝑎𝑡𝑚~ ≈ −120𝑉. 𝑚^−1^
```

por LaTeX semántico:

```markdown
$E_{0,\mathrm{atm}} \approx -120\,\mathrm{V\,m^{-1}}$
```

Esto evita advertencias de fuentes ausentes y permite que Pandoc, MathJax, XeLaTeX y LuaLaTeX interpreten la expresión correctamente.

## 9. Limpiar la salida del reconocedor

Los servicios pueden devolver la fórmula con alguno de estos delimitadores:

```latex
\[ ... \]
```

```latex
\( ... \)
```

```latex
$$ ... $$
```

No deben anidarse delimitadores. Se conserva solamente el contenido de la fórmula y se añaden los delimitadores adoptados por el documento:

```markdown
$$
...contenido LaTeX...
\tag{n}
$$
```

También conviene eliminar comandos puramente visuales o incompatibles que el reconocedor pueda inventar, siempre que no formen parte de la ecuación original.

## 10. Revisión obligatoria de cada fórmula

El reconocimiento matemático puede producir LaTeX válido pero matemáticamente incorrecto. Deben comprobarse especialmente:

- Signos positivos y negativos.
- Paréntesis, corchetes y llaves.
- Numeradores y denominadores.
- Exponentes y subíndices.
- Índices compuestos como `0,\mathrm{atm}`.
- Límites de evaluación, por ejemplo `z=0` y `z=H`.
- Derivadas parciales y ordinarias.
- Flechas de vectores.
- Letras griegas como `\sigma`, `\varepsilon` y `\rho`.
- Letras o números parecidos: `l`, `1`, `I`, `z`, `2`, `O` y `0`.
- Puntos de multiplicación.
- Unidades y sus exponentes.
- El número de ecuación asignado mediante `\tag{n}`.

Una forma práctica de revisión es comparar tres elementos simultáneamente:

1. El recorte de la fórmula original.
2. El código LaTeX reconocido.
3. La fórmula renderizada a partir de ese código.

## 11. Convertir el Markdown corregido a LaTeX

Pandoc reconoce `$...$` como matemática en línea y `$$...$$` como matemática independiente mediante la extensión `tex_math_dollars`.

Desde la carpeta del artículo:

```bash
cd /home/wachin/Dev3/electrocultura-christofleau/docs/studies/arXiv-Origins-Electroculture-Bertholon-Electrovegetometer

pandoc \
  arXiv-Origins-Electroculture-Bertholon-Electrovegetometer-EN.md \
  --from=markdown+tex_math_dollars \
  --to=latex \
  --standalone \
  --resource-path=. \
  --output=arXiv-Origins-Electroculture-Bertholon-Electrovegetometer-EN.tex
```

Para la traducción española se cambia `-EN.md` por `-ES.md`.

## 12. Generar directamente un PDF con XeLaTeX

### 12.1. Instalar los compiladores y fuentes

En Debian o Ubuntu:

```bash
sudo apt install -y \
  texlive-latex-base \
  texlive-latex-extra \
  texlive-fonts-recommended \
  texlive-fonts-extra \
  texlive-lang-spanish \
  texlive-xetex \
  texlive-luatex \
  lmodern \
  cm-super
```

### 12.2. Compilar desde Markdown

```bash
pandoc \
  arXiv-Origins-Electroculture-Bertholon-Electrovegetometer-EN.md \
  --from=markdown+tex_math_dollars \
  --standalone \
  --resource-path=. \
  --pdf-engine=xelatex \
  --output=arXiv-Origins-Electroculture-Bertholon-Electrovegetometer-EN.pdf
```

XeLaTeX es preferible a pdfLaTeX cuando el texto contiene caracteres Unicode. Sin embargo, los símbolos matemáticos deben seguir escribiéndose como LaTeX dentro de `$...$` o `$$...$$`, en lugar de depender de caracteres Unicode estilizados.

## 13. Comprobaciones rápidas

### 13.1. Buscar ecuaciones reconocidas

```bash
rg -n '^\$\$$|\\tag\{[0-9]+\}' \
  arXiv-Origins-Electroculture-Bertholon-Electrovegetometer-EN.md
```

### 13.2. Buscar caracteres matemáticos Unicode pendientes

```bash
rg -n '[𝐀-𝟿]|[⁰¹²³⁴⁵⁶⁷⁸⁹⁻]|[∂∇σρθε≈]' \
  arXiv-Origins-Electroculture-Bertholon-Electrovegetometer-EN.md
```

Este comando sirve como indicador, no como prueba definitiva: algunas letras griegas pueden aparecer legítimamente en el texto, pero es preferible que las expresiones matemáticas completas estén representadas en LaTeX.

### 13.3. Verificar que Pandoc reconoce matemática de bloque

```bash
pandoc \
  arXiv-Origins-Electroculture-Bertholon-Electrovegetometer-EN.md \
  --from=markdown+tex_math_dollars \
  --to=native \
  | rg 'DisplayMath'
```

### 13.4. Compilar antes de reemplazar el documento definitivo

Durante las pruebas se recomienda escribir la salida en `/tmp`:

```bash
pandoc \
  arXiv-Origins-Electroculture-Bertholon-Electrovegetometer-EN.md \
  --from=markdown+tex_math_dollars \
  --standalone \
  --resource-path=. \
  --pdf-engine=xelatex \
  --output=/tmp/electrovegetometer-prueba.pdf
```

## 14. Problemas frecuentes

### La ecuación aparece como texto sin formato

Comprobar que está encerrada correctamente:

```markdown
$$
E=mc^2
$$
```

Y que Pandoc se ejecuta con:

```text
--from=markdown+tex_math_dollars
```

### La fórmula aparece cortada

El recorte probablemente omitió un subíndice, exponente o límite. Repetirlo dejando un margen blanco ligeramente mayor.

### El OCR confunde símbolos

Volver a renderizar a 400 o 600 dpi y comparar el resultado de dos reconocedores diferentes. Si la fórmula es corta, suele ser más rápido corregir manualmente el LaTeX.

### XeLaTeX informa que faltan caracteres

Buscar caracteres matemáticos Unicode fuera de los delimitadores y convertirlos a LaTeX semántico. Por ejemplo:

```text
𝐽 → $J$
σ → $\sigma$
𝑚⁻² → $\mathrm{m^{-2}}$
```

### La numeración muestra llaves literales

Reemplazar:

```latex
\quad \{9\}
```

por:

```latex
\tag{9}
```

### Las imágenes del artículo no aparecen

Ejecutar Pandoc desde la carpeta que contiene el Markdown o proporcionar la ruta de recursos:

```text
--resource-path=.
```

Después, comprobar que las rutas de las imágenes son relativas al archivo Markdown.

## 15. Resumen del flujo

```text
PDF original
    ↓ renderizar páginas 3, 5, 6 y 7 a 400 dpi
Imágenes PNG
    ↓ recortar una ecuación por archivo
21 recortes
    ↓ Mathpix, SimpleTex o pix2tex
Código LaTeX
    ↓ revisión visual y corrección
Markdown con $...$ y $$...$$
    ↓ Pandoc + XeLaTeX
Archivo .tex o PDF final
```

Para este artículo, el DOCX convertido mediante iLovePDF puede mantenerse como fuente auxiliar para texto e imágenes, pero no debe considerarse una fuente matemática fiable.

## Referencias de herramientas

- [Pandoc: sintaxis matemática con delimitadores de dólar](https://pandoc.org/demo/example33/8.13-math.html)
- [Mathpix Snip: crear capturas y convertirlas](https://website.mathpix.com/docs/snip/create-snips)
- [Mathpix: procesamiento OCR de imágenes](https://docs.mathpix.com/guides/image-ocr)
- [SimpleTex: documentación oficial](https://doc.simpletex.cn/en/)
- [pix2tex/LaTeX-OCR](https://github.com/lukas-blecher/LaTeX-OCR)
