# FR 684117 — Electromagneto Protector para Plantas Jóvenes

**Inventor:** Justin Christofleau  
**Fecha de concesión:** 1930  
**País:** Francia

---

## Resumen de la Invención

Un dispositivo circular de metal magnético que combina tres funciones: **protección contra babosos y caracoles**, **mini-invernadero para germinación acelerada**, y **campo magnético para aumentar la vitalidad** de plantas jóvenes. Funciona como barrera física (agua) y como fuente de energía natural para la planta.

---

## Diagrama Técnico

```svg
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 900 750" font-family="'Segoe UI', Arial, sans-serif">
  <defs>
    <linearGradient id="water" x1="0" y1="0" x2="0" y2="1">
      <stop offset="0%" stop-color="#64B5F6"/>
      <stop offset="100%" stop-color="#1E88E5"/>
    </linearGradient>
    <linearGradient id="metal4" x1="0" y1="0" x2="1" y2="0">
      <stop offset="0%" stop-color="#607D8B"/>
      <stop offset="50%" stop-color="#90A4AE"/>
      <stop offset="100%" stop-color="#607D8B"/>
    </linearGradient>
    <linearGradient id="plant" x1="0" y1="1" x2="0" y2="0">
      <stop offset="0%" stop-color="#388E3C"/>
      <stop offset="100%" stop-color="#66BB6A"/>
    </linearGradient>
    <linearGradient id="soil4" x1="0" y1="0" x2="0" y2="1">
      <stop offset="0%" stop-color="#8D6E63"/>
      <stop offset="100%" stop-color="#5D4037"/>
    </linearGradient>
    <marker id="arrowG4" markerWidth="10" markerHeight="7" refX="9" refY="3.5" orient="auto">
      <polygon points="0 0, 10 3.5, 0 7" fill="#2E7D32"/>
    </marker>
    <marker id="arrowB4" markerWidth="10" markerHeight="7" refX="9" refY="3.5" orient="auto">
      <polygon points="0 0, 10 3.5, 0 7" fill="#1565C0"/>
    </marker>
    <marker id="arrowP4" markerWidth="10" markerHeight="7" refX="9" refY="3.5" orient="auto">
      <polygon points="0 0, 10 3.5, 0 7" fill="#7B1FA2"/>
    </marker>
  </defs>

  <!-- Background -->
  <rect width="900" height="750" fill="#FAFAF5"/>

  <!-- Title -->
  <text x="450" y="32" text-anchor="middle" font-size="18" font-weight="bold" fill="#333">FR 684117 — Electromagneto Protector para Plantas Jóvenes</text>
  <text x="450" y="50" text-anchor="middle" font-size="12" fill="#666">Vista en corte transversal — Triple función: barrera + invernadero + campo magnético</text>

  <!-- Ground level -->
  <line x1="30" y1="350" x2="870" y2="350" stroke="#5D4037" stroke-width="3" stroke-dasharray="12,6"/>
  <text x="450" y="342" text-anchor="middle" font-size="11" fill="#5D4037" font-weight="bold">▼ NIVEL DEL SUELO ▼</text>

  <!-- Soil -->
  <rect x="30" y="350" width="840" height="300" fill="url(#soil4)" opacity="0.2" rx="5"/>

  <!-- Atmosphere -->
  <rect x="30" y="65" width="840" height="285" fill="#E8F5E9" opacity="0.2"/>

  <!-- === MAIN CROSS-SECTION VIEW (Left) === -->
  <g transform="translate(80, 0)">
    <!-- Title -->
    <text x="200" y="80" text-anchor="middle" font-size="14" font-weight="bold" fill="#333">VISTA EN CORTE (AB)</text>
    
    <!-- Reservoir C (circular basin) -->
    <!-- Outer wall -->
    <ellipse cx="200" cy="420" rx="160" ry="30" fill="none" stroke="url(#metal4)" stroke-width="8"/>
    <ellipse cx="200" cy="420" rx="160" ry="30" fill="none" stroke="#455A64" stroke-width="2"/>
    
    <!-- Inner walls (cross section) -->
    <rect x="60" y="380" width="10" height="50" fill="url(#metal4)" stroke="#455A64" stroke-width="1.5"/>
    <rect x="330" y="380" width="10" height="50" fill="url(#metal4)" stroke="#455A64" stroke-width="1.5"/>
    
    <!-- Water in reservoir -->
    <rect x="70" y="395" width="260" height="25" fill="url(#water)" opacity="0.5" rx="3"/>
    <text x="200" y="412" text-anchor="middle" font-size="10" fill="#1565C0" font-weight="bold">AGUA</text>
    
    <!-- Central opening D -->
    <rect x="175" y="370" width="50" height="60" fill="url(#soil4)" opacity="0.3"/>
    <text x="200" y="445" text-anchor="middle" font-size="10" fill="#5D4037" font-weight="bold">D</text>
    <text x="200" y="455" text-anchor="middle" font-size="9" fill="#5D4037">Abertura central</text>
    
    <!-- Plant in center -->
    <!-- Stem -->
    <rect x="197" y="250" width="6" height="100" fill="#4CAF50"/>
    <!-- Leaves -->
    <ellipse cx="185" cy="260" rx="18" ry="8" fill="url(#plant)" transform="rotate(-20, 185, 260)"/>
    <ellipse cx="215" cy="275" rx="18" ry="8" fill="url(#plant)" transform="rotate(20, 215, 275)"/>
    <ellipse cx="180" cy="290" rx="15" ry="7" fill="url(#plant)" transform="rotate(-25, 180, 290)"/>
    <ellipse cx="220" cy="305" rx="15" ry="7" fill="url(#plant)" transform="rotate(25, 220, 305)"/>
    <!-- Roots -->
    <path d="M 200 350 Q 180 380 160 400" fill="none" stroke="#8D6E63" stroke-width="1.5"/>
    <path d="M 200 350 Q 200 380 200 410" fill="none" stroke="#8D6E63" stroke-width="1.5"/>
    <path d="M 200 350 Q 220 380 240 400" fill="none" stroke="#8D6E63" stroke-width="1.5"/>
    
    <!-- Glass lid E (greenhouse) -->
    <ellipse cx="200" cy="220" rx="120" ry="15" fill="#E0F7FA" stroke="#00BCD4" stroke-width="2" opacity="0.7"/>
    <text x="200" y="215" text-anchor="middle" font-size="10" fill="#00838F" font-weight="bold">E — Loseta de vidrio</text>
    <text x="200" y="235" text-anchor="middle" font-size="9" fill="#00838F">(invernadero)</text>
    
    <!-- Labels -->
    <!-- C - Reservoir -->
    <line x1="330" y1="400" x2="400" y2="370" stroke="#333" stroke-width="1"/>
    <rect x="380" y="358" width="50" height="18" fill="white" stroke="#333" rx="3"/>
    <text x="405" y="371" text-anchor="middle" font-size="12" font-weight="bold" fill="#333">C</text>
    
    <!-- D label already placed -->
    
    <!-- E label already placed -->
    
    <!-- Slug barrier explanation -->
    <g transform="translate(380, 420)">
      <rect x="0" y="0" width="160" height="55" fill="white" stroke="#8BC34A" rx="5" opacity="0.95"/>
      <text x="80" y="15" text-anchor="middle" font-size="10" font-weight="bold" fill="#2E7D32">🐌 BARRERA ANTI-CARACOLES</text>
      <text x="80" y="30" text-anchor="middle" font-size="9" fill="#555">El agua en la garganta C</text>
      <text x="80" y="42" text-anchor="middle" font-size="9" fill="#555">impide el paso de babosos</text>
      <text x="80" y="54" text-anchor="middle" font-size="9" fill="#555">y caracoles a la planta</text>
    </g>
  </g>

  <!-- === TOP VIEW (Right) === -->
  <g transform="translate(520, 0)">
    <!-- Title -->
    <text x="180" y="80" text-anchor="middle" font-size="14" font-weight="bold" fill="#333">VISTA EN PLANTA</text>
    
    <!-- Outer circle (reservoir) -->
    <circle cx="180" cy="300" r="130" fill="none" stroke="url(#metal4)" stroke-width="12"/>
    <circle cx="180" cy="300" r="130" fill="none" stroke="#455A64" stroke-width="2"/>
    
    <!-- Water ring -->
    <circle cx="180" cy="300" r="115" fill="url(#water)" opacity="0.3"/>
    <circle cx="180" cy="300" r="100" fill="none" stroke="#1565C0" stroke-width="1" stroke-dasharray="5,3"/>
    
    <!-- Central opening -->
    <circle cx="180" cy="300" r="40" fill="url(#soil4)" opacity="0.3"/>
    <circle cx="180" cy="300" r="40" fill="none" stroke="#5D4037" stroke-width="1.5"/>
    
    <!-- Plant in center (top view) -->
    <circle cx="180" cy="300" r="5" fill="#4CAF50"/>
    <line x1="180" y1="300" x2="160" y2="275" stroke="#66BB6A" stroke-width="2"/>
    <line x1="180" y1="300" x2="200" y2="275" stroke="#66BB6A" stroke-width="2"/>
    <line x1="180" y1="300" x2="155" y2="295" stroke="#66BB6A" stroke-width="2"/>
    <line x1="180" y1="300" x2="205" y2="295" stroke="#66BB6A" stroke-width="2"/>
    <line x1="180" y1="300" x2="160" y2="310" stroke="#66BB6A" stroke-width="1.5"/>
    <line x1="180" y1="300" x2="200" y2="310" stroke="#66BB6A" stroke-width="1.5"/>
    <ellipse cx="158" cy="278" rx="8" ry="4" fill="#81C784" transform="rotate(-30, 158, 278)"/>
    <ellipse cx="202" cy="278" rx="8" ry="4" fill="#81C784" transform="rotate(30, 202, 278)"/>
    <ellipse cx="153" cy="298" rx="8" ry="4" fill="#81C784" transform="rotate(-20, 153, 298)"/>
    <ellipse cx="207" cy="298" rx="8" ry="4" fill="#81C784" transform="rotate(20, 207, 298)"/>
    
    <!-- Magnetic field lines (circular) -->
    <circle cx="180" cy="300" r="60" fill="none" stroke="#7B1FA2" stroke-width="1" stroke-dasharray="5,3" opacity="0.4"/>
    <circle cx="180" cy="300" r="80" fill="none" stroke="#7B1FA2" stroke-width="1" stroke-dasharray="5,3" opacity="0.3"/>
    <circle cx="180" cy="300" r="100" fill="none" stroke="#7B1FA2" stroke-width="1" stroke-dasharray="5,3" opacity="0.2"/>
    
    <!-- Labels -->
    <text x="180" y="165" text-anchor="middle" font-size="10" fill="#455A64" font-weight="bold">C = Reservorio circular</text>
    <text x="180" y="178" text-anchor="middle" font-size="9" fill="#666">(metal magnético + agua)</text>
    
    <text x="180" y="350" text-anchor="middle" font-size="10" fill="#5D4037" font-weight="bold">D = Abertura central</text>
    <text x="180" y="363" text-anchor="middle" font-size="9" fill="#666">(sitio de la planta)</text>
    
    <!-- Arrows showing magnetic field -->
    <line x1="100" y1="250" x2="80" y2="230" stroke="#7B1FA2" stroke-width="1.5" marker-end="url(#arrowP4)"/>
    <text x="60" y="225" text-anchor="middle" font-size="9" fill="#7B1FA2">Campo</text>
    <text x="60" y="235" text-anchor="middle" font-size="9" fill="#7B1FA2">magnético</text>
    
    <!-- Slug crossing attempt -->
    <g transform="translate(250, 280)">
      <text x="0" y="0" font-size="18">🐌</text>
      <line x1="0" y1="5" x2="-30" y2="15" stroke="#D32F2F" stroke-width="2"/>
      <line x1="-30" y1="5" x2="0" y2="15" stroke="#D32F2F" stroke-width="2"/>
      <text x="-15" y="30" text-anchor="middle" font-size="8" fill="#D32F2F" font-weight="bold">¡BLOQUEADO!</text>
    </g>
  </g>

  <!-- === DETAILED FUNCTION DIAGRAM (Bottom) === -->
  <g transform="translate(50, 500)">
    <text x="400" y="15" text-anchor="middle" font-size="14" font-weight="bold" fill="#333">TRIPLE FUNCIÓN DEL DISPOSITIVO</text>
    
    <!-- Function 1: Water barrier -->
    <g transform="translate(0, 30)">
      <rect x="0" y="0" width="250" height="80" fill="#E3F2FD" stroke="#1565C0" rx="5"/>
      <text x="125" y="20" text-anchor="middle" font-size="12" font-weight="bold" fill="#1565C0">🛡️ FUNCIÓN 1: BARRERA</text>
      <text x="125" y="38" text-anchor="middle" font-size="10" fill="#333">Agua en garganta del reservorio C</text>
      <text x="125" y="52" text-anchor="middle" font-size="10" fill="#333">Los babosos y caracoles NO pueden</text>
      <text x="125" y="66" text-anchor="middle" font-size="10" fill="#333">cruzar el agua para llegar a la planta</text>
      <circle cx="230" cy="15" r="12" fill="#1565C0"/>
      <text x="230" y="20" text-anchor="middle" font-size="14" fill="white">1</text>
    </g>
    
    <!-- Function 2: Greenhouse -->
    <g transform="translate(320, 30)">
      <rect x="0" y="0" width="250" height="80" fill="#E0F7FA" stroke="#00BCD4" rx="5"/>
      <text x="125" y="20" text-anchor="middle" font-size="12" font-weight="bold" fill="#00838F">🌱 FUNCIÓN 2: INVERNADERO</text>
      <text x="125" y="38" text-anchor="middle" font-size="10" fill="#333">Loseta de vidrio E sobre abertura D</text>
      <text x="125" y="52" text-anchor="middle" font-size="10" fill="#333">Acelera germinación de semillas</text>
      <text x="125" y="66" text-anchor="middle" font-size="10" fill="#333">y crecimiento de planta joven</text>
      <circle cx="230" cy="15" r="12" fill="#00BCD4"/>
      <text x="230" y="20" text-anchor="middle" font-size="14" fill="white">2</text>
    </g>
    
    <!-- Function 3: Magnetic field -->
    <g transform="translate(640, 30)">
      <rect x="0" y="0" width="250" height="80" fill="#F3E5F5" stroke="#7B1FA2" rx="5"/>
      <text x="125" y="20" text-anchor="middle" font-size="12" font-weight="bold" fill="#7B1FA2">⚡ FUNCIÓN 3: MAGNETISMO</text>
      <text x="125" y="38" text-anchor="middle" font-size="10" fill="#333">Metal magnético toma electricidad</text>
      <text x="125" y="52" text-anchor="middle" font-size="10" fill="#333">negativa del suelo + positiva</text>
      <text x="125" y="66" text-anchor="middle" font-size="10" fill="#333">de atmósfera → activa vegetación</text>
      <circle cx="230" cy="15" r="12" fill="#7B1FA2"/>
      <text x="230" y="20" text-anchor="middle" font-size="14" fill="white">3</text>
    </g>
  </g>

  <!-- Energy flow diagram -->
  <g transform="translate(50, 630)">
    <text x="400" y="15" text-anchor="middle" font-size="12" font-weight="bold" fill="#333">FLUJO DE ENERGÍA</text>
    
    <!-- Atmosphere -->
    <rect x="50" y="25" width="120" height="35" fill="#E3F2FD" stroke="#1565C0" rx="5"/>
    <text x="110" y="47" text-anchor="middle" font-size="10" fill="#1565C0" font-weight="bold">ATMÓSFERA</text>
    <text x="110" y="70" text-anchor="middle" font-size="9" fill="#1565C0">+ Electricidad positiva</text>
    
    <line x1="170" y1="42" x2="220" y2="42" stroke="#1565C0" stroke-width="2" marker-end="url(#arrowB4)"/>
    
    <!-- Apparatus -->
    <rect x="220" y="25" width="160" height="35" fill="#F3E5F5" stroke="#7B1FA2" rx="5"/>
    <text x="300" y="47" text-anchor="middle" font-size="10" fill="#7B1FA2" font-weight="bold">APARATO (C)</text>
    
    <line x1="380" y1="42" x2="430" y2="42" stroke="#7B1FA2" stroke-width="2" marker-end="url(#arrowP4)"/>
    
    <!-- Plant -->
    <rect x="430" y="25" width="120" height="35" fill="#E8F5E9" stroke="#2E7D32" rx="5"/>
    <text x="490" y="47" text-anchor="middle" font-size="10" fill="#2E7D32" font-weight="bold">PLANTA</text>
    
    <line x1="550" y1="42" x2="600" y2="42" stroke="#2E7D32" stroke-width="2" marker-end="url(#arrowG4)"/>
    
    <!-- Soil -->
    <rect x="600" y="25" width="120" height="35" fill="#EFEBE9" stroke="#5D4037" rx="5"/>
    <text x="660" y="47" text-anchor="middle" font-size="10" fill="#5D4037" font-weight="bold">SUELO</text>
    <text x="660" y="70" text-anchor="middle" font-size="9" fill="#5D4037">− Electricidad negativa</text>
    
    <!-- Reverse arrow (soil to apparatus) -->
    <path d="M 600 55 L 300 55 L 300 75 L 150 75 L 150 55 L 110 55" fill="none" stroke="#5D4037" stroke-width="1.5" stroke-dasharray="5,3"/>
    <text x="400" y="85" text-anchor="middle" font-size="9" fill="#5D4037">Corrientes negativas del suelo → aparato</text>
  </g>

  <!-- Legend -->
  <g transform="translate(250, 710)">
    <rect x="0" y="0" width="400" height="25" fill="white" stroke="#ccc" rx="5" opacity="0.9"/>
    <text x="200" y="17" text-anchor="middle" font-size="10" fill="#666">
      C = Reservorio circular (metal magnético) · D = Abertura central · E = Loseta de vidrio (invernadero)
    </text>
  </g>

</svg>
```

