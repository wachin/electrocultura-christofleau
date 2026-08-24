# FR 804141 — Aparato de Iluminación Electromagnética

**Inventor:** Justin Christofleau  
**Fecha de concesión:** 1936  
**País:** Francia

---

## Resumen de la Invención

Un dispositivo que **trae electricidad natural al interior de las viviendas** humanas, captándola del aire ambiente y distribuyéndola a través de la luz. Un círculo metálico magnetizado atrae electricidad positiva de la atmósfera; la luz del foco cruza este campo magnético y **se carga de electricidad natural**, transfiriéndola a todo el espacio que ilumina.

---

## Diagrama Técnico

```svg
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 900 750" font-family="'Segoe UI', Arial, sans-serif">
  <defs>
    <linearGradient id="light" x1="0" y1="0" x2="0" y2="1">
      <stop offset="0%" stop-color="#FFF9C4"/>
      <stop offset="100%" stop-color="#FFECB3"/>
    </linearGradient>
    <linearGradient id="reflector" x1="0" y1="0" x2="0" y2="1">
      <stop offset="0%" stop-color="#B0BEC5"/>
      <stop offset="100%" stop-color="#ECEFF1"/>
    </linearGradient>
    <linearGradient id="ring10" x1="0" y1="0" x2="1" y2="0">
      <stop offset="0%" stop-color="#546E7A"/>
      <stop offset="50%" stop-color="#90A4AE"/>
      <stop offset="100%" stop-color="#546E7A"/>
    </linearGradient>
    <linearGradient id="bulb" x1="0" y1="0" x2="0" y2="1">
      <stop offset="0%" stop-color="#FFF59D"/>
      <stop offset="100%" stop-color="#FFEE58"/>
    </linearGradient>
    <marker id="arrowY10" markerWidth="10" markerHeight="7" refX="9" refY="3.5" orient="auto">
      <polygon points="0 0, 10 3.5, 0 7" fill="#F9A825"/>
    </marker>
    <marker id="arrowL10" markerWidth="10" markerHeight="7" refX="9" refY="3.5" orient="auto">
      <polygon points="0 0, 10 3.5, 0 7" fill="#FFC107"/>
    </marker>
  </defs>

  <!-- Background -->
  <rect width="900" height="750" fill="#FAFAF5"/>

  <!-- Title -->
  <text x="450" y="32" text-anchor="middle" font-size="18" font-weight="bold" fill="#333">FR 804141 — Aparato de Iluminación Electromagnética</text>
  <text x="450" y="50" text-anchor="middle" font-size="12" fill="#666">Vista frontal y corte — Traer electricidad natural al interior de viviendas</text>

  <!-- === VIEW 1: FRONT VIEW (Left) === -->
  <g transform="translate(50, 80)">
    <text x="180" y="15" text-anchor="middle" font-size="13" font-weight="bold" fill="#333">VISTA FRONTAL (Fig. 1)</text>
    
    <!-- Metal ring A (not closed circle) -->
    <path d="M 180 50 A 110 110 0 1 1 170 50" fill="none" stroke="url(#ring10)" stroke-width="15"/>
    
    <!-- Gap in ring -->
    <line x1="172" y1="42" x2="172" y2="58" stroke="#FF9800" stroke-width="4"/>
    <line x1="178" y1="42" x2="178" y2="58" stroke="#FF9800" stroke-width="4"/>
    
    <!-- Reflector B (inside ring) -->
    <path d="M 100 120 Q 180 80 260 120 L 250 130 Q 180 100 110 130 Z" fill="url(#reflector)" stroke="#90A4AE" stroke-width="2"/>
    
    <!-- Light bulb C -->
    <ellipse cx="180" cy="140" rx="25" ry="30" fill="url(#bulb)" stroke="#F9A825" stroke-width="2"/>
    <rect x="170" y="165" width="20" height="10" fill="#B0BEC5" stroke="#78909C" stroke-width="1"/>
    
    <!-- Light rays -->
    <line x1="180" y1="170" x2="180" y2="280" stroke="#FFC107" stroke-width="3"/>
    <line x1="180" y1="170" x2="100" y2="280" stroke="#FFC107" stroke-width="2" opacity="0.6"/>
    <line x1="180" y1="170" x2="260" y2="280" stroke="#FFC107" stroke-width="2" opacity="0.6"/>
    <line x1="180" y1="170" x2="60" y2="250" stroke="#FFC107" stroke-width="1.5" opacity="0.4"/>
    <line x1="180" y1="170" x2="300" y2="250" stroke="#FFC107" stroke-width="1.5" opacity="0.4"/>
    
    <!-- Light cone -->
    <path d="M 160 170 L 80 280 L 280 280 L 200 170" fill="#FFF9C4" opacity="0.3"/>
    
    <!-- Magnetic field lines inside ring -->
    <circle cx="180" cy="120" r="70" fill="none" stroke="#7B1FA2" stroke-width="1.5" stroke-dasharray="5,3" opacity="0.3"/>
    <circle cx="180" cy="120" r="50" fill="none" stroke="#7B1FA2" stroke-width="1" stroke-dasharray="5,3" opacity="0.25"/>
    
    <!-- Labels -->
    <line x1="290" y1="50" x2="340" y2="35" stroke="#333" stroke-width="1"/>
    <rect x="320" y="22" width="60" height="18" fill="white" stroke="#333" rx="3"/>
    <text x="350" y="35" text-anchor="middle" font-size="12" font-weight="bold" fill="#333">A — Anillo</text>
    <text x="350" y="52" text-anchor="middle" font-size="9" fill="#666">(magnetizado)</text>
    
    <line x1="260" y1="110" x2="340" y2="95" stroke="#333" stroke-width="1"/>
    <rect x="320" y="82" width="60" height="18" fill="white" stroke="#333" rx="3"/>
    <text x="350" y="95" text-anchor="middle" font-size="12" font-weight="bold" fill="#90A4AE">B — Reflector</text>
    
    <line x1="205" y1="140" x2="340" y2="140" stroke="#333" stroke-width="1"/>
    <rect x="320" y="128" width="60" height="18" fill="white" stroke="#333" rx="3"/>
    <text x="350" y="141" text-anchor="middle" font-size="12" font-weight="bold" fill="#F9A825">C — Foco</text>
    
    <!-- Energy input -->
    <line x1="180" y1="10" x2="180" y2="35" stroke="#F9A825" stroke-width="2.5" marker-end="url(#arrowY10)"/>
    <text x="180" y="8" text-anchor="middle" font-size="10" fill="#F9A825" font-weight="bold">⚡ Electricidad positiva</text>
    <text x="180" y="-2" text-anchor="middle" font-size="9" fill="#F9A825">de la atmósfera</text>
  </g>

  <!-- === VIEW 2: CROSS-SECTION (Right) === -->
  <g transform="translate(500, 80)">
    <text x="180" y="15" text-anchor="middle" font-size="13" font-weight="bold" fill="#333">VISTA EN CORTE (Fig. 2)</text>
    
    <!-- Base/tray E -->
    <rect x="80" y="200" width="200" height="20" fill="#8D6E63" stroke="#5D4037" stroke-width="2" rx="3"/>
    
    <!-- Perforations F -->
    <circle cx="120" cy="210" r="5" fill="white" stroke="#5D4037" stroke-width="1"/>
    <circle cx="160" cy="210" r="5" fill="white" stroke="#5D4037" stroke-width="1"/>
    <circle cx="200" cy="210" r="5" fill="white" stroke="#5D4037" stroke-width="1"/>
    <circle cx="240" cy="210" r="5" fill="white" stroke="#5D4037" stroke-width="1"/>
    
    <!-- Support G -->
    <rect x="170" y="220" width="20" height="40" fill="#8D6E63" stroke="#5D4037" stroke-width="1.5"/>
    
    <!-- Ring A (cross section) -->
    <rect x="60" y="100" width="20" height="100" fill="url(#ring10)" stroke="#455A64" stroke-width="2" rx="3"/>
    <rect x="280" y="100" width="20" height="100" fill="url(#ring10)" stroke="#455A64" stroke-width="2" rx="3"/>
    
    <!-- Reflector B (cross section) -->
    <path d="M 80 150 Q 180 110 280 150" fill="none" stroke="#90A4AE" stroke-width="4"/>
    
    <!-- Light bulb C -->
    <ellipse cx="180" cy="145" rx="20" ry="25" fill="url(#bulb)" stroke="#F9A825" stroke-width="2"/>
    
    <!-- Light rays going down -->
    <line x1="180" y1="170" x2="120" y2="205" stroke="#FFC107" stroke-width="2"/>
    <line x1="180" y1="170" x2="180" y2="205" stroke="#FFC107" stroke-width="2.5"/>
    <line x1="180" y1="170" x2="240" y2="205" stroke="#FFC107" stroke-width="2"/>
    
    <!-- Light passing through perforations -->
    <line x1="120" y1="215" x2="120" y2="260" stroke="#FFC107" stroke-width="1.5" opacity="0.6"/>
    <line x1="160" y1="215" x2="160" y2="260" stroke="#FFC107" stroke-width="1.5" opacity="0.6"/>
    <line x1="200" y1="215" x2="200" y2="260" stroke="#FFC107" stroke-width="1.5" opacity="0.6"/>
    <line x1="240" y1="215" x2="240" y2="260" stroke="#FFC107" stroke-width="1.5" opacity="0.6"/>
    
    <!-- Labels -->
    <text x="180" y="95" text-anchor="middle" font-size="10" fill="#455A64" font-weight="bold">A — Anillo magnetizado</text>
    <text x="180" y="135" text-anchor="middle" font-size="10" fill="#90A4AE" font-weight="bold">B — Reflector</text>
    <text x="180" y="165" text-anchor="middle" font-size="10" fill="#F9A825" font-weight="bold">C — Foco de luz</text>
    <text x="320" y="210" font-size="10" fill="#8D6E63" font-weight="bold">E — Bandeja perforada</text>
    <text x="320" y="225" font-size="9" fill="#666">(aberturas F)</text>
    <text x="220" y="245" font-size="10" fill="#8D6E63" font-weight="bold">G — Soporte vertical</text>
  </g>

  <!-- === HOW IT WORKS (Bottom) === -->
  <g transform="translate(50, 380)">
    <text x="400" y="15" text-anchor="middle" font-size="14" font-weight="bold" fill="#333">¿CÓMO FUNCIONA? — La Luz como Vehículo de Electricidad Natural</text>
    
    <!-- Step 1 -->
    <g transform="translate(0, 30)">
      <rect x="0" y="0" width="250" height="80" fill="#E3F2FD" stroke="#1565C0" rx="5"/>
      <circle cx="20" cy="15" r="12" fill="#1565C0"/>
      <text x="20" y="20" text-anchor="middle" font-size="12" font-weight="bold" fill="white">1</text>
      <text x="130" y="18" text-anchor="middle" font-size="11" font-weight="bold" fill="#1565C0">ANILLO MAGNETIZADO</text>
      <text x="130" y="35" text-anchor="middle" font-size="9" fill="#333">El anillo A está cargado de</text>
      <text x="130" y="48" text-anchor="middle" font-size="9" fill="#333">electricidad negativa de la tierra</text>
      <text x="130" y="61" text-anchor="middle" font-size="9" fill="#333">→ Atrae electricidad positiva</text>
      <text x="130" y="74" text-anchor="middle" font-size="9" fill="#333">del aire ambiente</text>
    </g>
    
    <!-- Arrow -->
    <line x1="260" y1="70" x2="310" y2="70" stroke="#1565C0" stroke-width="2" marker-end="url(#arrowY10)"/>
    
    <!-- Step 2 -->
    <g transform="translate(320, 30)">
      <rect x="0" y="0" width="250" height="80" fill="#FFF3E0" stroke="#FF9800" rx="5"/>
      <circle cx="20" cy="15" r="12" fill="#FF9800"/>
      <text x="20" y="20" text-anchor="middle" font-size="12" font-weight="bold" fill="white">2</text>
      <text x="130" y="18" text-anchor="middle" font-size="11" font-weight="bold" fill="#E65100">CAMPO MAGNÉTICO</text>
      <text x="130" y="35" text-anchor="middle" font-size="9" fill="#333">El espacio dentro del anillo</text>
      <text x="130" y="48" text-anchor="middle" font-size="9" fill="#333">se convierte en CAMPO MAGNÉTICO</text>
      <text x="130" y="61" text-anchor="middle" font-size="9" fill="#333">creado por electricidad natural</text>
      <text x="130" y="74" text-anchor="middle" font-size="9" fill="#333">(negativa + positiva combinadas)</text>
    </g>
    
    <!-- Arrow -->
    <line x1="580" y1="70" x2="630" y2="70" stroke="#FF9800" stroke-width="2" marker-end="url(#arrowY10)"/>
    
    <!-- Step 3 -->
    <g transform="translate(640, 30)">
      <rect x="0" y="0" width="150" height="80" fill="#FFF9C4" stroke="#F9A825" rx="5"/>
      <circle cx="20" cy="15" r="12" fill="#F9A825"/>
      <text x="20" y="20" text-anchor="middle" font-size="12" font-weight="bold" fill="white">3</text>
      <text x="80" y="18" text-anchor="middle" font-size="10" font-weight="bold" fill="#F57F17">LUZ + ENERGÍA</text>
      <text x="80" y="35" text-anchor="middle" font-size="9" fill="#333">Los rayos de luz</text>
      <text x="80" y="48" text-anchor="middle" font-size="9" fill="#333">CRUZAN el campo</text>
      <text x="80" y="61" text-anchor="middle" font-size="9" fill="#333">magnético →</text>
      <text x="80" y="74" text-anchor="middle" font-size="9" fill="#333">TOMAN electricidad</text>
    </g>
    
    <!-- Final result -->
    <g transform="translate(0, 125)">
      <rect x="200" y="0" width="400" height="50" fill="#E8F5E9" stroke="#4CAF50" rx="5"/>
      <text x="400" y="18" text-anchor="middle" font-size="12" font-weight="bold" fill="#2E7D32">→ RESULTADO: La luz ilumina Y distribuye electricidad natural</text>
      <text x="400" y="35" text-anchor="middle" font-size="10" fill="#333">Todo espacio alcanzado por la luz recibe electricidad natural = VITALIDAD</text>
    </g>
  </g>

  <!-- Applications diagram -->
  <g transform="translate(50, 570)">
    <text x="400" y="15" text-anchor="middle" font-size="13" font-weight="bold" fill="#333">APLICACIONES</text>
    
    <!-- Home -->
    <g transform="translate(0, 30)">
      <rect x="0" y="0" width="170" height="60" fill="#E3F2FD" stroke="#1565C0" rx="5"/>
      <text x="85" y="18" text-anchor="middle" font-size="11" font-weight="bold" fill="#1565C0">🏠 VIVIENDAS</text>
      <text x="85" y="33" text-anchor="middle" font-size="9" fill="#333">Traer electricidad natural</text>
      <text x="85" y="46" text-anchor="middle" font-size="9" fill="#333">al interior de casas</text>
      <text x="85" y="58" text-anchor="middle" font-size="9" fill="#333">(donde falta contacto con tierra)</text>
    </g>
    
    <!-- Stables -->
    <g transform="translate(190, 30)">
      <rect x="0" y="0" width="170" height="60" fill="#FFF3E0" stroke="#FF9800" rx="5"/>
      <text x="85" y="18" text-anchor="middle" font-size="11" font-weight="bold" fill="#E65100">🐄 ESTABLOS</text>
      <text x="85" y="33" text-anchor="middle" font-size="9" fill="#333">Aumentar vitalidad</text>
      <text x="85" y="46" text-anchor="middle" font-size="9" fill="#333">del ganado</text>
      <text x="85" y="58" text-anchor="middle" font-size="9" fill="#333">(mejor producción)</text>
    </g>
    
    <!-- Chicken coops -->
    <g transform="translate(380, 30)">
      <rect x="0" y="0" width="170" height="60" fill="#E8F5E9" stroke="#4CAF50" rx="5"/>
      <text x="85" y="18" text-anchor="middle" font-size="11" font-weight="bold" fill="#2E7D32">🐔 GALLINEROS</text>
      <text x="85" y="33" text-anchor="middle" font-size="9" fill="#333">Mayor producción</text>
      <text x="85" y="46" text-anchor="middle" font-size="9" fill="#333">de huevos</text>
      <text x="85" y="58" text-anchor="middle" font-size="9" fill="#333">(aves más sanas)</text>
    </g>
    
    <!-- Greenhouses -->
    <g transform="translate(570, 30)">
      <rect x="0" y="0" width="170" height="60" fill="#F3E5F5" stroke="#7B1FA2" rx="5"/>
      <text x="85" y="18" text-anchor="middle" font-size="11" font-weight="bold" fill="#6A1B9A">🌿 INVERNADEROS</text>
      <text x="85" y="33" text-anchor="middle" font-size="9" fill="#333">Aumentar vitalidad</text>
      <text x="85" y="46" text-anchor="middle" font-size="9" fill="#333">y madurez de plantas</text>
      <text x="85" y="58" text-anchor="middle" font-size="9" fill="#333">(ya aisladas por vidrio)</text>
    </g>
  </g>

  <!-- Scientific principle -->
  <g transform="translate(150, 680)">
    <rect x="0" y="0" width="600" height="50" fill="white" stroke="#F9A825" rx="5" opacity="0.95"/>
    <text x="300" y="18" text-anchor="middle" font-size="11" font-weight="bold" fill="#F9A825">PRINCIPIO CIENTÍFICO</text>
    <text x="300" y="35" text-anchor="middle" font-size="10" fill="#333">La electricidad de la naturaleza es la fuente de vida de todo lo que vive en la tierra.</text>
    <text x="300" y="48" text-anchor="middle" font-size="10" fill="#333">Traer esta electricidad al interior de viviendas aumenta la vitalidad de sus habitantes.</text>
  </g>

</svg>
```

