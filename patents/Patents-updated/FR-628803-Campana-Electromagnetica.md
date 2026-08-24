# FR 628803 — Campana Electromagnética

**Inventor:** Justin Christofleau  
**Fecha de concesión:** 1927  
**País:** Francia

---

## Resumen de la Invención

Un sistema para **traer electricidad atmosférica y magnetismo terrestre dentro de campanas de vidrio e invernaderos**, donde las plantas normalmente están aisladas de estas fuerzas naturales por el vidrio. Utiliza dos cables de metales diferentes (hierro galvanizado y cobre) que forman una pila natural, complementada por magnetismo terrestre y electricidad estática.

---

## Diagrama Técnico

```svg
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 900 750" font-family="'Segoe UI', Arial, sans-serif">
  <defs>
    <linearGradient id="glass" x1="0" y1="0" x2="1" y2="0">
      <stop offset="0%" stop-color="#E0F7FA" stop-opacity="0.3"/>
      <stop offset="50%" stop-color="#FFFFFF" stop-opacity="0.1"/>
      <stop offset="100%" stop-color="#E0F7FA" stop-opacity="0.3"/>
    </linearGradient>
    <linearGradient id="iron7" x1="0" y1="0" x2="1" y2="0">
      <stop offset="0%" stop-color="#78909C"/>
      <stop offset="50%" stop-color="#B0BEC5"/>
      <stop offset="100%" stop-color="#78909C"/>
    </linearGradient>
    <linearGradient id="copper7" x1="0" y1="0" x2="1" y2="0">
      <stop offset="0%" stop-color="#D4760A"/>
      <stop offset="50%" stop-color="#FFB74D"/>
      <stop offset="100%" stop-color="#D4760A"/>
    </linearGradient>
    <linearGradient id="soil7" x1="0" y1="0" x2="0" y2="1">
      <stop offset="0%" stop-color="#8D6E63"/>
      <stop offset="100%" stop-color="#5D4037"/>
    </linearGradient>
    <linearGradient id="plant7" x1="0" y1="1" x2="0" y2="0">
      <stop offset="0%" stop-color="#388E3C"/>
      <stop offset="100%" stop-color="#66BB6A"/>
    </linearGradient>
    <marker id="arrowY7" markerWidth="10" markerHeight="7" refX="9" refY="3.5" orient="auto">
      <polygon points="0 0, 10 3.5, 0 7" fill="#F9A825"/>
    </marker>
    <marker id="arrowR7" markerWidth="10" markerHeight="7" refX="9" refY="3.5" orient="auto">
      <polygon points="0 0, 10 3.5, 0 7" fill="#D32F2F"/>
    </marker>
    <marker id="arrowB7" markerWidth="10" markerHeight="7" refX="9" refY="3.5" orient="auto">
      <polygon points="0 0, 10 3.5, 0 7" fill="#1565C0"/>
    </marker>
  </defs>

  <!-- Background -->
  <rect width="900" height="750" fill="#FAFAF5"/>

  <!-- Title -->
  <text x="450" y="32" text-anchor="middle" font-size="18" font-weight="bold" fill="#333">FR 628803 — Campana Electromagnética</text>
  <text x="450" y="50" text-anchor="middle" font-size="12" fill="#666">Vista en corte — Traer electricidad atmosférica dentro de campanas de vidrio</text>

  <!-- Ground level -->
  <line x1="30" y1="500" x2="870" y2="500" stroke="#5D4037" stroke-width="3" stroke-dasharray="12,6"/>
  <text x="450" y="492" text-anchor="middle" font-size="11" fill="#5D4037" font-weight="bold">▼ NIVEL DEL SUELO ▼</text>

  <!-- Soil -->
  <rect x="30" y="500" width="840" height="200" fill="url(#soil7)" opacity="0.2" rx="5"/>

  <!-- === MAIN VIEW (Center) === -->
  
  <!-- Glass bell A (dome shape) -->
  <path d="M 250 500 L 250 300 Q 250 150 450 150 Q 650 150 650 300 L 650 500" 
        fill="url(#glass)" stroke="#00BCD4" stroke-width="3"/>
  
  <!-- Holes B at top -->
  <circle cx="380" cy="160" r="8" fill="white" stroke="#00BCD4" stroke-width="2"/>
  <circle cx="520" cy="160" r="8" fill="white" stroke="#00BCD4" stroke-width="2"/>
  
  <!-- Iron galvanized cable D (south side) -->
  <path d="M 380 160 L 380 140 Q 380 120 360 120 L 320 120" fill="none" stroke="url(#iron7)" stroke-width="4"/>
  <!-- Tip pointing south -->
  <polygon points="320,120 310,115 310,125" fill="#78909C"/>
  <!-- Going down into soil on south side -->
  <path d="M 380 160 L 380 300 Q 380 320 350 320 L 320 320 L 320 520" fill="none" stroke="url(#iron7)" stroke-width="4"/>
  
  <!-- Copper cable C (sky-facing) -->
  <path d="M 520 160 L 520 140 Q 520 100 520 80" fill="none" stroke="url(#copper7)" stroke-width="4"/>
  <!-- Sharp tip pointing to sky -->
  <polygon points="520,80 515,65 525,65" fill="#D4760A"/>
  <!-- Going down into soil on north side -->
  <path d="M 520 160 L 520 300 Q 520 320 550 320 L 580 320 L 580 520" fill="none" stroke="url(#copper7)" stroke-width="4"/>
  
  <!-- Connection point F (where cables join) -->
  <rect x="435" y="130" width="30" height="15" fill="#FF9800" stroke="#E65100" stroke-width="2" rx="3"/>
  
  <!-- Plant in center -->
  <!-- Stem -->
  <rect x="447" y="300" width="6" height="150" fill="#4CAF50"/>
  <!-- Leaves -->
  <ellipse cx="435" cy="320" rx="20" ry="8" fill="url(#plant7)" transform="rotate(-20, 435, 320)"/>
  <ellipse cx="465" cy="340" rx="20" ry="8" fill="url(#plant7)" transform="rotate(20, 465, 340)"/>
  <ellipse cx="430" cy="360" rx="18" ry="7" fill="url(#plant7)" transform="rotate(-25, 430, 360)"/>
  <ellipse cx="470" cy="380" rx="18" ry="7" fill="url(#plant7)" transform="rotate(25, 470, 380)"/>
  <ellipse cx="440" cy="400" rx="15" ry="6" fill="url(#plant7)" transform="rotate(-15, 440, 400)"/>
  <ellipse cx="460" cy="420" rx="15" ry="6" fill="url(#plant7)" transform="rotate(15, 460, 420)"/>
  <!-- Roots -->
  <path d="M 450 450 Q 430 480 410 500" fill="none" stroke="#8D6E63" stroke-width="1.5"/>
  <path d="M 450 450 Q 450 480 450 510" fill="none" stroke="#8D6E63" stroke-width="1.5"/>
  <path d="M 450 450 Q 470 480 490 500" fill="none" stroke="#8D6E63" stroke-width="1.5"/>
  
  <!-- Labels -->
  <!-- A - Bell -->
  <line x1="650" y1="300" x2="720" y2="250" stroke="#333" stroke-width="1"/>
  <rect x="700" y="235" width="80" height="18" fill="white" stroke="#333" rx="3"/>
  <text x="740" y="248" text-anchor="middle" font-size="12" font-weight="bold" fill="#333">A — Campana</text>
  <text x="740" y="265" text-anchor="middle" font-size="9" fill="#666">(vidrio perforado)</text>
  
  <!-- B - Holes -->
  <line x1="528" y1="160" x2="620" y2="130" stroke="#333" stroke-width="1"/>
  <rect x="600" y="118" width="50" height="18" fill="white" stroke="#333" rx="3"/>
  <text x="625" y="131" text-anchor="middle" font-size="12" font-weight="bold" fill="#333">B — Agujeros</text>
  
  <!-- C - Copper cable -->
  <line x1="525" y1="80" x2="620" y2="60" stroke="#333" stroke-width="1"/>
  <rect x="600" y="48" width="100" height="18" fill="white" stroke="#333" rx="3"/>
  <text x="650" y="61" text-anchor="middle" font-size="12" font-weight="bold" fill="#D4760A">C — Cobre</text>
  <text x="650" y="78" text-anchor="middle" font-size="9" fill="#666">(punta → cielo)</text>
  
  <!-- D - Iron cable -->
  <line x1="315" y1="120" x2="200" y2="100" stroke="#333" stroke-width="1"/>
  <rect x="120" y="88" width="110" height="18" fill="white" stroke="#333" rx="3"/>
  <text x="175" y="101" text-anchor="middle" font-size="12" font-weight="bold" fill="#78909C">D — Hierro galv.</text>
  <text x="175" y="118" text-anchor="middle" font-size="9" fill="#666">(punta → sur)</text>
  
  <!-- F - Connection -->
  <line x1="465" y1="130" x2="550" y2="105" stroke="#333" stroke-width="1"/>
  <rect x="530" y="93" width="60" height="18" fill="white" stroke="#333" rx="3"/>
  <text x="560" y="106" text-anchor="middle" font-size="12" font-weight="bold" fill="#FF9800">F — Unión</text>
  
  <!-- E - Soil under bell -->
  <line x1="450" y1="520" x2="650" y2="540" stroke="#333" stroke-width="1"/>
  <rect x="630" y="528" width="50" height="18" fill="white" stroke="#333" rx="3"/>
  <text x="655" y="541" text-anchor="middle" font-size="12" font-weight="bold" fill="#5D4037">E — Tierra</text>
  <text x="655" y="558" text-anchor="middle" font-size="9" fill="#666">(baña raíces)</text>

  <!-- Energy arrows -->
  <!-- Static electricity from sky -->
  <line x1="520" y1="30" x2="520" y2="65" stroke="#F9A825" stroke-width="2.5" marker-end="url(#arrowY7)"/>
  <text x="520" y="25" text-anchor="middle" font-size="10" fill="#F9A825" font-weight="bold">⚡ Electricidad estática</text>
  
  <!-- Magnetic force from south -->
  <line x1="270" y1="120" x2="305" y2="120" stroke="#D32F2F" stroke-width="2.5" marker-end="url(#arrowR7)"/>
  <text x="240" y="140" text-anchor="middle" font-size="10" fill="#D32F2F" font-weight="bold">← SUR</text>
  <text x="240" y="152" text-anchor="middle" font-size="9" fill="#D32F2F">Magnetismo terrestre</text>
  
  <!-- Energy flow in soil (circuit) -->
  <path d="M 320 520 Q 320 540 450 540 Q 580 540 580 520" fill="none" stroke="#4CAF50" stroke-width="2" stroke-dasharray="5,3"/>
  <text x="450" y="555" text-anchor="middle" font-size="9" fill="#4CAF50">Circuito cerrado por humedad del suelo</text>

  <!-- Compass -->
  <g transform="translate(120, 250)">
    <circle cx="0" cy="0" r="30" fill="white" stroke="#333" stroke-width="2"/>
    <line x1="0" y1="-24" x2="0" y2="-6" stroke="#D32F2F" stroke-width="3"/>
    <line x1="0" y1="6" x2="0" y2="24" stroke="#1565C0" stroke-width="3"/>
    <text x="0" y="-28" text-anchor="middle" font-size="11" font-weight="bold" fill="#D32F2F">N</text>
    <text x="0" y="38" text-anchor="middle" font-size="11" font-weight="bold" fill="#1565C0">S</text>
    <circle cx="0" cy="0" r="3" fill="#333"/>
  </g>

  <!-- Simplified version (right side) -->
  <g transform="translate(700, 300)">
    <text x="100" y="15" text-anchor="middle" font-size="12" font-weight="bold" fill="#333">VERSIÓN SIMPLIFICADA (H)</text>
    
    <!-- Simple bell -->
    <path d="M 20 200 L 20 100 Q 20 50 100 50 Q 180 50 180 100 L 180 200" 
          fill="url(#glass)" stroke="#00BCD4" stroke-width="2"/>
    
    <!-- Single cable H with two branches -->
    <path d="M 100 50 L 100 30" fill="none" stroke="#8D6E63" stroke-width="3"/>
    <!-- Branch I (south) -->
    <path d="M 100 30 L 60 30 L 50 25" fill="none" stroke="#8D6E63" stroke-width="3"/>
    <polygon points="50,25 45,20 45,30" fill="#8D6E63"/>
    <!-- Branch J (sky) -->
    <path d="M 100 30 L 140 30 L 150 20" fill="none" stroke="#8D6E63" stroke-width="3"/>
    <polygon points="150,20 145,10 155,10" fill="#8D6E63"/>
    
    <!-- Into soil -->
    <path d="M 100 50 L 100 220" fill="none" stroke="#8D6E63" stroke-width="3"/>
    
    <!-- Labels -->
    <text x="50" y="18" text-anchor="middle" font-size="9" fill="#D32F2F" font-weight="bold">I → SUR</text>
    <text x="150" y="18" text-anchor="middle" font-size="9" fill="#1565C0" font-weight="bold">J → CIELO</text>
    <text x="100" y="240" text-anchor="middle" font-size="9" fill="#5D4037">H → TIERRA</text>
  </g>

  <!-- Explanation box -->
  <g transform="translate(50, 600)">
    <rect x="0" y="0" width="800" height="70" fill="white" stroke="#00BCD4" rx="5" opacity="0.95"/>
    <text x="400" y="18" text-anchor="middle" font-size="11" font-weight="bold" fill="#00838F">¿POR QUÉ EL VIDRIO BLOQUEA LAS FUERZAS NATURALES?</text>
    <text x="400" y="35" text-anchor="middle" font-size="10" fill="#333">Las plantas tienen hojas con serraciones que actúan como antenas naturales para recibir fuerzas eléctricas de la atmósfera.</text>
    <text x="400" y="50" text-anchor="middle" font-size="10" fill="#333">El vidrio AISLA completamente a las plantas de estas fuerzas, impidiendo el intercambio eléctrico natural.</text>
    <text x="400" y="65" text-anchor="middle" font-size="10" fill="#333">Los cables C y D TRAEN estas fuerzas al interior de la campana, restaurando el intercambio eléctrico natural.</text>
  </g>

</svg>
```