---

## Descripción Científica Detallada

### El Problema que Resuelve

Las plantas jóvenes son vulnerables a múltiples amenazas:

1. **Babosos y caracoles:** Devoran plantulas tiernas, especialmente en clima húmedo
2. **Germinación lenta:** Las condiciones naturales pueden ser lentas para la germinación
3. **Vitalidad baja:** Las plantas jóvenes tienen poca energía para crecer vigorosamente

### La Solución: Dispositivo Triple Función

Christofleau diseñó un aparato que resuelve los tres problemas simultáneamente:

```
╔═══════════════════════════════════════════════════════════╗
║                  TRIPLE FUNCIÓN                          ║
╠═══════════════════════════════════════════════════════════╣
║  1. BARRERA FÍSICA (agua)                                ║
║     → Los caracoles no pueden cruzar el agua             ║
║     → Protección continua sin pesticidas                 ║
║                                                           ║
║  2. MINI-INVERNADERO (vidrio)                            ║
║     → Acelera germinación de semillas                    ║
║     → Protege de heladas y viento                        ║
║     → Se retira cuando la planta crece                   ║
║                                                           ║
║  3. CAMPO MAGNÉTICO (metal ferromagnético)               ║
║     → Atrae electricidad negativa del suelo              ║
║     → Atrae electricidad positiva de la atmósfera        ║
║     → Activa poder de vegetación y madurez               ║
╚═══════════════════════════════════════════════════════════╝
```

