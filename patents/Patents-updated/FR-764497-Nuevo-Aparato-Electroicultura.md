# FR 764497 — Nuevo Aparato de Electroicultura Subterráneo

**Inventor:** Justin Christofleau  
**Fecha de concesión:** 1934  
**País:** Francia

---

## Resumen de la Invención

Versión mejorada del aparato subterráneo de electrocultura (variante de CH 172269), diseñado específicamente para **corregir las desventajas de los mastiles superficiales**: eliminar postes costosos y antiestéticos, reducir la captación excesiva de electricidad estática (que causaba caídas en cereales), y priorizar las corrientes del suelo que aumentan cosechas en cantidad y calidad de forma equilibrada.

---

## Diagrama Técnico

```svg
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 900 800" font-family="'Segoe UI', Arial, sans-serif">
  <defs>
    <linearGradient id="soil3" x1="0" y1="0" x2="0" y2="1">
      <stop offset="0%" stop-color="#8D6E63"/>
      <stop offset="100%" stop-color="#4E342E"/>
    </linearGradient>
    <linearGradient id="iron3" x1="0" y1="0" x2="1" y2="0">
      <stop offset="0%" stop-color="#546E7A"/>
      <stop offset="50%" stop-color="#90A4AE"/>
      <stop offset="100%" stop-color="#546E7A"/>
    </linearGradient>
    <marker id="arrowG3" markerWidth="10" markerHeight="7" refX="9" refY="3.5" orient="auto">
      <polygon points="0 0, 10 3.5, 0 7" fill="#2E7D32"/>
    </marker>
    <marker id="arrowB3" markerWidth="10" markerHeight="7" refX="9" refY="3.5" orient="auto">
      <polygon points="0 0, 10 3.5, 0 7" fill="#1565C0"/>
    </marker>
  </defs>

  <!-- Background -->
  <rect width="900" height="800" fill="#FAFAF5"/>

  <!-- Title -->
  <text x="450" y="32" text-anchor="middle" font-size="18" font-weight="bold" fill="#333">FR 764497 — Nuevo Aparato de Electroicultura Subterráneo</text>
  <text x="450" y="50" text-anchor="middle" font-size="12" fill="#666">Vista completa con red de distribución — Solución a los problemas de mastiles</text>

  <!-- Ground level -->
  <line x1="30" y1="220" x2="870" y2="220" stroke="#5D4037" stroke-width="3" stroke-dasharray="12,6"/>
  <text x="450" y="212" text-anchor="middle" font-size="11" fill="#5D4037" font-weight="bold">▼ NIVEL DEL SUELO ▼</text>

  <!-- Soil layers -->
  <rect x="30" y="220" width="840" height="100" fill="#8D6E63" opacity="0.15"/>
  <text x="450" y="270" text-anchor="middle" font-size="9" fill="#8D6E63" font-style="italic">Capa arable</text>
  
  <rect x="30" y="320" width="840" height="200" fill="url(#soil3)" opacity="0.2"/>
  <text x="450" y="420" text-anchor="middle" font-size="9" fill="#4E342E" font-style="italic">Capa subterránea — Zona de instalación</text>
  
  <rect x="30" y="520" width="840" height="200" fill="#3E2723" opacity="0.15"/>
  <text x="450" y="620" text-anchor="middle" font-size="9" fill="#3E2723" font-style="italic">Subsuelo profundo</text>

  <!-- Atmosphere -->
  <rect x="30" y="55" width="840" height="165" fill="#E8F5E9" opacity="0.3"/>

  <!-- COMPARISON: Mastil vs Subterráneo -->
  
  <!-- Mastil (crossed out) -->
  <g transform="translate(120, 80)">
    <line x1="0" y1="140" x2="0" y2="-60" stroke="#795548" stroke-width="4"/>
    <circle cx="0" cy="-60" r="8" fill="#FFC107" stroke="#F57F17" stroke-width="2"/>
    <line x1="-20" y1="-60" x2="20" y2="-60" stroke="#795548" stroke-width="2"/>
    <line x1="-15" y1="-50" x2="15" y2="-50" stroke="#795548" stroke-width="2"/>
    <!-- X mark -->
    <line x1="-25" y1="-70" x2="25" y2="10" stroke="#D32F2F" stroke-width="3"/>
    <line x1="25" y1="-70" x2="-25" y2="10" stroke="#D32F2F" stroke-width="3"/>
    <text x="0" y="-80" text-anchor="middle" font-size="10" fill="#D32F2F" font-weight="bold">✗ MASTIL</text>
    <text x="0" y="160" text-anchor="middle" font-size="8" fill="#D32F2F">Problemas:</text>
    <text x="0" y="172" text-anchor="middle" font-size="8" fill="#D32F2F">Obstrucción, caídas,</text>
    <text x="0" y="184" text-anchor="middle" font-size="8" fill="#D32F2F">antiestético</text>
  </g>

  <!-- Arrow showing evolution -->
  <line x1="200" y1="150" x2="270" y2="150" stroke="#4CAF50" stroke-width="3" marker-end="url(#arrowG3)"/>
  <text x="235" y="140" text-anchor="middle" font-size="9" fill="#4CAF50" font-weight="bold">EVOLUCIÓN</text>

  <!-- Subterranean apparatus -->
  <g transform="translate(350, 0)">
    <!-- Label -->
    <text x="150" y="100" text-anchor="middle" font-size="10" fill="#2E7D32" font-weight="bold">✓ APARATO SUBTERRÁNEO</text>
    
    <!-- === THE APPARATUS === -->
    
    <!-- Left arm of U -->
    <rect x="80" y="300" width="35" height="160" fill="url(#iron3)" stroke="#455A64" stroke-width="2"/>
    
    <!-- Right arm of U -->
    <rect x="215" y="300" width="35" height="160" fill="url(#iron3)" stroke="#455A64" stroke-width="2"/>
    
    <!-- Bottom of U -->
    <rect x="80" y="445" width="170" height="15" fill="url(#iron3)" stroke="#455A64" stroke-width="2"/>
    
    <!-- South tip B -->
    <polygon points="80,300 80,460 50,380" fill="url(#iron3)" stroke="#455A64" stroke-width="2"/>
    
    <!-- Plate C with teeth -->
    <rect x="60" y="280" width="210" height="10" fill="#78909C" stroke="#455A64" stroke-width="1.5"/>
    
    <!-- Teeth top -->
    <line x1="80" y1="280" x2="80" y2="262" stroke="#78909C" stroke-width="2.5"/>
    <line x1="110" y1="280" x2="110" y2="262" stroke="#78909C" stroke-width="2.5"/>
    <line x1="140" y1="280" x2="140" y2="262" stroke="#78909C" stroke-width="2.5"/>
    <line x1="170" y1="280" x2="170" y2="262" stroke="#78909C" stroke-width="2.5"/>
    <line x1="200" y1="280" x2="200" y2="262" stroke="#78909C" stroke-width="2.5"/>
    <line x1="230" y1="280" x2="230" y2="262" stroke="#78909C" stroke-width="2.5"/>
    <line x1="260" y1="280" x2="260" y2="262" stroke="#78909C" stroke-width="2.5"/>
    
    <!-- Tail teeth (south) -->
    <polygon points="60,285 35,275 35,295 60,290" fill="#78909C" stroke="#455A64" stroke-width="1"/>
    <polygon points="45,283 15,270 15,295 45,290" fill="#78909C" stroke="#455A64" stroke-width="1"/>
    
    <!-- Spikes D -->
    <line x1="90" y1="280" x2="90" y2="250" stroke="#78909C" stroke-width="3"/>
    <line x1="130" y1="280" x2="130" y2="250" stroke="#78909C" stroke-width="3"/>
    <line x1="170" y1="280" x2="170" y2="250" stroke="#78909C" stroke-width="3"/>
    <line x1="210" y1="280" x2="210" y2="250" stroke="#78909C" stroke-width="3"/>
    <line x1="250" y1="280" x2="250" y2="250" stroke="#78909C" stroke-width="3"/>
    
    <!-- Nose E -->
    <path d="M 250,300 L 290,315 L 290,380 L 250,395" fill="url(#iron3)" stroke="#455A64" stroke-width="2"/>
    
    <!-- Bolt F -->
    <circle cx="290" cy="348" r="5" fill="#FF9800" stroke="#E65100" stroke-width="1.5"/>
    
    <!-- Cable G -->
    <path d="M 295 348 L 350 348 L 350 550 L 600 550" fill="none" stroke="#C62828" stroke-width="3"/>
    <path d="M 350 400 L 420 400 L 420 530" fill="none" stroke="#C62828" stroke-width="2"/>
    <path d="M 350 450 L 500 450 L 500 520" fill="none" stroke="#C62828" stroke-width="2"/>
    <path d="M 350 500 L 550 500 L 550 540" fill="none" stroke="#C62828" stroke-width="2"/>
    
    <!-- Clamp H -->
    <rect x="343" y="342" width="14" height="14" fill="#FF9800" stroke="#E65100" stroke-width="1.5" rx="2"/>
    
    <!-- Poles -->
    <rect x="20" y="370" width="22" height="16" fill="#D32F2F" rx="3"/>
    <text x="31" y="382" text-anchor="middle" font-size="10" font-weight="bold" fill="white">S</text>
    
    <rect x="290" y="290" width="22" height="16" fill="#1565C0" rx="3"/>
    <text x="301" y="302" text-anchor="middle" font-size="10" font-weight="bold" fill="white">N</text>
  </g>

  <!-- Labels for apparatus -->
  <g transform="translate(350, 0)">
    <!-- A -->
    <line x1="150" y1="380" x2="150" y2="570" stroke="#333" stroke-width="1"/>
    <rect x="130" y="570" width="40" height="18" fill="white" stroke="#333" rx="3"/>
    <text x="150" y="583" text-anchor="middle" font-size="12" font-weight="bold" fill="#333">A</text>
    
    <!-- B -->
    <line x1="50" y1="380" x2="-20" y2="350" stroke="#333" stroke-width="1"/>
    <rect x="-60" y="338" width="50" height="18" fill="white" stroke="#333" rx="3"/>
    <text x="-35" y="351" text-anchor="middle" font-size="12" font-weight="bold" fill="#333">B</text>
    
    <!-- C -->
    <line x1="165" y1="262" x2="165" y2="235" stroke="#333" stroke-width="1"/>
    <rect x="145" y="225" width="40" height="18" fill="white" stroke="#333" rx="3"/>
    <text x="165" y="238" text-anchor="middle" font-size="12" font-weight="bold" fill="#333">C</text>
    
    <!-- D -->
    <line x1="250" y1="250" x2="310" y2="225" stroke="#333" stroke-width="1"/>
    <rect x="290" y="215" width="40" height="18" fill="white" stroke="#333" rx="3"/>
    <text x="310" y="228" text-anchor="middle" font-size="12" font-weight="bold" fill="#333">D</text>
    
    <!-- E -->
    <line x1="310" y1="348" x2="360" y2="310" stroke="#333" stroke-width="1"/>
    <rect x="340" y="298" width="40" height="18" fill="white" stroke="#333" rx="3"/>
    <text x="360" y="311" text-anchor="middle" font-size="12" font-weight="bold" fill="#333">E</text>
    
    <!-- F -->
    <line x1="310" y1="348" x2="365" y2="380" stroke="#333" stroke-width="1"/>
    <rect x="345" y="370" width="40" height="18" fill="white" stroke="#333" rx="3"/>
    <text x="365" y="383" text-anchor="middle" font-size="12" font-weight="bold" fill="#333">F</text>
    
    <!-- G -->
    <line x1="400" y1="550" x2="450" y2="580" stroke="#333" stroke-width="1"/>
    <rect x="430" y="570" width="40" height="18" fill="white" stroke="#333" rx="3"/>
    <text x="450" y="583" text-anchor="middle" font-size="12" font-weight="bold" fill="#333">G</text>
    
    <!-- H -->
    <line x1="357" y1="342" x2="400" y2="315" stroke="#333" stroke-width="1"/>
    <rect x="380" y="303" width="40" height="18" fill="white" stroke="#333" rx="3"/>
    <text x="400" y="316" text-anchor="middle" font-size="12" font-weight="bold" fill="#333">H</text>
  </g>

  <!-- Energy distribution visualization -->
  <g transform="translate(350, 0)">
    <!-- Energy dots -->
    <circle cx="380" cy="550" r="4" fill="#FF5722" opacity="0.8"/>
    <circle cx="420" cy="530" r="4" fill="#FF5722" opacity="0.8"/>
    <circle cx="460" cy="550" r="4" fill="#FF5722" opacity="0.8"/>
    <circle cx="500" cy="520" r="4" fill="#FF5722" opacity="0.8"/>
    <circle cx="540" cy="540" r="4" fill="#FF5722" opacity="0.8"/>
    <circle cx="500" cy="450" r="4" fill="#FF5722" opacity="0.8"/>
    <circle cx="550" cy="500" r="4" fill="#FF5722" opacity="0.8"/>
    
    <!-- Spread lines -->
    <line x1="380" y1="550" x2="380" y2="570" stroke="#FF5722" stroke-width="1" opacity="0.5"/>
    <line x1="420" y1="530" x2="420" y2="570" stroke="#FF5722" stroke-width="1" opacity="0.5"/>
    <line x1="460" y1="550" x2="460" y2="570" stroke="#FF5722" stroke-width="1" opacity="0.5"/>
    <line x1="500" y1="520" x2="500" y2="570" stroke="#FF5722" stroke-width="1" opacity="0.5"/>
    <line x1="540" y1="540" x2="540" y2="570" stroke="#FF5722" stroke-width="1" opacity="0.5"/>
  </g>

  <!-- Magnetic field visualization -->
  <path d="M 380 350 Q 420 300 460 350 Q 500 400 540 350" fill="none" stroke="#E57373" stroke-width="1" stroke-dasharray="5,3" opacity="0.4"/>
  <path d="M 380 370 Q 420 320 460 370 Q 500 420 540 370" fill="none" stroke="#E57373" stroke-width="1" stroke-dasharray="5,3" opacity="0.3"/>

  <!-- Legend -->
  <g transform="translate(50, 600)">
    <rect x="0" y="0" width="800" height="80" fill="white" stroke="#ccc" rx="5" opacity="0.95"/>
    <text x="400" y="18" text-anchor="middle" font-size="11" font-weight="bold" fill="#333">COMPONENTES Y FUNCIONES</text>
    
    <text x="20" y="38" font-size="10" fill="#333"><tspan font-weight="bold" fill="#455A64">A</tspan> = Cuerpo en U (metal magnético) · <tspan font-weight="bold" fill="#455A64">B</tspan> = Punta sur (recolección S→N) · <tspan font-weight="bold" fill="#455A64">C</tspan> = Placa dentada (corrientes E↔O) · <tspan font-weight="bold" fill="#455A64">D</tspan> = Puntas melladas (inducción atmosférica)</text>
    
    <text x="20" y="55" font-size="10" fill="#333"><tspan font-weight="bold" fill="#455A64">E</tspan> = Nariz norte (salida) · <tspan font-weight="bold" fill="#FF9800">F</tspan> = Perno de conexión · <tspan font-weight="bold" fill="#C62828">G</tspan> = Red distribuidora subterránea · <tspan font-weight="bold" fill="#FF9800">H</tspan> = Abrazadera conductora</text>
    
    <text x="20" y="72" font-size="10" fill="#666">← Punta B (SUR magnético) ────── Nariz E (NORTE magnético) → | Red G orientada S↔N</text>
  </g>

  <!-- Compass -->
  <g transform="translate(820, 130)">
    <circle cx="0" cy="0" r="30" fill="white" stroke="#333" stroke-width="2"/>
    <line x1="0" y1="-24" x2="0" y2="-6" stroke="#D32F2F" stroke-width="3"/>
    <line x1="0" y1="6" x2="0" y2="24" stroke="#1565C0" stroke-width="3"/>
    <text x="0" y="-28" text-anchor="middle" font-size="11" font-weight="bold" fill="#D32F2F">N</text>
    <text x="0" y="38" text-anchor="middle" font-size="11" font-weight="bold" fill="#1565C0">S</text>
    <circle cx="0" cy="0" r="3" fill="#333"/>
  </g>

</svg>
```

