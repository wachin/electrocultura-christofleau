# FR 829789 — Fertilizador Electromagnético

**Inventor:** Justin Christofleau  
**Fecha de concesión:** 1938  
**País:** Francia

---

## Resumen de la Invención

Un dispositivo subterráneo de hierro fundido en forma de imán alargado, equipado con aletas de recolección, diseñado para captar y concentrar las corrientes magnéticas terrestres y la electricidad estática del suelo, distribuyéndolas en la tierra cultivada para aumentar la productividad agrícola.

---

## Diagrama Técnico

```svg
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 900 700" font-family="'Segoe UI', Arial, sans-serif">
  <defs>
    <linearGradient id="soil" x1="0" y1="0" x2="0" y2="1">
      <stop offset="0%" stop-color="#8B6914"/>
      <stop offset="100%" stop-color="#654321"/>
    </linearGradient>
    <linearGradient id="iron" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0%" stop-color="#708090"/>
      <stop offset="50%" stop-color="#A9A9A9"/>
      <stop offset="100%" stop-color="#708090"/>
    </linearGradient>
    <linearGradient id="copper" x1="0" y1="0" x2="0" y2="1">
      <stop offset="0%" stop-color="#D4760A"/>
      <stop offset="100%" stop-color="#B87333"/>
    </linearGradient>
    <marker id="arrowRed" markerWidth="10" markerHeight="7" refX="9" refY="3.5" orient="auto">
      <polygon points="0 0, 10 3.5, 0 7" fill="#D32F2F"/>
    </marker>
    <marker id="arrowBlue" markerWidth="10" markerHeight="7" refX="9" refY="3.5" orient="auto">
      <polygon points="0 0, 10 3.5, 0 7" fill="#1565C0"/>
    </marker>
    <marker id="arrowGreen" markerWidth="10" markerHeight="7" refX="9" refY="3.5" orient="auto">
      <polygon points="0 0, 10 3.5, 0 7" fill="#2E7D32"/>
    </marker>
  </defs>

  <!-- Background -->
  <rect width="900" height="700" fill="#F5F5F0"/>

  <!-- Title -->
  <text x="450" y="35" text-anchor="middle" font-size="20" font-weight="bold" fill="#333">FR 829789 — Fertilizador Electromagnético</text>
  <text x="450" y="55" text-anchor="middle" font-size="13" fill="#666">Vista lateral en sección — Instalación subterránea</text>

  <!-- Ground level line -->
  <line x1="50" y1="280" x2="850" y2="280" stroke="#5D4037" stroke-width="3" stroke-dasharray="12,6"/>
  <text x="460" y="272" text-anchor="middle" font-size="12" fill="#5D4037" font-weight="bold">▼ NIVEL DEL SUELO ▼</text>

  <!-- Soil background -->
  <rect x="50" y="280" width="800" height="350" fill="url(#soil)" opacity="0.3" rx="5"/>

  <!-- Atmosphere area -->
  <rect x="50" y="65" width="800" height="215" fill="#E3F2FD" opacity="0.3" rx="5"/>
  <text x="450" y="90" text-anchor="middle" font-size="12" fill="#1565C0" font-style="italic">ATMÓSFERA — Electricidad positiva</text>

  <!-- Magnetic field lines (Earth's) -->
  <path d="M 150 200 Q 200 150 250 200 Q 300 250 350 200 Q 400 150 450 200 Q 500 250 550 200 Q 600 150 650 200 Q 700 250 750 200" 
        fill="none" stroke="#E57373" stroke-width="1.5" stroke-dasharray="8,4" opacity="0.5"/>
  <text x="450" y="175" text-anchor="middle" font-size="10" fill="#E57373">Corrientes magnéticas terrestres (S → N)</text>

  <!-- === THE APPARATUS === -->
  
  <!-- Main body A - elongated magnet shape -->
  <path d="M 250 380 L 250 520 Q 250 540 270 540 L 480 540 Q 500 540 500 520 L 500 380 Z" 
        fill="url(#iron)" stroke="#455A64" stroke-width="2"/>
  
  <!-- South tip B (pointed) -->
  <polygon points="250,380 250,520 200,450" fill="url(#iron)" stroke="#455A64" stroke-width="2"/>
  
  <!-- Label A - Main body -->
  <line x1="375" y1="420" x2="375" y2="360" stroke="#333" stroke-width="1"/>
  <rect x="355" y="340" width="40" height="20" fill="white" stroke="#333" rx="3"/>
  <text x="375" y="354" text-anchor="middle" font-size="13" font-weight="bold" fill="#333">A</text>
  <text x="375" y="335" text-anchor="middle" font-size="9" fill="#666">Cuerpo de hierro</text>
  <text x="375" y="325" text-anchor="middle" font-size="9" fill="#666">fundido (imán)</text>

  <!-- Label B - South tip -->
  <line x1="210" y1="440" x2="140" y2="400" stroke="#333" stroke-width="1"/>
  <rect x="100" y="383" width="80" height="20" fill="white" stroke="#333" rx="3"/>
  <text x="140" y="397" text-anchor="middle" font-size="13" font-weight="bold" fill="#333">B</text>
  <text x="140" y="378" text-anchor="middle" font-size="9" fill="#666">Punta sur</text>
  <text x="140" y="368" text-anchor="middle" font-size="9" fill="#666">(recolección S→N)</text>

  <!-- Fin C1 (top) -->
  <rect x="260" y="340" width="8" height="40" fill="#78909C" stroke="#455A64" stroke-width="1"/>
  <rect x="300" y="340" width="8" height="40" fill="#78909C" stroke="#455A64" stroke-width="1"/>
  <rect x="340" y="340" width="8" height="40" fill="#78909C" stroke="#455A64" stroke-width="1"/>
  <rect x="380" y="340" width="8" height="40" fill="#78909C" stroke="#455A64" stroke-width="1"/>
  <rect x="420" y="340" width="8" height="40" fill="#78909C" stroke="#455A64" stroke-width="1"/>
  <rect x="460" y="340" width="8" height="40" fill="#78909C" stroke="#455A64" stroke-width="1"/>

  <!-- Fin C2 (bottom) -->
  <rect x="260" y="520" width="8" height="40" fill="#78909C" stroke="#455A64" stroke-width="1"/>
  <rect x="300" y="520" width="8" height="40" fill="#78909C" stroke="#455A64" stroke-width="1"/>
  <rect x="340" y="520" width="8" height="40" fill="#78909C" stroke="#455A64" stroke-width="1"/>
  <rect x="380" y="520" width="8" height="40" fill="#78909C" stroke="#455A64" stroke-width="1"/>
  <rect x="420" y="520" width="8" height="40" fill="#78909C" stroke="#455A64" stroke-width="1"/>
  <rect x="460" y="520" width="8" height="40" fill="#78909C" stroke="#455A64" stroke-width="1"/>

  <!-- Label C - Fins -->
  <line x1="430" y1="355" x2="570" y2="310" stroke="#333" stroke-width="1"/>
  <rect x="540" y="293" width="80" height="20" fill="white" stroke="#333" rx="3"/>
  <text x="580" y="307" text-anchor="middle" font-size="13" font-weight="bold" fill="#333">C</text>
  <text x="580" y="288" text-anchor="middle" font-size="9" fill="#666">Aletas (antenas)</text>
  <text x="580" y="278" text-anchor="middle" font-size="9" fill="#666">contacto con suelo</text>

  <!-- Metal range D (between poles) -->
  <rect x="260" y="443" width="240" height="6" fill="url(#copper)" stroke="#8D6E63" stroke-width="1"/>
  
  <!-- Insulating piece E -->
  <rect x="260" y="440" width="240" height="12" fill="none" stroke="#FF9800" stroke-width="1.5" stroke-dasharray="4,2"/>
  
  <!-- Label D -->
  <line x1="380" y1="455" x2="380" y2="490" stroke="#333" stroke-width="1"/>
  <rect x="360" y="490" width="40" height="20" fill="white" stroke="#333" rx="3"/>
  <text x="380" y="504" text-anchor="middle" font-size="13" font-weight="bold" fill="#333">D</text>
  <text x="380" y="520" text-anchor="middle" font-size="9" fill="#666">Rango metálico</text>

  <!-- Label E - Insulator -->
  <line x1="490" y1="446" x2="580" y2="420" stroke="#333" stroke-width="1"/>
  <rect x="555" y="405" width="60" height="20" fill="white" stroke="#333" rx="3"/>
  <text x="585" y="419" text-anchor="middle" font-size="13" font-weight="bold" fill="#333">E</text>
  <text x="585" y="438" text-anchor="middle" font-size="9" fill="#666">Aislante</text>

  <!-- Small bars I -->
  <rect x="300" y="441" width="3" height="10" fill="#FF9800"/>
  <rect x="380" y="441" width="3" height="10" fill="#FF9800"/>
  <rect x="460" y="441" width="3" height="10" fill="#FF9800"/>
  
  <!-- Label I -->
  <line x1="303" y1="446" x2="303" y2="415" stroke="#333" stroke-width="1"/>
  <text x="303" y="412" text-anchor="middle" font-size="10" font-weight="bold" fill="#333">I</text>

  <!-- Opening G -->
  <rect x="492" y="445" width="12" height="12" fill="white" stroke="#333" stroke-width="1.5"/>
  <line x1="498" y1="445" x2="498" y2="430" stroke="#333" stroke-width="1"/>
  <text x="498" y="425" text-anchor="middle" font-size="11" font-weight="bold" fill="#333">G</text>
  <text x="498" y="415" text-anchor="middle" font-size="9" fill="#666">Abertura</text>

  <!-- Conductor H (exits north side) -->
  <path d="M 504 451 L 540 451 L 540 560 L 600 560" fill="none" stroke="#C62828" stroke-width="2.5"/>
  <circle cx="540" cy="560" r="4" fill="#C62828"/>
  
  <!-- Label H -->
  <line x1="540" y1="530" x2="620" y2="510" stroke="#333" stroke-width="1"/>
  <rect x="595" y="498" width="80" height="20" fill="white" stroke="#333" rx="3"/>
  <text x="635" y="512" text-anchor="middle" font-size="13" font-weight="bold" fill="#333">H</text>
  <text x="635" y="528" text-anchor="middle" font-size="9" fill="#666">Conductor de salida</text>
  <text x="635" y="538" text-anchor="middle" font-size="9" fill="#666">→ al suelo cultivado</text>

  <!-- Energy flow arrows in soil -->
  <line x1="200" y1="580" x2="280" y2="580" stroke="#2E7D32" stroke-width="2" marker-end="url(#arrowGreen)"/>
  <line x1="300" y1="600" x2="380" y2="600" stroke="#2E7D32" stroke-width="2" marker-end="url(#arrowGreen)"/>
  <line x1="400" y1="620" x2="480" y2="620" stroke="#2E7D32" stroke-width="2" marker-end="url(#arrowGreen)"/>
  <text x="350" y="645" text-anchor="middle" font-size="10" fill="#2E7D32" font-style="italic">Distribución de energía en suelo cultivado</text>

  <!-- Magnetic poles indicator -->
  <rect x="160" y="560" width="30" height="20" fill="#D32F2F" rx="3"/>
  <text x="175" y="574" text-anchor="middle" font-size="12" font-weight="bold" fill="white">S</text>
  
  <rect x="530" y="380" width="30" height="20" fill="#1565C0" rx="3"/>
  <text x="545" y="394" text-anchor="middle" font-size="12" font-weight="bold" fill="white">N</text>

  <!-- Compass indicator -->
  <g transform="translate(780, 120)">
    <circle cx="0" cy="0" r="35" fill="white" stroke="#333" stroke-width="2"/>
    <line x1="0" y1="-28" x2="0" y2="-8" stroke="#D32F2F" stroke-width="3"/>
    <line x1="0" y1="8" x2="0" y2="28" stroke="#1565C0" stroke-width="3"/>
    <text x="0" y="-32" text-anchor="middle" font-size="12" font-weight="bold" fill="#D32F2F">N</text>
    <text x="0" y="42" text-anchor="middle" font-size="12" font-weight="bold" fill="#1565C0">S</text>
    <text x="-40" y="5" text-anchor="middle" font-size="10" fill="#333">O</text>
    <text x="40" y="5" text-anchor="middle" font-size="10" fill="#333">E</text>
    <circle cx="0" cy="0" r="3" fill="#333"/>
  </g>

  <!-- Legend -->
  <g transform="translate(70, 580)">
    <rect x="0" y="0" width="200" height="95" fill="white" stroke="#ccc" rx="5" opacity="0.9"/>
    <text x="100" y="18" text-anchor="middle" font-size="11" font-weight="bold" fill="#333">LEYENDA</text>
    <rect x="15" y="28" width="15" height="10" fill="url(#iron)"/>
    <text x="40" y="37" font-size="9" fill="#333">Hierro fundido (imán)</text>
    <rect x="15" y="45" width="15" height="10" fill="url(#copper)"/>
    <text x="40" y="54" font-size="9" fill="#333">Cobre / metal conductor</text>
    <rect x="15" y="62" width="15" height="10" fill="#78909C"/>
    <text x="40" y="71" font-size="9" fill="#333">Aletas de recolección</text>
    <line x1="15" y1="83" x2="30" y2="83" stroke="#C62828" stroke-width="2.5"/>
    <text x="40" y="87" font-size="9" fill="#333">Conductor de salida</text>
  </g>

  <!-- Depth annotation -->
  <line x1="120" y1="280" x2="120" y2="540" stroke="#333" stroke-width="1" stroke-dasharray="3,3"/>
  <text x="115" y="410" text-anchor="middle" font-size="10" fill="#333" transform="rotate(-90, 115, 410)">Profundidad: bajo arado</text>

</svg>
```