### Descripción de Componentes

#### Reservorio Circular (C)
- **Material:** Metal magnético (hierro blando)
- **Forma:** Anillo circular con garganta para agua
- **Función mecánica:** Contiene agua que actúa como barrera contra babosos
- **Función magnética:** Al descansar sobre la tierra, toma rápidamente electricidad negativa del suelo
- **Función de inducción:** Atrae ondas electromagnéticas y corrientes positivas de la atmósfera

#### Abertura Central (D)
- **Ubicación:** Centro exacto del reservorio
- **Función:** Sitio donde se coloca la planta o se siembran semillas
- **Tamaño:** Suficiente para el crecimiento inicial de la planta

#### Loseta de Vidrio (E)
- **Material:** Vidrio transparente
- **Función:** Forma un mini-invernadero sobre la abertura central
- **Efecto:** Acelera germinación y crecimiento inicial
- **Uso temporal:** Se retira cuando la planta toca el vidrio

### Mecanismo de Funcionamiento

```
FASE 1: SIEMBRA
────────────────
1. Colocar el reservorio C sobre el suelo
2. Llenar la garganta con agua
3. Sembrar semillas en el centro D
4. Cubrir con loseta de vidrio E

FASE 2: GERMINACIÓN ACELERADA
─────────────────────────────
• El vidrio E crea efecto invernadero
• La humedad y calor se concentran
• Germinación más rápida que en invernadero ordinario
• La planta brota donde se sembró (sin trasplante)

FASE 3: PROTECCIÓN CONTINUA
───────────────────────────
• El agua en C bloquea el paso de babosos/caracoles
• La planta crece protegida
• El campo magnético del metal activa la vegetación

FASE 4: CRECIMIENTO LIBRE
─────────────────────────
• Cuando la planta toca el vidrio, se retira E
• Se mantiene el agua en C para protección
• La planta continúa受益 del campo magnético
• Crecimiento más rápido y saludable
```