---

## Descripción Científica Detallada

### El Problema: Aislamiento por el Vidrio

Las campanas de vidrio e invernaderos son útiles para:
- Proteger de heladas y viento
- Mantener temperatura estable
- Acelerar el crecimiento

Pero tienen un **defecto fundamental**: el vidrio **aísla completamente** a las plantas de las fuerzas eléctricas de la naturaleza.

```
PLANTA EN CAMPAPA DE VIDRIO (sin modificación)
═══════════════════════════════════════════════

    Electricidad positiva
    de la atmósfera
         ↓ ↓ ↓
    ═══════════════  ← VIDRIO (bloquea 100%)
    │   PLANTA    │
    │  (aislada)  │
    │             │
    ═══════════════
         ↑ ↑ ↑
    Electricidad negativa
    del suelo

RESULTADO: La planta crece rápido pero
           con MENOR CALIDAD nutritiva
```

### La Solución: Traer la Electricidad al Interior

Christofleau diseñó un sistema que **penetra el vidrio** con dos cables de metales diferentes:

```
PLANTA EN CAMPAPA CON CABLES C y D
════════════════════════════════════

    ⚡ Electricidad estática
         ↓ (punta C)
    ═══════════════  ← VIDRIO (con agujeros B)
    │      C↓      │
    │   PLANTA    │
    │      ↑D      │
    ═══════════════
         ↓ (punta D → SUR)
    Magnetismo terrestre

    + Pila formada por C (cobre) y D (hierro)
      → Circuito cerrado por humedad del suelo
      → Electricidad baña las raíces
```