---

## Descripción Científica Detallada

### El Problema: Limitaciones de los Mastiles Superficiales

La electrocultura original utilizaba **dispositivos elevados en mastiles** para captar electricidad atmosférica. Aunque efectivos para aumentar cosechas, tenían defectos significativos:

| Problema | Causa | Consecuencia |
|---|---|---|
| **Obstrucción agrícola** | Mastiles en tierras cultivadas | Arados y maquinaria golpeaban los postes |
| **Daño por ganado** | Postes en pastizales | Ganado volcaba los dispositivos |
| **Anti-estético** | Postes visibles cerca de viviendas | Deterioro de la apariencia de propiedades |
| **Caídas de cereales** | Excesiva electricidad estática | Plantas crecían demasiado y se caían |
| **Costo** | Mastiles altos y aparatos grandes | Inversión inicial elevada |

### La Solución: Priorizar Corrientes del Suelo

Christofleau identificó que existen **dos tipos de electricidad** beneficiosas para las plantas:

```
╔══════════════════════════════════════════════════════════╗
║                    ATMÓSFERA                             ║
║   Electricidad POSITIVA estática (rayos, nubes, viento) ║
║   → Aumenta crecimiento VIGOROSO                        ║
║   → Exceso causa CAÍDAS en cereales                     ║
╠══════════════════════════════════════════════════════════╣
║                    SUELO                                 ║
║   Electricidad NEGativa telúrica (actividad microbiana)  ║
║   → Aumenta crecimiento EQUILIBRADO                     ║
║   → Mejora CALIDAD (azúcar, vitaminas, minerales)       ║
║   → Desarrolla VIDA MICROBIANA del suelo                 ║
╚══════════════════════════════════════════════════════════╝
```