---

## Descripción Científica Detallada

### El Problema: Aislamiento Indoor

Los seres humanos modernos pasan la mayoría de su tiempo **dentro de edificios**, donde están parcialmente **privados de las fuerzas electromagnéticas de la naturaleza**:

```
FUERA (Contacto natural)
═════════════════════════
☀ Sol + 💨 Viento + 🌧 Lluvia
     ↓ ↓ ↓ ↓ ↓
┌─────────────────────┐
│  Ser humano         │
│  (contacto directo) │
│  → VITALIDAD MÁXIMA │
└─────────────────────┘

DENTRO (Aislamiento)
═════════════════════
    ╔═══════════════╗
    ║   VIVIENDA    ║
    ║  ┌─────────┐  ║
    ║  │ Humano  │  ║  ← Aislado de fuerzas naturales
    ║  │ (aislado)│  ║  → Vitalidad REDUCIDA
    ║  └─────────┘  ║
    ╚═══════════════╝
```

### La Solución: Luz como Vehículo

Christofleau descubrió que **la luz puede transportar electricidad natural**:

```
MECANISMO DE TRANSMISIÓN
═════════════════════════

1. ANILLO A magnetizado atrae electricidad positiva
              ↓
2. Se crea CAMPO MAGNÉTICO dentro del anillo
              ↓
3. Los rayos de luz CRUZAN este campo
              ↓
4. La luz TOMA electricidad natural del campo
              ↓
5. La luz se TRANSMITE al espacio iluminado
              ↓
6. Todo lo que recibe la luz recibe electricidad

La luz no solo ilumina → ¡también ENERGIZA!
```