---

## Descripción Científica Detallada

### Principio Fundamental

Este dispositivo se basa en un principio bien establecido de la física: **una barra de hierro blando colocada en la dirección de la aguja de la brújula es inmediatamente atravesada por las corrientes magnéticas terrestres** que se mueven constantemente de sur a norte. El hierro, al ser un material ferromagnético, se magnetiza por inducción y actúa como un conductor de estas fuerzas naturales.

### Componentes y sus Funciones

| Componente | Material | Función |
|---|---|---|
| **A** — Cuerpo principal | Hierro fundido | Masa magnética que actúa como imán permanente. Su forma alargada maximiza la superficie de contacto con las corrientes del suelo. |
| **B** — Punta sur | Hierro fundido | Punta afilada orientada al sur magnético. Su geometría puntiaguda facilita la concentración y captación de las corrientes magnéticas terrestres (S→N). |
| **C** — Aletas (×12) | Hierro fundido | Superficies de contacto que aumentan la interfaz aparato-tierra. Actúan como antenas para atraer la electricidad negativa del suelo. Cada aleta es atravesada por la corriente magnética, amplificando el efecto. |
| **D** — Rango metálico | Metal conductor | Recorre todo el aparato entre los polos. Recoge la energía combinada (negativa del suelo + positiva de la atmósfera) y la transporta al punto de salida. |
| **E** — Pieza aislante | Material cerámico/aislante | Mantiene el rango D a distancia constante de los polos, evitando cortocircuitos internos. |
| **G** — Abertura | — | Punto de fijación del conductor de salida en el extremo norte. |
| **H** — Conductor | Cable metálico | Distribuye la energía recolectada hacia el suelo cultivado mediante una red de cables. |
| **I** — Barras de fijación | Hierro fundido | Sostienen la pieza aislante E, fusionadas con el cuerpo del aparato. |