**FR 764497 prioriza las corrientes del suelo** sobre las atmosféricas, logrando:
- Cosechas más grandes **sin caídas**
- Mejora de **calidad** (no solo cantidad)
- Beneficio más **natural** y sostenible

### Diseño del Aparato

#### Estructura Principal (A)
- **Material:** Metal magnético (hierro blando)
- **Forma:** Hierro con U invertida
- **Función:** La forma de U crea un circuito magnético cerrado que **refuerza y concentra** las corrientes que lo atraviesan

#### Punta Sur (B)
- **Orientación:** Estrictamente hacia el sur magnético
- **Función:** Recolección magnética de corrientes S→N
- **Geometría:** Punta afilada para concentrar las fuerzas

#### Placa Dentada (C)
- **Diseño:** Metal magnético con dientes en ambos lados
- **Función lateral:** Dientes captan corrientes terrestres este-oeste
- **Cola mellada sur:** Aumenta recolección de corrientes S→N
- **Ventaja:** Superficie maximizada para contacto con corrientes direccionales

#### Puntas Melladas (D)
- **Ubicación:** Parte superior del aparato
- **Función:** Por inducción electromagnética a través de la capa de tierra, captan **pequeña cantidad de electricidad positiva** de la atmósfera
- **Balance:** La cantidad inducida es suficiente para atraer corrientes del suelo sin causar excesos