### Los Tres Mecanismos de Recolección

#### 1. Cobre (C) — Electricidad Estática del Aire
- **Punta afilada hacia el cielo**
- Atrae electricidad estática del aire ambiente
- El cobre es excelente conductor
- **Efecto de punta:** concentra el campo eléctrico

#### 2. Hierro Galvanizado (D) — Magnetismo Terrestre
- **Punta tensada hacia el sur magnético**
- Recoge magnetismo terrestre que se mueve de sur a norte
- El hierro se magnetiza por inducción
- **Orientación crítica:** debe apuntar al sur magnético

#### 3. Pila Natural (C + D) — Circuito Cerrado
- **Dos metales diferentes** hundidos en la tierra
- La humedad del suelo cierra el circuito
- Se crea una **pila galvánica** natural
- **Las raíces de la planta** quedan dentro del circuito
- **Electricidad baña constantemente** las raíces

### Efectos Combinados

```
ENERGÍA QUE RECIBE LA PLANTA
═════════════════════════════

1. ELECTRICIDAD ESTÁTICA DEL AIRE (vía cable C)
   → Crecimiento más rápido
   → Vegetación más abundante

2. MAGNETISMO TERRESTRE (vía cable D)
   → Aumento de fructificación
   → Mayor contenido de alcohol y azúcar
   → Mejores cualidades nutritivas

3. PILA GALVÁNICA (C + D en tierra)
   → Electricidad continua baña raíces
   → Intercambio eléctrico restaurado
   → Vitalidad multiplicada

TOTAL: La planta bajo campana ahora recibe
       las fuerzas naturales que el vidrio bloqueaba
```