### Dirección de Instalación

```
         SUR (magnético)
            ↑
            │
     Punta B apunta aquí
            │
   ═══════════════════
   │    APARATO A    │
   │   (orientado S→N)│
   ═══════════════════
            │
            ↓
         NORTE (magnético)
     
   → Cable H sale por el norte
     hacia la red distribuidora
```

### Mecanismo de Funcionamiento

1. **Magnetización por inducción:** Al enterrar el aparato en la dirección exacta S→N magnético, el cuerpo de hierro fundido (A) se magnetiza instantáneamente por las corrientes terrestres.

2. **Recolección de electricidad negativa:** Las aletas (C) aumentan enormemente la superficie de contacto con el suelo, atrayendo la electricidad negativa natural del suelo hacia la masa principal.

3. **Recolección de corrientes verticales:** La aleta superior captación las corrientes atmosféricas positivas que descienden verticalmente, atraídas por inducción electromagnética.

4. **Recolección de corrientes este-oeste:** Las aletas laterales capturan las corrientes terrestres que fluyen en dirección este-oeste (y ocasionalmente oeste-este).

5. **Transporte de energía:** El rango metálico D, mantenido aislado por E, recoge toda la energía (negativa del suelo + positiva de la atmósfera) y la transporta al extremo norte.

6. **Distribución:** Por el conductor H, la energía combinada se distribuye en una red subterránea que baña las raíces de las plantas cultivadas.

