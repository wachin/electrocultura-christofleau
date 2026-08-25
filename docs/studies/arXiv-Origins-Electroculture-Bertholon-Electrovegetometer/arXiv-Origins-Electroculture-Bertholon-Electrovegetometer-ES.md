# En los orígenes de la electrocultura: Un modelado retrodictivo del electrovegetómetro de Bertholon del siglo XVIII en el régimen pre-corona

> **Traducción al español del paper original en inglés**
> **Fuente:** [arXiv:2505.08723](https://arxiv.org/abs/2505.08723) (mayo 2025)
> **Autor:** T. Dufour
> **Afiliación:** Laboratoire de Physique des Plasmas, Sorbonne Université, CNRS, École Polytechnique
> **Revista:** Compte-Rendus Mécanique de l'Académie des Sciences
> **DOI:** [https://doi.org/10.5802/crmeca.331](https://doi.org/10.5802/crmeca.331)

---

## Resumen

El electrovegetómetro de Bertholon (1783) fue un aparato pasivo diseñado para recolectar electricidad atmosférica y redistribuirla sobre los cultivos mediante descargas corona difusas ("aigrettes lumineuses"). Este estudio desarrolla un modelo numérico bidimensional, cuasi-estacionario y óhmico del sistema aire-aparato, en el que la atmósfera se trata como un medio resistivo que transporta la corriente de conducción global y la estructura metálica como un conductor flotante soportado por aisladores de madera con fugas. Los resultados muestran que, bajo condiciones de tiempo despejado, el aparato produce enhance locales del campo eléctrico de dos a tres órdenes de magnitud, pero las corrientes permanecen en el rango pA-nA/m². Bajo condiciones de tormenta, los campos pueden alcanzar 10⁵-10⁶ V/m, acercándose al umbral de inicio de corona, lo que haría plausible la producción de "aigrettes" luminosas reportadas históricamente.

---

## 1. Introducción

### Un impulso interdisciplinario: desde el coloquio de Montpellier hasta el presente estudio

El presente estudio se inició a raíz del coloquio francés *"Hommage à Pierre Bertholon, savant et électricien des Lumières"*, celebrado en Montpellier en octubre de 2023 bajo el patrocinio de la UNESCO. Este evento reunió a historiadores de la ciencia, físicos, especialistas en electricidad atmosférica y académicos de la filosofía natural del siglo XVIII — comunidades que rara vez interactúan aunque su combinación posee un potencial interdisciplinario insospechado y significativo.

Las discusiones con los participantes durante y después de la reunión revelaron un interés compartido en reevaluar el electrovegetómetro de Bertholon utilizando las herramientas de la moderna electrodinámica atmosférica, permaneciendo fieles a su contexto histórico y restricciones materiales.

### Encuadre histórico

En 1783, Pierre-Nicolas Bertholon de Saint-Lazare, comúnmente conocido como Abbé Bertholon, publicó *De l'électricité des végétaux*, un tratado en el que afirmaba que la "electricidad atmosférica" actúa continuamente sobre las plantas y podría aprovecharse para mejorar la germinación, el crecimiento, la floración y la fructificación.

Su propuesta práctica clave, el **electrovegetómetro** (*électro-végétomètre*), era un aparato pasivo destinado a recolectar carga de la atmósfera y redistribuirla suavemente sobre los cultivos mediante "aigrettes lumineuses": una expresión francesa histórica que puede entenderse hoy como descargas corona difusas y luminiscentes.

Aunque Bertholon interpretó el funcionamiento de su aparato mediante la noción del siglo XVIII de "fluido eléctrico", el principio físico al que apelaba puede expresarse claramente en términos electrodinámicos modernos: **los conductores puntiagudos sumergidos en un campo eléctrico ambiental pueden actuar como fuentes (o sumideros) de carga espacial**, modificando las densidades locales de iones y los débiles flujos de aire, alterando así el entorno microfísico cerca de las hojas y el suelo.

### Configuraciones del electrovegetómetro

Bertholon describió dos configuraciones estrechamente relacionadas:

**Configuración I — "Varilla de punto único, brazo articulado":**
- Un mástil de madera alto, cuidadosamente aislado del suelo con alquitrán, resinas y elementos de vidrio
- Un solo puntón de hierro en la cabeza, protegido por un embudo de hojalata para favorecer la recolección ascendente
- Una cadena suspendida que conducía el "fluido eléctrico" interceptado hacia un pequeño disco de hierro
- Un brazo metálico articulado que podía balancearse sobre hileras seleccionadas de cultivos
- Una corona de puntas finas en el extremo que liberaba carga como corona difusa justo sobre el dosel vegetal

**Configuración II — "Corona de múltiples puntos, brazo giratorio y extensible":**
- Una corona de puntas afiladas montada sobre un buje tratado con resina e aislado con vidrio
- Un brazo giratorio y telescópico que podía barrer un círculo completo
- Una corona terminal de puntos que distribuía carga suavemente sobre la vegetación

> En ambas configuraciones, el aparato era **enteramente pasivo**: no medía voltaje ni corriente e inyectaba energía externa alguna.

### De las ideas de la Ilustración a la electrodinámica atmosférica moderna

A finales del siglo XVIII, varios aspectos esenciales de la electricidad atmosférica ya eran reconocidos:

- **Stephen Gray** y **Charles François de Cisternay Du Fay** distingüeron conductores de aisladores e introdujeron la idea de dos estados eléctricos opuestos
- **Benjamin Franklin** sintetizó estas ideas, definió la convención de polaridad y argumentó que el rayo era una descarga eléctrica de la misma naturaleza que las chispas de las máquinas
- **Dalibard y Le Monnier** confirmaron en Francia que las nubes tormentosas portan carga eléctrica
- **John Canton** y **Giambattista Beccaria** demostraron mediante mediciones sistemáticas que incluso el aire sin nubes era raramente neutro

La comprensión moderna enmarca estos fenómenos en el circuito eléctrico global (GEC) de la Tierra-ionosfera. La Tierra y la ionosfera se comportan como un **capacitor esférico con fugas**: las tormentas eléctricas mantienen la ionosfera a aproximadamente +250/+300 kV respecto a la superficie, mientras que las regiones de "tiempo despejado" cierran el circuito mediante la débil conductividad eléctrica del aire.

Bajo condiciones claras y no perturbadas, la columna atmosférica transporta una pequeña corriente de conducción descendente cuasi-estacionaria descrita por la ley de Ohm:

> **J_z(z) = σ(z) · E_z(z)**

Donde σ(z) es la conductividad eléctrica y E_z(z) el campo eléctrico vertical. Cerca de la superficie, los valores típicos son E₀,atm ≈ -100 a -150 V/m y J₀,atm ≈ -1 a -3 pA/m².

### Brecha de conocimiento y preguntas de investigación

Los relatos históricos describen el electrovegetómetro de Bertholon como un aparato puramente pasivo: la corriente atmosférica de conducción ambiental se recolectaba en una punta superior afilada y se redistribuía a través de un conductor por una corona inferior de puntos, sin fuente de energía externa ni medio de regular o medir el estado eléctrico.

Lo que permanece incierto es si tal configuración pasiva podría, incluso en principio, **generar flujos de iones o carga lo suficientemente grandes como para tener significado físico** a la altura del dosel vegetal.

---

## 2. Modelo

### Supuestos físicos y alcance

El entorno electrostático alrededor del electrovegetómetro de Bertholon se modela como una atmósfera cuasi-estacionaria y óhmica que transporta la corriente de conducción del tiempo global. Las suposiciones clave son:

1. La atmósfera se comporta como un **medio lineal y resistivo** caracterizado por una conductividad prescrita σ(x, z), dominada por su dependencia con la altitud σ(z)
2. La **corriente de conducción vertical** es aproximadamente conservada en ausencia de fuentes o sumideros (∇·J = 0)
3. Las partes metálicas del aparato se tratan como **conductores perfectos**, cada región metálica conectada siendo equipotencial
4. La estructura es **eléctricamente flotante**: no se impone voltaje externo, y su potencial se ajusta de forma autoconsistente
5. El suelo se representa como un límite conductor y equipotencial
6. El problema se resuelve en geometría **bidimensional** (Cartesiana/asimétrica)

### Ecuaciones gobernantes y perfil de conductividad

El potencial eléctrico V(x, z) satisface la **ecuación de conducción estacionaria** en todos los materiales:

> **∇ · [σ(x,z) ∇V(x,z)] = 0**

El campo eléctrico y la densidad de corriente se derivan de:
> **E⃗ = -∇V**
> **J⃗ = σE⃗**

La conductividad del aire depende de la altitud según:
> **σ_air(z) = σ₀ · exp(z/H_σ)**

Donde H_σ = 6 km es la escala de altura de conductividad.

### Dominio computacional

El problema se resuelve en 2D sobre x ∈ [-0.4, 2.0] m y z ∈ [0.0, 4.0] m en una cuadrícula uniforme de Nx = 6000, Nz = 10,000 nodos (Δx = Δz = 400 µm).

El aparato tipo Bertholon se modela como:
- Un **mástil vertical de madera**, 2.0 m de alto y 0.15 m de ancho
- Un elemento horizontal corto de madera en z = 1.5 m
- Dos pies de madera, cada uno de 0.5 m de alto y 1.5 cm de grosor
- El **conductor metálico** representado por una estructura en forma de L con puntas triangulares
- En la parte superior: una punta triangular de 0.30 m de alto y 0.02 m de ancho en z = 2.2 m (ángulo de vértice de 4°)
- Un brazo horizontal de 1.50 m de largo aproximadamente a 0.5 m del suelo
- Una **corona terminal** compuesta por cinco puntas triangulares (cada una de 0.30 m de alto) con orientaciones angulares de -40°, -20°, 0°, +20° y +40°

### Condiciones de contorno e implementación numérica

Los límites superior e inferior aplican la densidad de corriente vertical impuesta J₀,atm, mientras que los límites laterales son simétricos. La ecuación gobernante se discretiza en un **esténcil de diferencias finitas de cinco puntos**. La conductividad en cada cara de celda se calcula con la media armónica entre celdas adyacentes. El sistema resultante se resuelve por **relajación Jacobi**.

### Regímenes atmosféricos ideales

| Parámetro | Tiempo despejado | Tormenta |
|-----------|-----------------|----------|
| **Campo eléctrico** | Descendente (negativo) | Ascendente (positivo) |
| **E₀,atm** | -100 a -150 V/m | +1 a +10 kV/m |
| **Potencial V(z)** | Aumenta con altitud | Disminuye con altitud |
| **V(1m)** | +100 a +150 V | -1 a -10 kV |
| **V(10m)** | +1000 a +1500 V | -10 a -100 kV |
| **Conductividad σ(0)** | (1-5) × 10⁻¹⁴ S/m | (1-10) × 10⁻¹² S/m |
| **Densidad de corriente J** | ≈ -2 pA/m² | +0.1 a +10 nA/m² |
| **Campo de ruptura** | ≈ 3.0 MV/m | 2.5-2.8 MV/m |

---

## 3. Resultados

### Condiciones de tiempo despejado ("soleado")

Aquí se examina la Configuración I del electrovegetómetro (Figura 1a), que consiste en una estructura conductora en forma de L combinando un colector de punto único en la extremidad superior con una corona de cinco puntos cerca del nivel del suelo.

#### Respuesta del colector superior de punto único

El potencial en estado estable, la magnitud del campo eléctrico y la densidad de corriente en las cercanías del colector superior de punto único muestran:

- El **potencial atmosférico** oscila entre aproximadamente 260 y 305 V sobre la extensión vertical del dominio. Cerca del punto metálico, el potencial cae bruscamente a ≈260-265 V, mientras que el aire circundante a la misma altitud se encuentra alrededor de 290-300 V
- Esta **depresión lateral de 30-40 V** está confinada a una región de solo unos pocos milímetros de ancho
- El **campo eléctrico local** excede 20 kV/m, con un valor pico de E_max = 20.9 kV/m
- Esto corresponde a un **factor de enhance de aproximadamente 175**
- El campo elevado decae rápidamente: dentro de 1 cm de la punta cae al rango de kV/m y dentro de unos pocos cm vuelve a los valores ambientales de tiempo despejado
- La **densidad de corriente** tiene un pico de J_max = 1.36 nA/m², consistente con la ley de Ohm usando la conductividad superficial de tiempo despejado σ₀ ≈ 1.7 × 10⁻¹⁴ S/m

#### Respuesta de la corona inferior de cinco puntos

La corona inferior de cinco puntos muestra:

- Cada una de las cinco puntas metálicas produce una **depresión distinta** en el campo de potencial, típicamente 20-40 V más profunda que el aire circundante
- La **magnitud del campo eléctrico** exhibe cinco lóbulos de alto campo distintos, uno por vértice. Su superposición forma un envolvente estructurado
- El campo alcanza E_max ≈ 80.9 kV/m, **casi 700 veces el campo ambiental de tiempo despejado**
- La **densidad de corriente** indica cada punto de la corona genera un estrecho chorro de corriente que se difunde hacia abajo y se fusiona con la corriente de conducción de fondo

> **Bajo forzamiento de tiempo despejado, todos los campos simulados permanecen bien por debajo de los umbrales de ruptura del aire**, confirmando la operación en un régimen óhmico lineal pre-corona.

### Condiciones de tiempo tormentoso

La respuesta bajo condiciones idealizadas de tormenta muestra resultados dramáticamente diferentes:

#### Colector superior de punto único

- El **pozo de potencial** alrededor del vértice es significativamente más profundo y comprimido que bajo tiempo despejado
- Los potenciales locales cerca del vértice del punto único caen por debajo de -12 kV, comparado con el rango de -260 V visto anteriormente
- El **campo eléctrico** alcanza un pico de E_max ≈ 735 kV/m localizado en una región sub-milimétrica
- Este valor se acerca a los rangos empíricos de inicio de corona para conductores puntiagudos bajo condiciones húmedas o pre-tormenta
- La **densidad de corriente** alcanza un pico de J_max ≈ 5.4 µA/m², un aumento de casi tres órdenes de magnitud respecto a los valores de tiempo despejado

#### Corona inferior de cinco puntos

- El **campo eléctrico** alcanza un pico de E_max ≈ 2845 kV/m, aproximadamente 40 veces mayor que el máximo del punto único bajo tormenta
- Este valor se encuentra directamente dentro del **rango empírico de ruptura** para aire húmedo a nivel del suelo
- La **densidad de corriente** alcanza J_max ≈ 5.4 µA/m², más de tres órdenes de magnitud por encima de su contraparte de tiempo despejado

> **La corona de múltiples puntos actúa como un concentrador de campo excepcionalmente eficiente** bajo condiciones de tormenta, mucho más que el colector superior de punto único.

### Influencia del ángulo de vértice

Un barrido paramétrico para diferentes valores del ángulo de vértice θ de la varilla de punto único revela:

- Bajo tiempo despejado: E_max cae de aproximadamente 20 kV/m para vértices muy afilados a 13 kV/m a 90°. La dependencia es suave y relativamente débil — la variación permanece dentro de un factor ≲1.5
- Bajo tormenta: E_max disminuye de 800 kV/m para puntas agudas a 450 kV/m para la cuña más roma
- La **corona inferior** permanece esencialmente constante a medida que θ varía — bajo tiempo despejado cerca de 80 kV/m y bajo tormenta cerca de 2700-3000 kV/m

Esto indica que la punta inferior está controlada casi enteramente por su propia geometría de vértice y por el forzamiento ambiental, con un acoplamiento insignificante a la nitidez del colector superior distante.

### Influencia de la geometría del conductor

Cuatro variantes del diseño del conductor fueron examinadas:

1. **Configuración I** — Colector de punto único y distribuidor de corona
2. **Configuración II** — El punto superior único es reemplazado por una pequeña corona de puntas afiladas
3. **Configuración I extendida** — Retiene un punto superior único pero extiende el mástil metálico aproximadamente 1 m
4. **Configuración de corona aislada** — Se elimina todo el ensamblaje mástil-brazo, dejando solo la corona de cinco puntos a la altura del dosel

Resultados clave:
- Bajo **tiempo despejado**: todas las configuraciones producen campos pico similares del orden de 10² kV/m
- Bajo **tormenta**: las tres configuraciones con mástil alcanzan campos comparables de ~2.5-3 × 10³ kV/m, mientras que la configuración de solo corona permanece significativamente menor (aproximadamente la mitad)

> **El mástil metálico elevado canaliza eficientemente** el potencial de columna mejorado por la tormenta hacia la región de la corona.

---

## 4. Discusión

### Operación en tiempo despejado: enhance localizado pero moderado

Bajo forzamiento de tiempo despejado, el electrovegetómetro reconstruido se comporta como una **perturbación débil** de la corriente de conducción global. El colector superior y la corona inferior generan enhance locales fuertes (de dos a tres órdenes de magnitud) pero estas regiones mejoradas permanecen confinadas a vecindarios de milímetros a centímetros alrededor de las puntas.

Para el microentorno de la planta, esto implica que, en condiciones de tiempo no perturbado, el dispositivo podría crear estrechos **"puntos calientes"** de campo mejorado e flujo de iones inmediatamente alrededor de cada punta, pero estas perturbaciones decaerían a valores casi ambientales sobre distancias comparables o menores que las escalas típicas de hojas y dosel.

El régimen de tiempo despejado parece compatible con la idea cualitativa de Bertholon de una influencia continua pero "suave" de la electricidad atmosférica, aunque los resultados sugieren que esta influencia es físicamente sutil.

### Forzamiento de tormenta y la plausibilidad de "aigrettes" luminosas

Bajo forzamiento tormentoso idealizado, la misma geometría opera en un régimen muy diferente. Cuando el campo de fondo y la conductividad se incrementan a valores representativos de condiciones pre-tormenta, tanto la punta superior como la corona inferior pueden alcanzar **campos eléctricos pico de varios 10⁵ V/m hasta la escala MV/m** en el modelo lineal.

Estos niveles son comparables o exceden los **umbrales empíricos de inicio de corona** para conductores puntiagudos a presión terrestre y se acercan a estimaciones convencionales de ruptura.

Es importante enfatizar que, debido a que el modelo descuida la carga espacial y la retroalimentación de ionización, estos valores de escala MV/m deben interpretarse como **límites superiores** del estado pre-corona más que como campos sostenidos realistas: en una atmósfera real, la corona se desencadenaría antes y la carga espacial resultante parcialmente apantallaría las puntas.

No obstante, el hecho de que la solución óhmica pre-corona se acerque naturalmente a los umbrales de inicio de corona bajo forzamiento GEC mejorado es significativo. Proporciona una **justificación cuantitativa** para los informes de Bertholon sobre débiles brillos luminosos ("aigrettes lumineuses") en las puntas bajo clima perturbado y para observaciones históricas de fuego de San Elmo en mástiles de barcos y agujas de iglesias.

En esta imagen, el electrovegetómetro puede actuar como un **facilitador de descargas corona** durante períodos en que la columna atmosférica ya está altamente tensada por carga de tormenta cercana. Los resultados muestran que las corrientes de tormenta pueden incrementarse en aproximadamente tres órdenes de magnitud comparado con el tiempo despejado.

### Robustez a incertidumbres geométricas y el papel del mástil

Los barridos paramétricos indican que varios aspectos de la respuesta del dispositivo son **relativamente robustos** a las incertidumbres históricas en la geometría:

- Variar el ángulo de vértice del colector superior solo altera el campo máximo y la densidad de corriente cerca de la punta por factores del orden de la unidad, no por órdenes de magnitud
- Reemplazar el punto superior único por una pequeña corona o extender el mástil modestamente apenas afecta los campos pico en la corona inferior
- **El papel principal del mástil** es interceptar una porción mejorada del potencial de columna de fondo y canalizarla hacia el distribuidor, en lugar de codificar sensiblemente los detalles del diseño del colector

Desde una perspectiva de reconstrucción histórica, esto es tranquilizador: incluso si el hardware real de Bertholon se desviaba de la geometría estilizada utilizada aquí, las **conclusiones cualitativas** sobre la operación en tiempo despejado versus tormentoso, la localización de campos y la importancia relativa del colector versus el distribuidor son poco probable que cambien drásticamente.

### Limitaciones del modelo actual

El modelo 2D, lineal y óhmico tiene varias limitaciones importantes:

1. **Conductividad prescrita y ley de Ohm lineal** — sin tratamiento explícito de producción de carga, adhesión, recombinación o deriva más allá de lo codificado en σ(z)
2. **Configuración bidimensional** — representa una estructura infinitamente larga, conduciendo a puntas de tipo cuña en lugar de conos 3D realistas
3. **Soportes de madera** modelados con conductividades fijas y bajas, y el suelo tratado implícitamente mediante condiciones de contorno
4. **Regímenes ideales** — perfiles horizontales uniformes simples con J₀,atm y E₀,atm prescritos
5. **Sin representación explícita de vegetación** — las hojas, tallos y estructura del dosel pueden distorsionar el campo

---

## 5. Conclusión

Reexaminando el electrovegetómetro de Bertholon del siglo XVIII dentro del marco de la moderna electrodinámica atmosférica, los hallazgos principales se resumen como sigue:

1. **Bajo condiciones típicas de tiempo despejado**, los puntos afilados del electrovegetómetro mejoran el campo eléctrico local de **dos a tres órdenes de magnitud** respecto al campo atmosférico de fondo, alcanzando decenas de kV/m en el punto superior único y aproximadamente 80 kV/m en la corona inferior de múltiples puntos. Las densidades de corriente asociadas permanecen en el rango pA-nA/m². Las perturbaciones de campo y corriente están fuertemente localizadas y decaen a valores casi ambientales dentro de cm.

2. **Cuando el campo de fondo y la conductividad se incrementan** a valores representativos de condiciones pre-tormenta o de tormenta, la misma geometría produce campos pico en el rango **10⁵-10⁶ V/m**. Estos niveles se acercan o exceden los umbrales empíricos de inicio de corona, particularmente en la corona inferior. Estos resultados indican que el dispositivo de Bertholon **podría haber producido resplandores de corona** y flujos de iones mejorados durante clima perturbado, proporcionando una base física plausible para informes históricos de "aigrettes" luminosas.

3. Las **variaciones paramétricas** muestran que los campos y corrientes pico en la corona inferior son en gran medida insensibles a los detalles finos del colector, siempre que esté presente un mástil elevado. La función principal del mástil es interceptar una porción del potencial de columna atmosférica y canalizarla al distribuidor, mientras que la corona de múltiples puntos cerca de la altura del dosel permanece como la característica dominante que controla el enhance del campo local.

4. Los resultados están contingentes a las suposiciones de geometría 2D, conducción óhmica lineal, perfiles de conductividad prescritos y propiedades materiales simplificadas. Deben verse como **límites superiores pre-corona** más que como predicciones completamente realistas del comportamiento de descarga.

> **En conclusión**, el estudio sugiere que el electrovegetómetro de Bertholon era físicamente capaz de **concentrar la electricidad atmosférica** y ocasionalmente producir corona visible bajo forzamiento de tormenta, mientras que su influencia de tiempo despejado sobre las plantas fue probablemente sutil, localizada y difícil de cuantificar con los instrumentos del siglo XVIII.

Este trabajo ilustra cómo el modelado numérico moderno del circuito eléctrico global atmosférico, incluso en una forma simplificada pre-corona, puede afinar nuestra comprensión de dispositivos históricos de electroingeniería y sus posibles modos de operación.

---

## Referencias

- [Aplin, 2008] K. L. Aplin, R. G. Harrison, M. J. Rycroft. "Investigating Earth's Atmospheric Electricity: a Role Model for Planetary Studies." *Space Sci Rev*, 137, 11-27.
- [Winkler et al., 1898] J. H. Winkler, B. Franklin, T. F. Dalibard, L. G. Le Monnier. *Ueber Luftelektricität*. Berlin, A. Asher & Co.
- [Bailey, 2001] A. G. Bailey. "The charging of insulator surfaces." *Journal of Electrostatics*, 51-52, 82-90.
- [Bertholon, 1783] Bertholon. *De l'électricité des végétaux*. París, P. F. Didot Jeune.
- [Guha, 2010] A. Guha et al. "First results of fair-weather atmospheric electricity measurements in Northeast India." *J. Earth Syst. Sci.*, 119, 221-228.
- [Herbert, 2012] K. B. H. Herbert. "John Canton — Pioneer investigator of atmospheric electricity." *Weather*, 52(9), 286-290.
- [Kudintseva, 2016] I. G. Kudintseva et al. "AC and DC global electric circuit properties and the height profile of atmospheric conductivity." *Annals of Geophysics*, 59(5).
- [Kundt, 1999] W. Kundt, G. Thuma. "Geoelectricity: atmospheric charging and thunderstorms." *J. Atmos. Sol.-Terr. Phys.*, 61, 955-963.
- [Mareev, 2014] E. A. Mareev, E. M. Volodin. "Variation of the global electric circuit and Ionospheric Potential in a general circulation model." *Geophys. Res. Lett.*, 41(24), 9009-9016.
- [McGinness, 2025] B. P. S. McGinness et al. "The role of point discharge in the historical development of atmospheric electricity." *Hist. Geo Space Sci.*, 16, 51-63.
- [Standler, 1979] R. B. Standler, W. P. Winn. "Effects of coronae on electric fields beneath thunderstorms." *Quart. J. Royal Meteor. Soc.*, 105, 285-302.
- [Tinsley, 2007] B. A. Tinsley et al. "The role of the global electric circuit in solar and internal forcing of clouds and climate." *Adv. Space Res.*, 40(7), 1126-1139.
- [Williams, 2009] E. R. Williams. "C.T.R. Wilson versus G.C. Simpson: Fifty years of controversy in atmospheric electricity." *Atmospheric Research*, 91, 259-271.

---

> 📄 **Paper original:** [arXiv:2505.08723](https://arxiv.org/abs/2505.08723)
> 📥 **Descargar PDF:** [arxiv.org/pdf/2505.08723](https://arxiv.org/pdf/2505.08723)
> 🔬 **DOI:** [10.5802/crmeca.331](https://doi.org/10.5802/crmeca.331)
