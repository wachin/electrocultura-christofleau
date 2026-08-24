# Tarea pendiente: Integrar imágenes al README.md

## Resumen del trabajo realizado

1. **Carpeta `images/` creada** con las 62 imágenes extraídas del DOCX:
   `/home/wachin/Dev3/electrocultura-christofleau/images/`

2. **PDF analizado completamente** (64 páginas). El PDF original está en:
   `/home/wachin/Dev3/electrocultura-christofleau/Christofleau-Electroculture_text.pdf`

3. **Mapeo imagen→contenido completado** (ver tabla abajo).

## Tareas pendientes

### 1. Añadir números de página [p. X] en README.md

El README.md actualmente no tiene números de página. Deben insertarse `[p. X]` al inicio de cada sección, según el PDF original. Mapeo de páginas:

| Sección en README.md | Página PDF |
|---|---|
| Portada "ELECTROCULTURA por Mons. Justin Christofleau" | p. 1 |
| "ELECTROCULTURA por MONS. JUSTIN CHRISTOFLEAU" | p. 3 |
| Retrato de Justin Christofleau con credenciales | p. 4 |
| "EL LLAMAMIENTO DEL SR. J. CHRISTOFLEAU..." | p. 5 |
| Diagrama del aparato con cables vibratorios | p. 7 |
| Sección "DESCRIPCIÓN" (Magnetismo, corrientes, etc.) | p. 8 |
| "NOTAS DE M. JUSTIN CHRISTOFLEAU" | p. 9 |
| "INSTRUCCIONES DE INSTALACIÓN" (inicio) | p. 10 |
| Diagrama de instalación (Figs A, B, C, D) | p. 11 |
| "APLICACIÓN A VIDES CON ALAMBRES" | p. 12 |
| Diagrama de vides con alambres | p. 13 |
| "NOTA" sobre barrera eléctrica + diagrama | p. 14 |
| "PARA VIDES QUE CORREN DE ESTE A OESTE" | p. 15 |
| "APLICACIÓN A UNA HILERA DE ÁRBOLES" | p. 15 |
| "APLICACIÓN A ÁRBOLES AISLADOS" + diagrama | p. 16 |
| "ELECTROCULTURA por GEORGE BLANCHARD — CHARLA CIENTÍFICA" | p. 17 |
| Continuación Charla Científica | p. 19 |
| Continuación (electrólisis, resultados) | p. 20 |
| "Un borde de perejil" foto | p. 21 |
| "APLICACIÓN DE LA ELECTRICIDAD A LA VIDA VEGETAL por Mons. G. Blanchard" | p. 22 |
| Continuación (resultados: zanahorias, remolachas, peral) | p. 23 |
| Continuación (acumulación de electricidad, sequía) | p. 24 |
| "Conjunto de nueve postes" + "Vista del aparato" fotos | p. 25 |
| Continuación (corrientes industriales vs atmosféricas) | p. 26 |
| "Campo de Patatas" foto | p. 27 |
| Continuación (tres factores esenciales) | p. 28 |
| "OPINIÓN DE LOS CIENTÍFICOS" (Dr. Foreau De Courmelles) | p. 29 |
| "Algunas fresas" foto | p. 30 |
| "INFORMES OFICIALES" (Metz) | p. 31 |
| "OPINIÓN DE LA PRENSA" (Agriculture de Touraine) | p. 32 |
| "White Haricots from Spain" foto | p. 33 |
| "PEAS 7½ to 9ft High" foto | p. 34 |
| Brisbane Daily Mail + L'Homme Libre | p. 35 |
| L'Homme Libre + La Revue du Ciel | p. 36 |
| "LISTA DE PERIÓDICOS" | p. 37 |
| "NOTAS VARIAS" | p. 38 |
| "Repollo de 11 pies" foto | p. 40 |
| Continuación Notas Varias | p. 41-42 |
| Diagrama de fijación de cable gotero | p. 43 |
| "PUNTOS A RECORDAR" | p. 44 |
| "TESTIMONIOS" (Roger Claret) | p. 45 |
| "Trébol electrificado" foto | p. 46 |
| "Viejo peral cargado de fruta" foto | p. 47 |
| Testimonios (Lovell, McCaughan) | p. 48 |
| Testimonios (Etoc, Groussin) | p. 49 |
| Diagrama "Application to Culture" | p. 50 |
| Testimonios (Fairweather, McHugh) | p. 51 |
| "Avena cosechada en 1922" foto | p. 52 |
| Testimonios (Lovell, Illingsworth) | p. 53 |
| Diagrama "Method of fixing Vines running East and West" | p. 54 |
| Testimonios (Van Zuilecom, Gordon) | p. 55 |
| Testimonios (Stagg) | p. 56 |
| Testimonios (McCaughan, Halligan) | p. 57 |
| Testimonios (Wood, Culahan, Titley) | p. 58 |
| Informes Burgess (bananas, Queensland) | p. 59 |
| "PRECIO DEL APARATO" | p. 60 |
| "¡LA MÁQUINA DE HACER DINERO!" anuncio | p. 62 |
| "ELECTRIFIQUE SUS SEMILLAS" | p. 64 |