### Descripción de Componentes

#### Anillo Metálico (A)
- **Material:** Metal magnético (hierro blando)
- **Forma:** Círculo no cerrado (abierto en la parte superior)
- **Función:**
  - Previamente cargado de electricidad negativa de la tierra
  - Atrae constantemente electricidad positiva de la atmósfera
  - Crea campo magnético en su interior
- **Importancia del círculo no cerrado:** Permite que el campo magnético no se auto-cancele

#### Reflector (B)
- **Material:** Metal pulido (aluminio, plata, acero inoxidable)
- **Forma:** Parabólico o cóncavo
- **Función:**
  - Dirige la luz del foco hacia abajo
  - Concentra los rayos que cruzan el campo magnético
  - Maximiza la distribución de electricidad natural

#### Foco de Luz (C)
- **Tipo:** Incandescente, halógena, o cualquier fuente de luz
- **Función:** Genera rayos de luz que cruzan el campo magnético
- **Nota:** La electricidad del foco se COMPLEMENTA con la electricidad natural

#### Bandeja Perforada (E)
- **Material:** Metal o madera
- **Función:** Sostiene el aparato y permite que la luz pase
- **Aberturas (F):** Permiten que los rayos iluminen el espacio inferior

#### Soporte (G)
- **Función:** Mantiene vertical el aparato
- **Altura:** Ajustable según la aplicación