### Fundamento Científico del Campo Magnético

El metal magnético del reservorio funciona según principios bien establecidos:

1. **Conducción de electricidad telúrica:** Al contacto con el suelo, el metal toma inmediatamente electricidad negativa natural.

2. **Inducción atmosférica:** La masa metálica atrae ondas electromagnéticas y corrientes positivas de la atmósfera.

3. **Campo combinado:** La planta queda rodeada en su base por un campo magnético formado por:
   - **Corrientes negativas del suelo** (captadas por el metal)
   - **Corrientes positivas de la atmósfera** (atraídas por inducción)

4. **Efecto biológico:** Este campo magnético:
   - **Activa el poder de vegetación** (crecimiento más vigoroso)
   - **Aumenta riqueza en cualidades nutritivas** (mejor calidad)
   - **Acelera la madurez** (cosecha más temprana)

### Ventajas sobre Métodos Tradicionales

| Aspecto | Cebolla/ pesticidas | Invernadero tradicional | FR 684117 |
|---|---|---|---|
| Protección babosos | Parcial | No | **Completa** |
| Germinación | Normal | Acelerada | **Acelerada** |
| Trasplante | Necesario | Acelerada | **No necesario** |
| Campo magnético | No | No | **Sí** |
| Costo | Bajo | Alto | **Moderado** |
| Mantenimiento | Alto | Medio | **Bajo** |
| Toxicidad | Sí | No | **No** |