### 2. Reemplazar placeholders de imágenes

El README.md tiene placeholders como `[Imagen: ...]`. Deben reemplazarse con:

```markdown
![Texto alternativo](images/imageXX.png "Título descriptivo")
```

**Mapeo de placeholders a imágenes:**

| Placeholder en README.md | Imagen |
|---|---|
| `[Imagen: Diagrama del aparato de electrocultura mostrando los cables vibratorios bajo la acción del viento]` | `images/image6.png` |
| `[Imagen: Diagrama que muestra la aplicación del aparato a vides con alambres]` | `images/image12.png` |
| `[Imagen: Diagrama de barrera para evitar la fuga de electricidad]` | `images/image13.png` |
| `[Imagen: Diagrama de la aplicación del aparato a una hilera de árboles]` | `images/image49.png` |
| `[Imagen: Diagrama de la electrificación de un solo árbol]` | `images/image15.png` |
| `[Imagen: Un borde de perejil cultivado con electrocultura]` | `images/image20.png` |
| `[Imagen: Cultivo de perejil con electrocultura]` | `images/image38.png` (o `image20.png` si es la misma) |
| `[Imagen: Conjunto de nueve postes erigidos en el vivero del Sr. C. E. Pope...]` | `images/image24.png` |
| `[Imagen: Vista en primer plano del aparato]` | `images/image24.png` (misma imagen, contiene ambas fotos) |
| `[Imagen: Algunas fresas cultivadas con electrocultura]` | `images/image29.png` |
| `[Imagen: Repollo de 11 pies (3,35 m) de circunferencia]` | `images/image39.png` |
| `[Imagen: Diagrama que muestra el método de fijación del cable gotero...]` | `images/image42.png` |
| `[Imagen: Trébol electrificado por el proceso de electrocultura...]` | `images/image45.png` |
| `[Imagen: Un viejo peral cargado de fruta...]` | `images/image46.png` |
| `[Imagen: Avena cosechada en 1922 en un campo sin fertilizantes...]` | `images/image51.png` |
| `[Imagen: Diagrama de aplicación del aparato a vides]` | `images/image53.png` |

### 3. Notas importantes

- **image3.png** es una imagen en blanco (puede ignorarse).
- **image1.png** y **image2.png** son páginas de título decorativas del PDF (pueden omitirse o usarse como portada adicional).
- **image4.png** es el retrato de Justin Christofleau (ideal para la sección de portada).
- **image17.png** (>10MB) e **image38.png** (>10MB) no pudieron transcribirse, probablemente son fotografías grandes.
- El script Python que intenté ejecutar fue cancelado, pero usaba `edit` para hacer cada reemplazo individualmente.
- Después de modificar README.md, se recomienda ejecutar: `git diff` para verificar cambios.

### 4. Comando útil para contar placeholders restantes

```bash
grep -c '\[Imagen:' README.md
```

Eso mostrará cuántos placeholders quedan por reemplazar (debería ser 0 al finalizar).