### Flujo de Energía Completo

```
ATMÓSFERA
    ↓ Electricidad positiva
╔═══════════════╗
║   ANILLO A    ║ ← Magnetizado con electricidad negativa
║  (atrayente)  ║
╚═══════════════╝
    ↓ Campo magnético creado
┌───────────────┐
│   REFLECTOR B │ ← Concentra la luz
│   + FOCO C    │ ← Genera luz
└───────────────┘
    ↓ Rayos de luz cruzan campo magnético
    ↓ Los rayos TOMAN electricidad natural
    ↓
╔═══════════════╗
║  BANDEJA E    ║ ← Perforada (F)
╚═══════════════╝
    ↓ Luz + Electricidad natural
    ↓
┌───────────────┐
│   ESPACIO     │ ← Iluminado Y energizado
│  ILUMINADO    │
│  (vivienda,   │
│   invernadero)│
└───────────────┘
```

### Resultados en Humanos

Según Christofleau, los seres humanos en viviendas con este dispositivo experimentan:

- **Mayor vitalidad** y energía diaria
- **Mejor calidad del sueño**
- **Mayor bienestar** general
- **Reducción de fatiga**
- **Mejora del estado de ánimo**
- **Sin efectos secundarios** (energía 100% natural)

### Resultados en Plantas (Invernaderos)