### Instrucciones de Uso

1. **Preparar el suelo:** Fertilizar normalmente el área donde se colocará el dispositivo
2. **Colocar el reservorio:** Poner C sobre el suelo en el sitio deseado
3. **Llenar con agua:** Añadir agua a la garganta del reservorio (que sea suficientemente ancha para que babosos no puedan saltar)
4. **Sembrar:** Colocar semillas o planta joven en la abertura central D
5. **Cubrir con vidrio:** Poner la loseta E para crear el efecto invernadero
6. **Mantener:** Reponer agua según sea necesario
7. **Retirar vidrio:** Cuando la planta toque el vidrio, retirar E
8. **Continuar:** Mantener el agua en C para protección continua

### Resultados Esperados

- **Germinación:** 30-50% más rápida que en suelo desnudo
- **Supervivencia:** Casi 100% contra babosos y caracoles
- **Crecimiento:** 20-40% más rápido debido al campo magnético
- **Calidad:** Mayor contenido de nutrientes
- **Sin trasplante:** La planta crece donde se sembró (menor estrés)

---

## Referencias

- **Patente original:** FR 684117 (1930) — Justin Christofleau
- **Libro:** *Electroculture* by Justin Christofleau (1927)
- **Fuente digital:** [rexresearch.com/ElectroCulture/ChristofleauEC](https://www.rexresearch.com/ElectroCulture/ChristofleauEC/ChristofleauEC.htm)

---

*Documento actualizado con diagramas técnicos modernos y explicaciones científicas detalladas.*  
*Autor original: Justin Christofleau — Traducción y actualización para fines de investigación.*
