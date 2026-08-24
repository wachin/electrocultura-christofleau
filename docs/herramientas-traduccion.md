# Herramientas utilizadas para la traducción

## Extracción de texto del PDF

- **pdftotext** (poppler-utils) — para extraer el texto plano del archivo `Christofleau-Electroculture_text.pdf`.
  - Instalado en Termux mediante: `pkg install poppler`

## Traducción y formateo

- **Qwen Code** (CLI) — agente que realizó la traducción automática del inglés al español y el formateo del documento Markdown.
- El texto fuente extraído tenía **2911 líneas** de texto plano.
- El documento resultante tiene **1038 líneas** (~100 KB) en formato Markdown.

## Archivos

| Archivo | Descripción |
|---------|-------------|
| `Christofleau-Electroculture_text.pdf` | PDF original del libro |
| `README.md` | Traducción completa al español en formato Markdown |
| `docs/herramientas-traduccion.md` | Este archivo |