- **Crecimiento más rápido**
- **Mayor producción** de frutos
- **Mejor calidad** nutritiva
- **Madurez anticipada**
- **Mayor resistencia** a enfermedades

### Especificaciones de Instalación

| Parámetro | Recomendación |
|---|---|
| **Altura** | 2-3 metros sobre el suelo |
| **Orientación del gap** | Superior (hacia el cielo) |
| **Tipo de foco** | Incandescente o halógena (calor有助 al efecto) |
| **Superficie cubierta** | 20-50 m² (según potencia del foco) |
| **Uso** | Continuo (encendido durante horas de uso) |

### Adaptaciones

El aparato puede adaptarse a cualquier modo de iluminación:

1. **Lámparas de mesa** → Anillo alrededor de la lámpara
2. **Luces de techo** → Anillo montado en el techo
3. **Faroles exteriores** → Anillo alrededor del farol
4. **Invernaderos** → Series de anillos a lo largo del techo
5. **Establos/gallineros** → Anillos sobre los comederos

---

## Referencias

- **Patente original:** FR 804141 (1936) — Justin Christofleau
- **Libro:** *Electroculture* by Justin Christofleau (1927)
- **Fuente digital:** [rexresearch.com/ElectroCulture/ChristofleauEC](https://www.rexresearch.com/ElectroCulture/ChristofleauEC/ChristofleauEC.htm)

---

*Documento actualizado con diagramas técnicos modernos y explicaciones científicas detalladas.*  
*Autor original: Justin Christofleau — Traducción y actualización para fines de investigación.*