#### Nariz Norte (E) y Perno (F)
- **Función:** Conexión segura para la red distribuidora
- **Diseño:** Abertura roscada para fijación firme

#### Abrazadera (H)
- **Material:** Metal magnético, dos piezas comprimidas
- **Función:** Contacto eléctrico perfecto entre cable y aparato

#### Red Distribuidora (G)
- **Orientación:** Sur a Norte magnético
- **Profundidad:** 20-30 cm bajo la superficie
- **Función:** Distribuye la energía por toda el área cultivada

### Mecanismo Físico Completo

```
PASO 1: Magnetización por orientación
─────────────────────────────────────
Barra de hierro blando en dirección S→N
→ Se convierte en imán por corrientes terrestres
→ Adquiere polos Norte y Sur

PASO 2: Recolección de corrientes del suelo
─────────────────────────────────────────────
El cuerpo en U (A) atrae electricidad negativa del suelo
Las aletas laterales captan corrientes E↔O
La punta B concentra corrientes S→N

PASO 3: Inducción atmosférica controlada
─────────────────────────────────────────
Las puntas D, cubiertas por tierra, inducen
pequeña cantidad de electricidad positiva
→ Suficiente para atraer corrientes del suelo
→ Insuficiente para causar caídas

PASO 4: Distribución por red
────────────────────────────
Los cables G, orientados S→N, también se magnetizan
Crean campo magnético distribuido en toda el área
Electricidad positiva atrae y retiene corrientes negativas

PASO 5: Campo magnético combinado
──────────────────────────────────
Capa arable sobre campo magnético formado por:
  • Electricidad negativa del suelo
  • Electricidad positiva de la atmósfera (traída por aparato)
→ Las plantas ven aumentado su intercambio natural
→ Vitalidad multiplicada
```