### Especificaciones del Dispositivo

| Componente | Material | Orientación | Función |
|---|---|---|---|
| **C** — Cable superior | Cobre | Punta → cielo | Recolección de electricidad estática |
| **D** — Cable inferior | Hierro galvanizado | Punta → sur magnético | Recolección de magnetismo terrestre |
| **F** — Unión | Soldadura por puntos | — | Conecta ambos cables |
| **B** — Agujeros | — | Parte superior de campana | Permiten paso de cables |
| **E** — Extremos en tierra | — | Base interior de campana | Forman pila galvánica |

### Versión Simplificada (H)

Para quien prefiera un dispositivo más simple:

```
        I → SUR (magnetismo)
         ↙
    ─────●─────  ← Cable H con dos ramas
         ↖
        J → CIELO (electricidad estática)
         │
         ↓
      TIERRA (E)

Un solo cable H con dos ramas:
• I apunta al sur (magnetismo)
• J apunta al cielo (electricidad)
• Extremo inferior en tierra (circuito)
```

### Aplicaciones

1. **Campanas de vidrio** para plantas individuales
2. **Invernaderos** completos (múltiples cabless C/D)
3. **Marcos de vidrio** para plantas en exterior
4. **Cualquier superficie transparente** que reciba luz solar

### Resultados Esperados

- **Crecimiento:** Más rápido que en campana sin cables
- **Calidad:** Mayor contenido de azúcar, vitaminas, minerales
- **Fructificación:** Aumento significativo
- **Madurez:** Anticipada
- **Sin químicos:** La electricidad natural reemplaza fertilizantes

---

## Referencias

- **Patente original:** FR 628803 (1927) — Justin Christofleau
- **Libro:** *Electroculture* by Justin Christofleau (1927)
- **Fuente digital:** [rexresearch.com/ElectroCulture/ChristofleauEC](https://www.rexresearch.com/ElectroCulture/ChristofleauEC/ChristofleauEC.htm)

---

*Documento actualizado con diagramas técnicos modernos y explicaciones científicas detalladas.*  
*Autor original: Justin Christofleau — Traducción y actualización para fines de investigación.*
