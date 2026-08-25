# Tutorial: Convertir Markdown Científico a PDF Profesional con LaTeX

> **Para qué sirve:** Este tutorial te enseña a convertir documentos científicos en formato Markdown a PDFs profesionales en dos columnas, listos para imprimir y entregar en instituciones académicas.

---

## 📋 Índice

1. [Instalación de herramientas](#1-instalación-de-herramientas)
2. [Extraer imágenes de un PDF](#2-extraer-imágenes-de-un-pdf)
3. [Estructura de archivos](#3-estructura-de-archivos-después-de-extraer-imágenes)
4. [Generar el archivo LaTeX](#4-generar-el-archivo-latex)
5. [Compilar a PDF](#5-compilar-a-pdf)
6. [Abrir y compilar con TeXstudio](#6-abrir-y-compilar-con-texstudio)
7. [Usar el agente de IA](#7-usar-el-agente-de-ia)
8. [Solución de problemas](#8-solución-de-problemas)

---

## 1. Instalación de herramientas

### Requisitos previos

Necesitas un sistema **Linux** (Ubuntu/Debian) con conexión a internet.

### Paso 1: Instalar LaTeX y paquetes necesarios

Abre la **terminal** y ejecuta estos comandos uno por uno:

```bash
# 1. Actualizar lista de paquetes
sudo apt update

# 2. Instalar LaTeX base con soporte para español
sudo apt install -y texlive-latex-base texlive-latex-extra texlive-fonts-recommended texlive-fonts-extra texlive-lang-spanish

# 3. Instalar fuentes modernas
sudo apt install -y lmodern

# 4. Instalar fuentes adicionales para mejor calidad
sudo apt install -y texlive-fonts-extra cm-super

# 5. Instalar TeXstudio (editor visual para LaTeX)
sudo apt install -y texstudio
```

**Tiempo de instalación:** ~10-15 minutos (depende de tu conexión).

**Espacio en disco:** ~500 MB aproximadamente.

### Paso 2: Verificar la instalación

```bash
# Verificar que pdflatex está instalado
pdflatex --version | head -1

# Deberías ver algo como:
# pdfTeX 3.141592653-2.6-1.40.26 (TeX Live 2025/dev/Debian)
```

---

## 2. Extraer imágenes de un PDF

Antes de trabajar con el Markdown, necesitas extraer las imágenes del PDF original. Sigue estos pasos:

### Paso 1: Convertir PDF a DOCX

1. Ve a **[https://www.ilovepdf.com/es/pdf_a_word](https://www.ilovepdf.com/es/pdf_a_word)**
2. Haz clic en **"Seleccionar archivo PDF"** y sube tu PDF
3. Espera a que se complete la conversión
4. Haz clic en **"Descargar DOCX"**

### Paso 2: Extraer las imágenes del DOCX

1. **Busca el archivo `.docx`** que descargaste
2. **Crea una copia** del archivo (clic derecho → "Copiar", luego "Pegar")
3. **Renombra la copia** cambiando la extensión de `.docx` a `.zip`
   - Ejemplo: `paper.docx` → `paper.zip`
4. **Extrae el ZIP:**
   - **Windows:** Clic derecho → "Extraer todo" → "Extraer aquí"
   - **Linux:** Clic derecho → "Extraer aquí" o usar `unzip paper.zip`
5. **Busca las imágenes** en la carpeta extraída:
   ```
   word/
   └── media/
       ├── image1.jpeg
       ├── image2.png
       └── ...
   ```
6. **Copia las imágenes** a tu carpeta `images/`

### Paso 3: Renombrar las imágenes (opcional)

Para mejor organización, puedes renombrar las imágenes:

```bash
# Ejemplo: renombrar image1.jpeg a figure1-laser-rig.jpg
cd images/
mv image1.jpeg figure1-laser-rig.jpg
```

### Estructura resultante:

```
tu-carpeta/
├── paper.pdf                    ← PDF original
├── paper.docx                   ← DOCX descargado de ilovepdf
├── paper.zip                    ← Copia del DOCX renombrada
├── word/                        ← Carpeta extraída del ZIP
│   └── media/
│       ├── image1.jpeg          ← Imágenes originales
│       └── ...
├── images/                      ← Imágenes para el Markdown
│   ├── image1.jpeg
│   └── ...
├── mi-paper-ES.md              ← Tu documento en Markdown
└── ...
```

---

## 3. Estructura de archivos (después de extraer imágenes)

Tu carpeta debe tener esta estructura:

```
tu-carpeta/
├── MANUAL.md                    ← Este archivo (guía)
├── mi-paper-ES.md              ← Tu documento en Markdown
├── mi-paper-ES.tex             ← LaTeX generado (se crea en el paso 3)
├── header-unicode.tex          ← Soporte para caracteres especiales
└── images/                     ← Carpeta con las imágenes
    ├── image1.png
    ├── image2.jpeg
    └── ...
```

### Archivos explicados:

| Archivo | Descripción |
|---------|-------------|
| `mi-paper-ES.md` | Tu documento en formato Markdown (el original) |
| `mi-paper-ES.tex` | Archivo LaTeX generado (para compilar) |
| `header-unicode.tex` | Soporte para caracteres Unicode (subíndices, símbolos, etc.) |
| `images/` | Carpeta con todas las imágenes del documento |

### Archivos en esta carpeta del tutorial:

| Archivo | Descripción |
|---------|-------------|
| `arXiv-From-Electroculture-to-Plasma-Agriculture.pdf` | Paper original en inglés |
| `arXiv-From-Electroculture-to-Plasma-Agriculture.docx` | DOCX descargado de ilovepdf |
| `arXiv-From-Electroculture-to-Plasma-Agriculture-ES.md` | Paper traducido al español |
| `arXiv-From-Electroculture-to-Plasma-Agriculture-ES.tex` | LaTeX generado (ya compilado) |
| `header-unicode.tex` | Soporte Unicode para este paper |
| `images/` | 13 imágenes del paper |

---

## 4. Generar el archivo LaTeX

### Opción A: Una sola columna (recomendado para lectura)

Este es el método más sencillo. Ejecuta en la terminal:

```bash
pandoc tu-paper-ES.md -o tu-paper-ES.tex \
  --from markdown \
  --to latex \
  --include-in-header=header-unicode.tex
```

### Opción B: Dos columnas (estilo artículo académico)

Para el formato de revista científica en dos columnas:

```bash
pandoc tu-paper-ES.md -o tu-paper-ES.tex \
  --from markdown \
  --to latex \
  --include-in-header=header-unicode.tex \
  -V documentclass=article \
  -V classoption:twocolumn \
  -V papersize=letter \
  -V fontsize=10pt \
  -V geometry:"top=2cm,bottom=2cm,left=1.8cm,right=1.8cm,columnsep=0.6cm" \
  -V lang=es
```

### Parámetros explicados:

| Parámetro | Valor | Descripción |
|-----------|-------|-------------|
| `--from markdown` | — | Formato de entrada |
| `--to latex` | — | Formato de salida (LaTeX) |
| `--include-in-header` | `header-unicode.tex` | Archivo de soporte Unicode |
| `-V documentclass` | `article` | Tipo de documento |
| `-V classoption` | `twocolumn` | Dos columnas (solo Opción B) |
| `-V papersize` | `letter` | Tamaño de papel (carta) |
| `-V fontsize` | `10pt` | Tamaño de fuente |
| `-V geometry` | `top=2cm,...` | Márgenes y separación de columnas |
| `-V lang` | `es` | Idioma (español) |

---

## 5. Compilar a PDF

### Método 1: Desde la terminal

```bash
# Primera pasada (genera el PDF)
pdflatex tu-paper-ES.tex

# Segunda pasada (resuelve referencias cruzadas)
pdflatex tu-paper-ES.tex
```

### Método 2: Desde TeXstudio (recomendado)

1. **Abrir TeXstudio:**
   ```bash
   texstudio tu-paper-ES.tex
   ```

2. **Compilar:** Presiona **F1** o haz clic en el botón verde ▶

3. **Ver PDF:** Presiona **F7** o haz clic en "Ver PDF"

4. **Atajos útiles:**
   | Tecla | Acción |
   |-------|--------|
   | **F1** | Compilar |
   | **F7** | Ver PDF |
   | **F8** | Compilar + Ver PDF |

### Si sale error de Unicode

Ve a: **Opciones → Configurar TeXstudio → Compilador**

Cambia `pdflatex` por `xelatex` en el campo "PdfLaTeX".

---

## 6. Abrir y compilar con TeXstudio

### Paso 1: Abrir el archivo .tex

```bash
texstudio arXiv-From-Electroculture-to-Plasma-Agriculture-ES.tex
```

O simplemente haz **doble clic** en el archivo `.tex` desde el administrador de archivos.

### Paso 2: Compilar

- Presiona **F1** o haz clic en el botón verde ▶ de "Compilar"

### Paso 3: Ver el PDF

- Presiona **F7** o haz clic en "Ver PDF"

### Atajos útiles en TeXstudio

| Tecla | Acción |
|-------|--------|
| **F1** | Compilar |
| **F7** | Ver PDF |
| **F8** | Compilar + Ver PDF |
| **F9** | Compilar todo |

### Si sale error de Unicode

Ve a: **Opciones → Configurar TeXstudio → Compilador**

Cambia `pdflatex` por `xelatex` en el campo "Motor predeterminado".

---

## 7. Usar el agente de IA

### Prompt 1: Generar el archivo LaTeX

Copia y pega este prompt en tu agente de IA (FreeBuff, ChatGPT, Claude, etc.):

```
Genera un archivo LaTeX para este documento Markdown. 
Requisitos:
- Formato de dos columnas (estilo artículo académico)
- Papel carta
- Fuente 10pt
- Márgenes de 2cm
- Soporte para caracteres Unicode (subíndices, símbolos griegos, etc.)
- Incluir soporte para español (babel)
- Las imágenes deben mantenerse en sus posiciones originales
- Las tablas deben ser legibles en dos columnas

Archivo Markdown: [pegar aquí el contenido o la ruta del archivo]
```

### Prompt 2: Corregir errores de compilación

Si el LaTeX tiene errores, usa este prompt:

```
Este archivo LaTeX tiene errores de compilación. 
Analiza el log de errores y corrige el archivo:

[pегar aquí los errores del log]

Errores específicos que suelen aparecer:
- Unicode characters not set up → Agregar \newunicodechar
- longtable not in 1-column mode → Usar tabular en su lugar
- Missing package → Agregar \usepackage correspondiente
```

### Prompt 3: Verificar paridad Markdown vs LaTeX

```
Verifica que este archivo LaTeX tenga todo el contenido 
del Markdown original. Compara:
- Todas las secciones
- Todas las imágenes
- Todas las tablas
- Todas las referencias
- Los caracteres especiales

Markdown original: [ruta del .md]
LaTeX generado: [ruta del .tex]

Reporta si falta algo.
```

### Prompt 4: Agregar información al final del PDF

```
Agrega al final de este archivo LaTeX una página separada 
con la siguiente información:

- Crédito a la herramienta utilizada
- URL del repositorio
- URL del paper original
- DOI del paper

Usa \clearpage y \onecolumn para que sea una página separada.
```

---

## 8. Solución de problemas

### Problema: "Unicode character not set up"

**Solución:** Agregar al `header-unicode.tex`:

```latex
\newunicodechar{₂}{\ensuremath{_2}}
\newunicodechar{₃}{\ensuremath{_3}}
\newunicodechar{°}{\textdegree}
```

### Problema: "longtable not in 1-column mode"

**Solución:** Las tablas largas no funcionan en dos columnas. Opciones:

1. Usar `tabular` en lugar de `longtable`
2. Dividir la tabla en partes más pequeñas
3. Usar `\onecolumn` temporalmente para la tabla

### Problema: Imágenes no aparecen

**Verificar:**
1. Que la ruta en el `.tex` sea correcta: `\graphicspath{{images/}}`
2. Que las imágenes existan en la carpeta `images/`
3. Que los nombres de archivo coincidan exactamente (sensible a mayúsculas)

### Problema: Compilación lenta

**Solución:** En TeXstudio, ve a **Opciones → Configurar TeXstudio → Compilador** y marca "Modo rápido" (solo una pasada).

---

## 📚 Recursos adicionales

- **Pandoc:** [pandoc.org](https://pandoc.org/)
- **LaTeX Wikibook:** [es.wikibooks.org/wiki/LaTeX](https://es.wikibooks.org/wiki/LaTeX)
- **TeXstudio Manual:** [texstudio.org](https://texstudio.org/)
- **FreeBuff:** [freebuff.com](https://freebuff.com) — Asistente de IA para conversiones

---

## ✅ Checklist antes de imprimir

- [ ] El PDF se ve correctamente en dos columnas
- [ ] Todas las imágenes aparecen y son legibles
- [ ] Las tablas son legibles y no se cortan
- [ ] Los caracteres especiales (subíndices, símbolos) se ven bien
- [ ] Las referencias están numeradas correctamente
- [ ] El DOI es correcto
- [ ] La página final con URLs está separada del contenido

---

*Manual creado con la asistencia de FreeBuff (freebuff.com)*
*Para el repositorio: https://github.com/wachin/electrocultura-christofleau*