### Comparación: Mastil vs Aparato Subterráneo

| Característica | Mastil Superficial | FR 764497 Subterráneo |
|---|---|---|
| **Tipo de electricidad** | Principalmente estática atmosférica | Principalmente corrientes del suelo |
| **Efecto en crecimiento** | Vigoroso (riesgo de caídas) | **Equilibrado (sin caídas)** |
| **Calidad de producto** | Variable | **Mejorada (azúcar, vitaminas)** |
| **Visibilidad** | visible (antiestético) | **Invisible** |
| **Obstrucción agrícola** | Sí | **No** |
| **Mantenimiento** | Requiere acceso | **Nulo** |
| **Vida microbiana del suelo** | Moderada | **Desarrollada** |
| **Costo inicial** | Alto (mastil + aparato) | **Menor (solo aparato)** |
| **Tipo de beneficio** | Crecimiento rápido | **Crecimiento natural y sostenible** |

### Especificaciones de Instalación

| Parámetro | Recomendación |
|---|---|
| **Profundidad del aparato** | 40-60 cm |
| **Orientación** | Sur a Norte magnético (usar brújula) |
| **Profundidad de cables** | 20-30 cm |
| **Separación entre ramas** | 1-2 metros |
| **Conexión ared** | Perno F + abrazadera H |
| **Extensión de la red** | Cubrir toda el área cultivada |

### Aplicaciones Recomendadas

- **Cereales:** Elimina riesgo de caídas por crecimiento excesivo
- **Viñedos:** Crecimiento equilibrado con mejor calidad de uva
- **Hortalizas:** Mayor tamaño sin sacrificar calidad
- **Frutales:** Aumento de producción sostenible
- **Pastos:** Mejor crecimiento sin intervención mecánica

---

## Referencias

- **Patente original:** FR 764497 (1934) — Justin Christofleau
- **Patente complementaria:** CH 172269 (misma invención, registro suizo)
- **Libro:** *Electroculture* by Justin Christofleau (1927)
- **Fuente digital:** [rexresearch.com/ElectroCulture/ChristofleauEC](https://www.rexresearch.com/ElectroCulture/ChristofleauEC/ChristofleauEC.htm)

---

*Documento actualizado con diagramas técnicos modernos y explicaciones científicas detalladas.*  
*Autor original: Justin Christofleau — Traducción y actualización para fines de investigación.*