### Fundamento Físico

La efectividad de este dispositivo se fundamenta en tres fenómenos bien documentados:

- **Magnetismo terrestre:** La Tierra genera un campo magnético dipolar que crea corrientes magnéticas continuas de sur a norte. Estas corrientes son conductoras de electricidad natural.

- **Electricidad telúrica:** El suelo contiene electricidad negativa natural, producto de la actividad microbiana, la descomposición orgánica y las reacciones geoquímicas. Esta electricidad es esencial para la vida vegetal.

- **Inducción electromagnética:** Al colocar un conductor (el aparato) en un campo magnético variable, se inducen corrientes eléctricas en el conductor, amplificando la energía disponible.

### Especificaciones de Instalación

| Parámetro | Valor recomendado |
|---|---|
| **Profundidad** | 30-50 cm (bajo el nivel de arado) |
| **Orientación** | Sur a Norte magnético (verificar con brújula) |
| **Distancia entre aparatos** | 10-15 metros en terreno regular |
| **Conexión a red** | Cable conductor H → red subterránea |
| **Tipo de suelo** | Cualquier suelo cultivable |

### Resultados Esperados

Según los informes de Christofleau y experimentadores posteriores:

- **Aumento de productividad:** 20-50% más de rendimiento según el cultivo
- **Maduración anticipada:** Semanas antes que en cultivos sin tratamiento
- **Mejora de calidad:** Mayor contenido de azúcar, vitaminas y minerales
- **Salud vegetal:** Mayor resistencia a plagas y enfermedades
- **Sin fertilizantes químicos:** La electricidad natural reemplaza parcialmente los aportes químicos

---

## Referencias

- **Patente original:** FR 829789 (1938) — Justin Christofleau
- **Libro:** *Electroculture* by Justin Christofleau (1927)
- **Fuente digital:** [rexresearch.com/ElectroCulture/ChristofleauEC](https://www.rexresearch.com/ElectroCulture/ChristofleauEC/ChristofleauEC.htm)

---

*Documento actualizado con diagramas técnicos modernos y explicaciones científicas detalladas.*  
*Autor original: Justin Christofleau — Traducción y actualización para fines de investigación.*
