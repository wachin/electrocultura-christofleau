# Tutorial: Convertir Markdown Científico a PDF Profesional con LaTeX

> **Para qué sirve:** Este tutorial te enseña a convertir documentos científicos en formato Markdown a PDFs profesionales en dos columnas, listos para imprimir y entregar en instituciones académicas.

---

## 📋 Índice

1. [Instalación de herramientas](#1-instalación-de-herramientas)
2. [Estructura de archivos](#2-estructura-de-archivos)
3. [Generar el archivo LaTeX](#3-generar-el-archivo-latex)
4. [Compilar a PDF](#4-compilar-a-pdf)
5. [Usar el agente de IA](#5-usar-el-agente-de-ia)
6. [Solución de problemas](#6-solución-de-problemas)

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

## 2. Estructura de archivos

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

---

## 3. Generar el archivo LaTeX

### Método manual (recomendado para aprendizaje)

Ejecuta este comando en la terminal, reemplazando los valores:

```bash
pandoc tu-paper-ES.md -o tu-paper-ES.tex \
  --pdf-engine=pdflatex \
  -V documentclass=article \
  -V classoption:twocolumn \
  -V papersize=letter \
  -V fontsize=10pt \
  -V geometry:"top=2cm,bottom=2cm,left=1.8cm,right=1.8cm,columnsep=0.6cm" \
  -V lang=es \
  -H header-unicode.tex \
  --standalone
```

### Parámetros explicados:

| Parámetro | Valor | Descripción |
|-----------|-------|-------------|
| `--pdf-engine` | `pdflatex` | Motor de compilación |
| `-V documentclass` | `article` | Tipo de documento |
| `-V classoption` | `twocolumn` | Dos columnas (estilo académico) |
| `-V papersize` | `letter` | Tamaño de papel (carta) |
| `-V fontsize` | `10pt` | Tamaño de fuente |
| `-V geometry` | `top=2cm,...` | Márgenes y separación de columnas |
| `-V lang` | `es` | Idioma (español) |
| `-H header-unicode.tex` | — | Archivo de soporte Unicode |
| `--standalone` | — | Genera archivo completo con preámbulo |

---

## 4. Compilar a PDF

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

## 5. Usar el agente de IA

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

## 6. Solución de problemas

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
