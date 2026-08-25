# En los orígenes de la electrocultura: Un modelado retrodictivo del electrovegetómetro de Bertholon del siglo XVIII en el régimen pre-corona

**Autor:** T. Dufour  
**Afiliación:** LPP, Sorbonne Université, CNRS, École Polytechnique, Université Paris-Sud, Observatoire de Paris, Université Paris-Saclay, PSL Research University, 4 Place Jussieu, 75252 Paris, France  
**Revista:** Compte-Rendus Mécanique de l'Académie des Sciences, Volumen 354 (2026), pp. 117-139  
**DOI:** [https://doi.org/10.5802/crmeca.346](https://doi.org/10.5802/crmeca.346)

---

## Resumen

El electrovegetómetro de Pierre-Nicolas Bertholon del siglo XVIII fue concebido para aprovechar la "electricidad atmosférica" para el crecimiento de las plantas, pero sus capacidades físicas nunca han sido cuantificadas dentro del contexto de la comprensión actual del sistema eléctrico atmosférico terrestre. Este estudio aborda la falta de evaluación cuantitativa de dicho dispositivo histórico de "electrocultura" y su plausible influencia en el entorno eléctrico cercano al dosel. Su objetivo es reinterpretar el aparato de Bertholon utilizando la electrodinámica atmosférica contemporánea, preguntándose bajo qué condiciones realistas de tiempo despejado y de tormenta un colector-distribuidor puramente pasivo podría generar campos y flujos iónicos de significación física. Se ha desarrollado un modelo óhmico cuasi-estacionario bidimensional en el que la atmósfera es una columna resistente que transporta la corriente de conducción global, la estructura metálica es un conductor flotante soportado por aislantes de madera con fugas y se excluyen la carga espacial y la corona, de modo que todos los resultados describen límites superiores pre-arranque. Las simulaciones muestran que en tiempo despejado el punto superior simple y la corona inferior de múltiples puntos del electrovegetómetro amplifican el campo de fondo entre dos y tres órdenes de magnitud, pero solo dentro de regiones milimétrico-centimétricas alrededor de las puntas y con corrientes totales limitadas al rango de pA-nA·m⁻². Bajo forzamiento de tormenta, los campos pico en la corona alcanzan 10⁵-10⁶ V·m⁻¹, acercándose o excediendo los umbrales empíricos de arranque de corona, mientras permanecen en gran medida insensibles a incertidumbres en el ángulo de vértice o la geometría del colector siempre que esté presente un mástil elevado. Estos resultados hacen que los informes de Bertholon sobre "aigrettes" luminosas sean físicamente plausibles, pero sugieren que cualquier impacto agronómico en tiempo despejado era sutil y altamente localizado y que las reclamaciones modernas de "electrocultura" requieren estudios cuidadosos y acoplados de electrostática y biología más allá del régimen pre-corona.

**Palabras clave:** Electrocultura, electrovegetómetro, agricultura plasma, Bertholon

---

# Introducción

## Un impulso interdisciplinario: desde el coloquio de Montpellier hasta el presente estudio

El presente estudio se inició como resultado del coloquio francés *«Homenaje a Pierre Bertholon, sabio y electricista de las Luces»*, celebrado en Montpellier en octubre de 2023 bajo el patrocinio de la UNESCO. Este evento reunió a historiadores de la ciencia, físicos, especialistas en electricidad atmosférica y académicos de la filosofía natural del siglo XVIII, comunidades que rara vez interactúan aunque su combinación posee un potencial interdisciplinario insospechado y significativo. Las discusiones con los participantes durante y después de la reunión revelaron un interés compartido en reevaluar el electrovegetómetro de Bertholon utilizando las herramientas de la electrodinámica atmosférica moderna, manteniendo fidelidad a su contexto histórico y restricciones materiales. El presente artículo es, por lo tanto, en parte producto de este encuentro interdisciplinario, ilustrando el valor científico de tales coloquios para tender puentes entre culturas de investigación distintas y estimular nuevas líneas de investigación a través de fronteras disciplinarias.

## Encuadre histórico

Para situar este renovado interés dentro de su contexto científico original, es necesario revisitar los fundamentos históricos del trabajo de Bertholon. En 1783, Pierre-Nicolas Bertholon de Saint-Lazare, comúnmente conocido como Abbé Bertholon, publicó *De l'électricité des végétaux*, un tratado en el que afirmaba que la "electricidad atmosférica" actúa continuamente sobre las plantas y podría aprovecharse para mejorar la germinación, el crecimiento, la floración y la fructificación [Bertholon, 1783]. Su propuesta práctica clave, el electrovegetómetro (*électro-végétomètre*), era un aparato pasivo destinado a recolectar carga de la atmósfera y redistribuirla suavemente sobre los cultivos a través de "aigrettes lumineuses": una expresión francesa histórica que puede entenderse hoy como descargas de corona luminosas tenues.

Aunque Bertholon interpretó el funcionamiento de su aparato a través de la noción del siglo XVIII de "fluido eléctrico", el principio físico al que apelaba puede expresarse claramente en términos electrodinámicos modernos: conductores afilados sumergidos en un campo eléctrico ambiental pueden actuar como fuentes (o sumideros) de carga espacial, modificando las densidades iónicas locales y los flujos de aire débiles y alterando así el entorno microfísico cerca de las hojas y el suelo. En las descripciones de Bertholon, el electrovegetómetro consistía esencialmente en un mástil vertical, aislado, que elevaba una estructura de recolección hacia el campo eléctrico atmosférico. Una ruta conductora llevaba la carga interceptada hacia abajo hasta un brazo distribuidor, que terminaba en una corona de puntos finos suspendida sobre las hileras de cultivos. Los puntos estaban destinados a liberar carga a través de descargas no disruptivas, modificando sutilmente el gradiente de potencial y el entorno de carga alrededor del dosel.

Bertholon describió dos configuraciones estrechamente relacionadas de este electrovegetómetro:

-   La Configuración I "varilla de punto único, brazo articulado" (**Figura 1a**), combinaba un colector relativamente simple con un difusor mecánicamente

> versátil. Un alto mástil de madera, cuidadosamente aislado del suelo por alquitrán, resinas y elementos de vidrio, llevaba un punto de hierro único en su cabeza, protegido por un embudo de hojalata para favorecer la recolección ascendente. Una cadena suspendida conducía el "fluido eléctrico" interceptado hasta un pequeño disco de hierro donde se esperaba que la carga recolectada se acumulara antes de ser redistribuida. Desde allí, un brazo metálico articulado, soportado horizontalmente sobre caballetes aislantes, podía balancearse sobre hileras seleccionadas de cultivos. En su extremo final, una corona de puntos finos podía liberar carga como una corona difusa justo encima del dosel. Una cadena de puesta a tierra removible permitía que todo el aparato se neutralizara cuando el aire era juzgado "sobrecargado".

-   La Configuración II "corona de múltiples puntos, brazo giratorio y extensible" (**Figura 1b**) se caracteriza por una corona de puntos afilados montada en un cubo tratado con resina, aislado con vidrio,

> para aumentar el área efectiva de recolección de *fluido eléctrico* manteniendo un alto aislamiento. Una palanca curvada y una cadena conectaban este cubo a un brazo giratorio telescópico que podía barrer un círculo completo y extenderse o retraerse para ajustar la huella tratada. Como en la Configuración I, una corona terminal de puntos estaba destinada a difundir carga suavemente sobre la vegetación.

> En ambas configuraciones, el aparato era enteramente pasivo: ni medía voltaje ni corriente e inyectaba energía externa. Dado que conceptos modernos como el potencial eléctrico, la corriente y las unidades estandarizadas aún no estaban disponibles, Bertholon razonaba cualitativamente con nociones de "más" o "menos" electricidad. Los componentes individuales de cada configuración se detallan en la Tabla 1.

> ![](./images/image1.jpeg)

> ***Figura 1. Electrovegetómetro de Bertholon, un aparato pasivo destinado a canalizar la "electricidad atmosférica" hacia los cultivos. (a) Configuración I, con un colector de varilla de punto único (E) en la cabeza del mástil y un brazo articulado que distribuía la carga a través de una corona de múltiples puntos (N). (b) Configuración II, equipada con un colector de corona de múltiples puntos (E), un brazo giratorio y extensible y una huella de tratamiento más grande que termina en un distribuidor de corona de múltiples puntos (N). Un dispositivo de neutralización (Z), mostrado en el recuadro de (b), podía proporcionar seguridad y control de encendido/apagado. Adaptado de [Bertholon, 1783].***

**Tabla 1. Comparación entre el diseño y funcionamiento del electrovegetómetro de Bertholon (Figura 1): Configuración I y Configuración II.**

| Característica | Configuración I (varilla de punto único, brazo articulado) | Configuración II (corona de múltiples puntos, brazo giratorio y extensible) |
|----------------|-------------------------------------------------------------|-----------------------------------------------------------------------------|
| **Propósito** | Captura pasiva → Conducción aislada → Difusión suave sobre cultivos (sin medición) | Igual |
| **Mástil / Base** | Mástil de madera (A-B): sección enterrada secada al fuego, alquitranada, envuelta en polvo de carbón/cemento, luego base de albañilería; parte sobre el suelo pintada/con betún | Mástil (A-B) con cilindro de cabeza saturado en resina (C) tratado con alquitrán/brea/turpentina |
| **Aislamiento superior** | Tubo de vidrio grueso relleno de mastique bituminoso (D); segundo aislante de vidrio aguas abajo (H) | Interfaz rotativa aislada mediante inserción de resina (D) y manga de vidrio/mastique (H) |
| **Colector (en la cabeza del mástil)** | Varilla de punto único (E) montada en D; protegida por un embudo de hojalata (F) | Corona de múltiples puntos (E) para maximizar la captura de carga |
| **Ruta de conducción (vertical)** | Cadena conductora (G) suspendida de E, guiada a través de H para prevenir fugas | Palanca de hierro curvada (C) que lleva la cadena (G) a la interfaz del brazo |
| **Regulación / buffer** | La cadena termina en un disco de hierro (K) que actúa como pequeño "condensador/regulador" | Sin disco separado; regulación implícita (enfoque en movilidad y alcance) |
| **Brazo horizontal** | Brazo conductor articulado (K-L-M-N) con bisagras en L y Q, soportado sobre caballetes aislantes (O, P) con cuerdas de seda tensadas | Brazo conductor telescópico (L-M) con conductor telescópico (Q), soportado sobre caballete aislante (P) |
| **Difusor terminal** | Corona de puntos metálicos afilados (N, R), que liberan corona no disruptiva | Corona de puntos metálicos afilados |
| **Movilidad / cobertura** | El brazo se balancea en bisagras (L, Q) para cubrir un sector (hilera/franja) | Rotación completa de 360°; extender/retraer para variar el alcance |
| **Neutralización** | Cadena entre K y tierra para drenar carga | Igual |
| **Seguridad** | "Excitador en forma de C" (marco de cobre/hierro con mango de vidrio + cadena de tierra arrastrándose) | Igual |

## De las ideas de la Ilustración a la electrodinámica atmosférica moderna

A finales del siglo XVIII, varios aspectos esenciales de la electricidad atmosférica ya eran reconocidos. Los experimentos de Stephen Gray y Charles François de Cisternay Du Fay ya habían distinguido conductores de aislantes e introducido la idea de dos estados eléctricos opuestos, más tarde renombrados "positivo" y "negativo" [Bailey, 2001]. Benjamin Franklin sintetizó estas ideas, definió la convención de polaridad y argumentó, sobre la base de similitudes de laboratorio y experimentos de campo, que el rayo era una descarga eléctrica de la misma naturaleza que las chispas de las máquinas [Williams, 2009]. Sus propuestas fueron confirmadas en Francia por Dalibard y Le Monnier quienes utilizaron conductores de hierro elevados y bien aislados para extraer chispas durante tormentas, confirmando así que las nubes tormentosas portan carga eléctrica [Winkler et al., 1898]. Poco después, las mediciones sistemáticas de electroscopio de John Canton en Londres y Giambattista Beccaria en Turín mostraron que incluso el aire sin nubes rara vez era neutro: descargas lentas "silenciosas", variaciones diurnas del campo y brillos luminosos como el fuego de San Elmo de los marineros revelaban que la atmósfera inferior estaba persistentemente electrificada [Herbert, 2012]. Desde un punto de vista moderno, el fuego de San Elmo se entendía como una descarga de corona de baja corriente de conductores afilados en un campo ambiental fuerte [McGinness, 2025]. Sin embargo, estos conocimientos del siglo XVIII eran locales y cualitativos. Un marco cuantitativo y global, en el que las tormentas, las regiones de tiempo despejado y la ionosfera están acopladas a través de un solo circuito eléctrico atmosférico, surgió solo a principios del siglo XX, particularmente

a través del trabajo de C. T. R. Wilson y las síntesis posteriores del "circuito eléctrico atmosférico global" [Aplin, 2008].

La electrodinámica atmosférica moderna enmarca estos fenómenos en términos del circuito eléctrico global (GEC). El sistema Tierra-ionosfera se comporta como un capacitor esférico con fugas: las tormentas y nubes electrificadas mantienen la ionosfera a aproximadamente +250/+300 kV en relación con la superficie, mientras que las regiones de "tiempo despejado" cierran el circuito a través de la débil conductividad eléctrica del aire [Tinsley, 2007], [Mareev, 2014]. En condiciones claras sin perturbaciones, la columna atmosférica transporta una pequeña corriente de conducción descendente casi estable, descrita localmente por la ley de Ohm:

$$J_z(z) = \sigma(z) E_z(z) \quad {1}$$

donde σ(z) es la conductividad eléctrica y Ez(z) el campo eléctrico vertical (tomado positivo hacia arriba). Cerca de la superficie, los valores típicos son E0,atm ≈ −100 a −150 V.m⁻¹ y J0,atm ≈ −1 a −3 pA.m⁻² [Guha, 2010]. La conductividad aumenta muchos órdenes de magnitud con la altitud (desde aproximadamente 10⁻¹⁴ S.m⁻¹ cerca del suelo hasta 10⁻⁷ S.m⁻¹ en la termosfera inferior), de modo que |𝐸~𝑧~| disminuye correspondientemente y el potencial V(z) aumenta desde 0 V en el suelo hacia el nivel ionosférico de unos pocos ×10⁵ V [Kudintseva, 2016].

Bajo condiciones perturbadas o tormentosas, esta estructura vertical simple se modifica fuertemente. La separación de carga en las nubes tormentosas produce campos cuasi-estáticos grandes en la superficie (hasta varios kV.m⁻¹), aumenta la producción de iones y altera el perfil de conductividad [Kundt, 1999]. La densidad de corriente vertical puede aumentar al rango de nA.m⁻² y se desarrollan campos fuertes y localmente variables cerca de objetos afilados, creando condiciones favorables para descargas de corona y leaders [Standler, 1979]. Estos estados perturbados forman la rama de tormenta del circuito global y son cruciales para interpretar cómo un conductor que sobresale, como el electrovegetómetro de Bertholon, podría experimentar tanto un forzamiento modesto de tiempo despejado como un forzamiento episódico y mucho más fuerte de tiempo de tormenta.

**Tabla 2. Regímenes superficiales idealizados utilizados como condiciones de contorno atmosféricas.**

| Parámetro | Condiciones de tiempo despejado | Condiciones de tormenta |
|-----------|--------------------------------|------------------------|
| **Dirección del campo eléctrico** | Descendente (negativo) | Ascendente (positivo) |
| **Campo eléctrico vertical E₀,atm** | −100 → −150 V·m⁻¹ | +1 → +10 kV·m⁻¹ |
| **Potencial eléctrico V(z)** | Aumenta con la altitud (dV/dz = −E_z > 0) | Disminuye con la altitud (dV/dz = −E_z < 0) |
| **V(1m)** | +100 V → +150 V | −1 kV → −10 kV |
| **V(10m)** | +1000 V → +1500 V | −10 kV → −100 kV |
| **Conductividad en superficie σ(0)** | (1-5) × 10⁻¹⁴ S·m⁻¹ | (1-10) × 10⁻¹² S·m⁻¹ |
| **Variación de σ con la altura (0-20 m)** | Aumenta gradualmente (≈10×) debido a la ionización por rayos cósmicos y radiactividad | Aumenta bruscamente (≈100×) cerca del suelo debido a la ionización inducida por campo y carga espacial |
| **Densidad de corriente de conducción J** | ≈ −2 pA·m⁻² (descendente, negativo) | +0,1 → +10 nA·m⁻² (ascendente, positivo) |
| **Referencia de potencial superficial V(0)** | 0 V (por convención) | 0 V (por convención) |
| **Campo eléctrico de ruptura (Ebd)** | ≈ 3,0 MV·m⁻¹ | 2,5-2,8 MV·m⁻¹ |

Debido a su altura limitada (**Figura 1**), el aparato de Bertholon solo puede interactuar con los primeros metros de la atmósfera, donde la imagen idealizada unidimensional del GEC se rompe y los procesos locales dominan. La topografía, la carga de aerosoles, la vegetación, la humedad, la conductividad superficial y la proximidad a la carga de tormenta influyen todos en el campo eléctrico local. Para un colector-distribuidor pasivo como el electrovegetómetro, esta capa cercana a la superficie controla tanto la magnitud de la corriente interceptada como la probabilidad de iniciar descargas en las puntas. Para mayor claridad, se pueden distinguir dos regímenes idealizados, como se resume en la Tabla 2:

-   Condiciones de tiempo despejado ("soleado"), que representan estados atmosféricos sin perturbaciones con campos débiles y corrientes de conducción muy pequeñas;

-   Condiciones de tiempo tormentoso, que representan períodos bajo nubes electrificadas o cerca de celdas tormentosas activas, donde los campos y las corrientes pueden aumentar por órdenes de magnitud.

## Brecha de conocimiento y preguntas de investigación

Los relatos históricos describen el electrovegetómetro de Bertholon como un aparato puramente pasivo: la corriente de conducción atmosférica ambiental

era recolectada en una punta superior afilada y redistribuida a través de un conductor por una corona inferior de puntos, sin ninguna fuente de energía externa o medio para regular o medir el estado eléctrico. Lo que sigue siendo incierto es si una configuración pasiva de este tipo podría, incluso en principio, generar flujos iónicos o de carga lo suficientemente grandes como para tener significación física a la altura del dosel. Ningún estudio anterior ha incrustado explícitamente el electrovegetómetro en el marco del circuito eléctrico atmosférico global, con campos, corrientes y perfiles de conductividad realistas de tiempo despejado y de tormenta, ni ha cuantificado hasta dónde desde las puntas su influencia en el microentorno eléctrico de los cultivos puede extenderse.

Una segunda brecha concierne la ausencia de una distinción sistemática entre los regímenes de tiempo despejado y de tormenta. La electricidad atmosférica moderna reconoce que las condiciones típicas de tiempo despejado (por ejemplo, 𝐸~0,𝑎𝑡𝑚~ ≈ −120 𝑘𝑉. 𝑚^−1^, 𝐽~0,𝑎𝑡𝑚~ ≈ −2 𝑝𝐴. 𝑚^−2^) se asocian con corrientes de conducción débiles y cuasi-estacionarias, mientras que las condiciones de tiempo de tormenta pueden soportar campos eléctricos mucho más fuertes y estructurados. Sin embargo, las discusiones historiográficas y experimentales existentes del electrovegetómetro no cuantifican cómo estos regímenes impulsarían diferencialmente una estructura metálica flotante, ni estiman los límites superiores pre-corona de los campos y corrientes alcanzables en el colector superior y la corona inferior. Esto dificulta juzgar si los informes históricos de "aigrettes" luminosas corresponden a campos que plausiblemente exceden los umbrales de arranque de corona difusa.

Finalmente, las consecuencias electrodinámicas de la incertidumbre geométrica siguen sin explorarse. Los grabados históricos restringen la arquitectura general del electrovegetómetro pero no la altura precisa del mástil, la longitud del brazo, la separación de las puntas ni los ángulos de vértice. Por lo tanto, se desconoce cuán fuertemente la corriente de columna de fondo puede concentrarse en la capa del dosel por una corona realista, sobre qué distancia sobre el suelo persisten el campo eléctrico y la densidad de corriente mejorados (por ejemplo, dentro de los primeros 0,2-0,5 m) y cuán sensibles son estas cantidades a la geometría del colector y del mástil.

El presente trabajo aborda estas brechas desarrollando un modelo simplificado de conducción bidimensional del sistema aire-dispositivo, en el que el electrovegetómetro se trata como una estructura metálica flotante polarizada por el circuito eléctrico global. Dentro de este marco óhmico pre-corona, calculamos el potencial, el campo eléctrico y la densidad de corriente alrededor de reconstrucciones idealizadas del dispositivo de Bertholon bajo forzamiento de tiempo despejado y de tormenta, para varias combinaciones plausibles de altura del mástil, longitud del brazo y separación de puntas. Las simulaciones cuantifican (i) los campos locales máximos y los factores de amplificación en colectores de punto único y de múltiples puntos, (ii) la concentración de la corriente de columna de fondo en la capa del dosel y los gradientes verticales y horizontales resultantes de |𝐸| y |𝐽| y (iii) las condiciones atmosféricas y geométricas bajo las cuales los campos calculados se acercan o exceden los criterios empíricos de arranque de corona difusa. Dado que no se modela la acumulación de carga espacial ni la retroalimentación de ionización, estos resultados deben interpretarse como límites superiores controlados pre-arranque en lugar de predicciones del comportamiento de descarga.

Estas consideraciones llevan a las siguientes preguntas de investigación:

> - Bajo forzamiento realista de tiempo despejado, qué potenciales, magnitudes de campo eléctrico y densidades de corriente se establecen alrededor del colector superior y la corona inferior y

> sobre qué escalas de longitud decaen estas perturbaciones sobre el dosel?

> ecuación {5}, donde 𝜎~0~

> = [𝐽0,atm] está determinada por el 𝐸0,atm impuesto

-   Bajo campos de fondo mejorados que representan condiciones pre-tormenta o afectadas por tormenta, ¿puede un electrovegetómetro puramente pasivo alcanzar niveles de campo eléctrico en sus puntas que se acerquen a los umbrales de arranque de corona difusa, haciendo que las "aigrettes" luminosas históricas sean físicamente plausibles?

-   ¿Cómo dependen la amplificación del campo, la concentración de corriente en la capa del dosel y la proximidad a los umbrales de arranque de corona de la altura del mástil, la longitud del brazo, la separación de puntas y el diseño del colector dentro del rango consistente con las descripciones históricas?

# Modelo

Todos los cálculos numéricos se realizaron utilizando GNU Octave (versión 10.3.0), empleando scripts personalizados para la discretización de diferencias finitas, el esquema de relajación y el post-procesamiento.

## Supuestos físicos y alcance

El entorno electrostático alrededor del electrovegetómetro de Bertholon se modela como una atmósfera cuasi-estacionaria y óhmica que transporta la corriente de conducción global del clima. Los supuestos clave son los siguientes:

campo eléctrico atmosférico superficial 𝐸~0,atm~ y la

densidad de corriente de columna correspondiente 𝐽~0,atm~. **La Figura 2a** muestra la estructura de isopotenciales resultante para valores de 𝐸~0,atm~ que van desde −0,4 𝑘𝑉. 𝑚^−1^ hasta 10 𝑘𝑉. 𝑚^−1^. Aparecen dos regímenes atmosféricos físicamente distintos en este rango y, por lo tanto, se consideran en las simulaciones:

-   Condiciones de tiempo despejado, caracterizadas por 𝐸~0,atm~ ≈

> −120𝑉. 𝑚^−1^ y 𝐽~0,atm~ ≈ −2 𝑝𝐴. 𝑚^−2^, produciendo gradientes de potencial débiles e isopotenciales suavemente curvados (lado izquierdo de la **Figura 2a**).

-   Condiciones de tiempo tormentoso, asociadas con campos eléctricos positivos mucho más fuertes, aquí representados por 𝐸~0,atm~ =

> +5𝑘𝑉. 𝑚^−1^ y 𝐽~0,atm~ = 5𝑛𝐴. 𝑚^−2^, que producen caídas de potencial pronunciadas con la altitud e isopotenciales densamente empaquetados (lado derecho de la **Figura 2a**).

-   Se adopta una altura de escala de conductividad de 𝐻~𝜎~ = 6𝑘𝑚. En una columna atmosférica verticalmente uniforme, la conservación de corriente {6} conduce entonces al perfil de campo eléctrico de la ecuación {7}. A través de la ley de Gauss, la densidad de carga espacial de diagnóstico correspondiente viene dada por la ecuación {8}.

∇⃗→ ⋅ [𝜎(𝑥, 𝑧) ∇⃗→𝑉(𝑥, 𝑧)] = 0 {2}

$$\vec{E} = -\vec{\nabla} V \quad \{3\}$$

$$\vec{J} = \sigma \vec{E} \quad \{4\}$$

-   La atmósfera se comporta como un medio lineal y resistivo caracterizado por una conductividad prescrita σ(x, z), dominada

$$\sigma_{\text{air}}(z) = \sigma_0 \exp\left(-\frac{z}{H_{\sigma}}\right) \quad \{5\}$$

> por su dependencia de altitud σ(z).

-   La corriente de conducción vertical se conserva aproximadamente

$$J_z(z) = \sigma(z) \cdot E_z(z) = J_{0,\text{atm}} \quad \{6\}$$

> (∇⃗→. →J = 0) en ausencia de fuentes o sumideros. La carga espacial ρ y la retroalimentación de ionización no se resuelven explícitamente; en cambio, su efecto neto sobre la conductividad está codificado en σ(z).

> 𝐸~𝑧~(𝑧) = −𝐸~0,𝑎𝑡𝑚~

𝑑𝐸~𝑧~

> 𝑧

exp (− ) {7}

𝐻

> 𝜎

> 𝐸~𝑧~(𝑧)

-   Las partes metálicas del dispositivo se tratan como conductores perfectos, cada región metálica conectada siendo

> 𝜌(𝑧) = 𝜀~0~ 𝑑𝑧 = −𝜀~0~

> 𝐻~𝜎~

> {8}

> equipotencial. La estructura es eléctricamente flotante: no se impone voltaje externo y su potencial se ajusta de manera autoconsistente bajo el forzamiento del circuito global impuesto.

-   El suelo se representa como un límite conductor y equipotencial. El dosel de cultivos no se resuelve explícitamente (los campos se evalúan en el aire sobre un suelo plano), por lo que las distorsiones de campo a pequeña escala

> La densidad de carga espacial 𝜌(𝑧) no se resuelve explícitamente. En cambio, σ(z) se prescribe y el solucionador permanece puramente óhmico y pre-corona. Para casos sustitutos de tipo tormentosa, se considera la misma forma aunque las magnitudes de |𝐸~0,𝑎𝑡𝑚~|, |𝐽~0,𝑎𝑡𝑚~| y 𝜎~0~ se aumentan para igualar los valores idealizados en el régimen "tipo tormenta". Las regiones

> sólidas son aire con 𝜎~air~(𝑧) dado por la ecuación {5}, soportes de madera

> por plantas individuales se descuidan.

-   El problema se resuelve en dos dimensiones [Cartesiano /

> con 𝜎~wood~

≈ 10^−15^ 𝑆. 𝑚^−1^ (fuertemente aislante pero no perfectamente)

> 7 −1

> axisimétrico] geométrico, asumiendo invarianza en la dirección perpendicular al plano.

-   Los soportes de madera se representan como conductores débiles (σwood muy baja) que pueden tener fugas de corriente pero son altamente resistivos comparados con el metal.

## Ecuaciones gobernantes y perfil de conductividad

El potencial eléctrico 𝑉(𝑥, 𝑧) satisface la ecuación de conducción estacionaria {2} en todos los materiales, mientras que el campo eléctrico y la densidad de corriente se derivan de las ecuaciones {3} y {4}. La atmósfera se describe utilizando el perfil de conductividad dependiente de la altitud de

y el conductor metálico: 𝜎~metal~ = 1 × 10 𝑆. 𝑚. Debido a esta

fuerte discrepancia de conductividad, la estructura metálica se trata como un solo conductor flotante con un potencial interno efectivamente uniforme.

## Geometría y dominio computacional

El problema se resuelve en dos dimensiones sobre 𝑥 ∈ [−0,4, 2,0] 𝑚 y 𝑧 ∈ [0,0, 4,0] 𝑚 en una cuadrícula uniforme de 𝑁~𝑥~ = 6000, 𝑁~𝑧~ = 10 000 nodos (Δx = Δz = 400 µm). Esta formulación 2D representa una estructura infinitamente larga en la dirección perpendicular al plano; los resultados son, por lo tanto, secciones transversales con profundidad unitaria.

El aparato tipo Bertholon se modela como se muestra en la **Figura 2b**. Un mástil vertical de madera, de 2,0 m de alto y 0,15 m de ancho, forma el soporte central. Un elemento horizontal corto de madera se coloca a

𝑧 = 1,5 m y dos pies de madera, cada uno de 0,5 m de alto y 1,5 cm de grosor, proporcionan soporte a nivel del suelo debajo del conductor. El conductor metálico se representa por una estructura en forma de L con puntas triangulares. En la parte superior, una punta triangular de 0,30 m de alto y 0,02 m de ancho ubicada en 𝑧 = 2,2 m sirve como el colector superior de punto único, con un ángulo de vértice de 4°. Desde la base de esta punta, un segmento metálico vertical se extiende 1,70 m hacia abajo con un grosor de

0,02 m. Este segmento se conecta a un brazo horizontal de 1,50 m de largo

posicionado aproximadamente a 0,5 m sobre el suelo. Al final de este brazo, una corona terminal compuesta por cinco puntas triangulares (cada una de 0,30 m de alto y 0,02 m en la base) se dispone con orientaciones angulares de −40°, −20°, 0°, +20° y +40° con respecto a la vertical. Esta geometría estilizada corresponde a radios de vértice agudos del orden de 1 mm.

> ![](./images/image2.jpeg)

> ***Figura 2. (a) Potencial eléctrico*** 𝑽(𝑬𝒛, 𝒛) ***en la atmósfera sobre el suelo, mostrado como contornos de colores (en kV) y líneas de isopotencial negras. El eje horizontal representa el campo eléctrico vertical impuesto*** 𝑬𝒛***, que va desde valores de tiempo despejado (***𝑬𝒛 < 𝟎***) hasta valores de tiempo de tormenta (***𝑬𝒛 > 𝟎***). Las dos líneas verticales blancas corresponden a las condiciones atmosféricas de tiempo despejado y tormentoso de este estudio. (b) Modelo geométrico del electrovegetómetro de Bertholon implementado en la configuración I, que incluye el mástil aislante de madera y los soportes (marrón), la estructura conductora en forma de L (rojo) y la corona de múltiples puntos. El dominio computacional representa una sección transversal vertical de 2 m × 4 m de la atmósfera circundante.***

## Condiciones de contorno e implementación numérica

> implementación

Los límites superior e inferior aplican la densidad de corriente vertical impuesta 𝐽~0,𝑎𝑡𝑚~ siguiendo las ecuaciones {9} y {10} mientras que los límites laterales son simétricos, como se expresa en la ecuación {11}.

La ecuación gobernante {2} se discretiza en un esquema de

diferencias finitas de cinco puntos bidimensional. Para asegurar la continuidad de la densidad de corriente a través de cambios abruptos de conductividad, la conductividad en cada cara de celda se calcula con la ecuación {12} que proporciona la media armónica entre celdas adyacentes. Este esquema de promediado preserva la conservación de flujo y la

𝜕𝑉

|

𝜕𝑧

𝑧=0

> = − 𝐽0,𝑎𝑡𝑚 {9}

> 𝜎(0)

> estabilidad en regiones donde materiales de conductividades muy diferentes se encuentran (por ejemplo, interfaces aire/madera o aire/metal). El

> sistema discreto resultante se resuelve por relajación de Jacobi, en el que el

[𝜕𝑉]

|

𝜕𝑧

𝑧=𝐻

> [𝐽0,𝑎𝑡𝑚]

> = − 𝜎(𝐻)

{10}

> potencial en el nodo (𝑖, 𝑗) se actualiza iterativamente según la ecuación

> {13} con actualizaciones de contorno y aplicación de calibre después de cada

𝜕𝑉

|

𝜕𝑥

izquierda/derecha

= 0 {11}

> barrido.

> [2𝜎~1~𝜎~2~]

> 𝜎 =

> {12}

Un nodo de aire se fija en 𝑉 = 0 para establecer el potencial de referencia. Esta elección aplica la corriente de columna pero no impone una Tierra perfectamente equipotencial en z = 0; los potenciales cercanos al suelo pueden

> (𝑛+1)

𝑉

> 𝑖,𝑗

> cara

𝜎~1~ + 𝜎~2~ + 𝜀

por lo tanto variar horizontalmente, una aproximación aceptable aquí pero no exacta.

> 𝜎𝑒𝑉𝑖,𝑗+1 + 𝜎𝑤𝑉𝑖,𝑗−1 + 𝜎𝑛𝑉𝑖+1,𝑗 + 𝜎𝑠𝑉𝑖−1,𝑗

> = 𝜎 + 𝜎 + 𝜎 + 𝜎

𝑒 𝑤 𝑛 𝑠

{13}

La inicialización utiliza el perfil analítico de tiempo despejado en la ecuación {14} y las regiones metálicas se siembran con el potencial promedio de las celdas de aire vecinas. Las iteraciones se detienen una vez que se satisface la ecuación {15} o cuando se alcanzan 2000 iteraciones. Este criterio produce una buena concordancia con la columna analítica 1D y la conservación de corriente (el flujo superior vs inferior difiere en <0,01%), pero los campos pico siguen siendo algo sensibles a la resolución de la cuadrícula y la geometría de las puntas. Deben interpretarse como valores pre-corona aproximados en lugar de cantidades completamente convergidas. Las iteraciones continúan hasta que el cambio máximo en V entre dos pasos sucesivos cae por debajo de una tolerancia prescrita, asegurando la convergencia del campo de potencial electrostático.

# Resultados

## Condiciones de tiempo despejado ("soleado")

Aquí examinamos la Configuración I del electrovegetómetro (**Figura 1a**), que consiste en una estructura conductora en forma de L que combina un colector de punto único en la extremidad superior con una corona de cinco puntos cerca del nivel del suelo. La respuesta de esta geometría se evalúa bajo forzamiento de tiempo despejado, caracterizado por una corriente de conducción descendente impuesta 𝐽~0,𝑎𝑡𝑚~ ≈ −2 𝑝𝐴. 𝑚^−2^ y un campo eléctrico de fondo 𝐸~0,𝑎𝑡𝑚~ ≈ −120𝑉. 𝑚^−1^ aplicado en el límite inferior.

𝑉(0)

(𝑧) = 𝐸~0,atm~𝐻~𝜎~ (1 − 𝑒

> [𝑧]

> 𝐻𝜎) {14}

−

> El potencial en estado estacionario, la magnitud del campo eléctrico y la magnitud de la densidad de corriente en las cercanías del colector superior de punto único

> Max|𝑉^(𝑛+1)^ − 𝑉^(𝑛)^| < 10^−3^ {15}

El campo eléctrico y la densidad de corriente se calculan después de la convergencia utilizando diferencias finitas centradas. Los componentes horizontal y vertical del campo eléctrico se derivan directamente de los gradientes de potencial (Ecuaciones {16}-{17}) y la magnitud del campo se obtiene de la ecuación {18}. Los componentes de la densidad de corriente se derivan entonces de la ley de Ohm (Ecuaciones {19}-{20}) usando la conductividad local y la magnitud total de la densidad de corriente se calcula a partir de la Ecuación {21}. Estas cantidades se visualizan en unidades de kV.m⁻¹ para el campo eléctrico y pA.m⁻² o nA.m⁻² para la densidad de corriente, con regiones sólidas enmascaradas.

> 𝐸 = − 𝜕𝑉 {16}

> ^𝑥^ 𝜕𝑥

se muestran en la **Figura 3**. La **Figura 3a** ilustra que el potencial atmosférico varía desde aproximadamente 260 hasta 305 V sobre la extensión vertical del dominio. Cerca del punto metálico, el potencial cae bruscamente a ≈260-265 V, mientras que el aire circundante a la misma altitud se encuentra alrededor de 290-300 V. Esta depresión lateral de 30-40 V está firmemente confinada a una región de solo unos pocos mm de ancho, formando un embudo de potencial estrecho alineado con la geometría cónica de la varilla. Dado que el conductor es eléctricamente flotante, su potencial (≈240 V en la base del punto) surge de manera autoconsistente como el valor requerido para satisfacer la corriente de columna impuesta. Fuera de la región inmediata de la punta, los contornos de isopotencial relajan de nuevo hacia su espaciado casi uniforme de tiempo despejado.

La **Figura 3b** revela la amplificación resultante del campo eléctrico. El gradiente asociado con la caída de 30-40 V sobre distancias sub-centimétricas produce campos locales que exceden 20 𝑘𝑉. 𝑚^−1^ con la simulación

𝐸~𝑧~

> 𝜕𝑉

> = − 𝜕𝑧

{17}

> dando un valor pico de 𝐸~max~ = 20,9 𝑘𝑉. 𝑚^−1^. Esto corresponde a un factor de amplificación de aproximadamente:

> |𝐸| = √𝐸^2^ + 𝐸^2^ {18}

𝐸max

2,1 × 10^4^

> 𝑥 𝑧

> 𝜕𝑉

𝐽 = −𝜎.

{19}

|𝐸0,𝑎𝑡𝑚|

≈ 1,2 × 10^2^ ∼ 175

> ^𝑥^ 𝜕𝑥

> 𝜕𝑉

> 𝐽~𝑧~ = −𝜎. 𝜕𝑧 {20}

𝑥 𝑧

> |𝐽| = √𝐽^2^ + 𝐽^2^ {21}

> Este valor se debe puramente a la concentración geométrica en el vértice.

> El campo elevado decae rápidamente: dentro de 1 cm de la punta cae al rango de kV/m y dentro de unos pocos cm regresa a los valores ambientales de tiempo despejado.

> La **Figura 3c** muestra la magnitud de la densidad de corriente asociada. Las corrientes más fuertes están confinadas en un estrecho chorro axial que emerge de la varilla de punto único, con un pico de 𝐽~max~ = 1,36 𝑛𝐴. 𝑚^−2^. Este valor es consistente con la ley de Ohm 𝐽 = 𝜎𝐸, usando la conductividad superficial de tiempo despejado local 𝜎~0~ ≈ 1,7 × 10^−14^ 𝑆. 𝑚^−1^. Aunque pequeña en términos absolutos, una corriente de este tipo corresponde a un flujo microscópico de:

> 𝑁̇ ≈ [𝐽max] ≈ 8 × 10^9^ cargas.s^−1^.pm^−2^,

𝑒

> mostrando que incluso las corrientes de nanoamperio involucran miles de millones de portadores de carga por segundo. Como se espera en el régimen óhmico pre-corona, el patrón espacial de |𝐽| refleja el de |𝐸| y se fusiona suavemente con la corriente atmosférica de fondo 𝐽~0,𝑎𝑡𝑚~ ≈ −2 𝑝𝐴. 𝑚^−2^ sobre escalas de cm.

> ![](./images/image3.jpeg)

> ***Figura 3. Respuesta pre-corona del colector superior de varilla de punto único (ángulo de vértice*** θ ***= 4°) bajo forzamiento de tiempo despejado (***𝑬𝟎,𝒂𝒕𝒎 ≈ −𝟏𝟐𝟎𝑽. 𝒎^−𝟏^***,*** 𝑱𝟎,𝒂𝒕𝒎 ≈

> −𝟐𝒑𝑨. 𝒎^−𝟐^***). (a) Potencial V*** 𝒔***mostrando fuerte compresión de isopotenciales cerca del vértice metálico flotante. (b) Magnitud del campo eléctrico*** |𝑬|***con amplificación geométrica hasta*** 𝑬𝒎𝒂𝒙 = 𝟐𝟎. 𝟗 𝒌𝑽. 𝒎^−𝟏^***. (c) Magnitud de la densidad de corriente*** |𝑱| ***con pico en*** 𝑱𝒎𝒂𝒙 = 𝟏. 𝟑𝟔 𝒏𝑨. 𝒎^−𝟐^ ***y relajándose al fondo dentro de centímetros.***

![](./images/image4.jpeg)

> ***Figura 4. Respuesta pre-corona de la corona inferior de cinco puntos bajo forzamiento de tiempo despejado (***𝑬𝟎,𝒂𝒕𝒎 ≈ −𝟏𝟐𝟎𝑽. 𝒎^−𝟏^***,*** 𝑱𝟎,𝒂𝒕𝒎 ≈ −𝟐𝒑𝑨. 𝒎^−𝟐^***) con ángulo de vértice*** θ

> ***= 4°. (a,b) Potencial V mostrando depresiones locales alrededor de cada vértice y un embudo de potencial estrecho y profundo en la punta central. (c,d) Magnitud del campo eléctrico***

> |𝑬| ***formando cinco lóbulos de alto campo interactuantes, con un máximo localizado*** 𝑬𝒎𝒂𝒙 = 𝟖𝟎. 𝟗 𝒌𝑽. 𝒎^−𝟏^***. (e,f) Magnitud de la densidad de corriente*** |𝑱| ***revelando cinco canales de conducción enfocados y un pico*** 𝑱𝒎𝒂𝒙 = 𝟏. 𝟑𝟒 𝒏𝑨. 𝒎^−𝟐^***. Todos los valores permanecen dentro del régimen lineal dominado por conducción.***

El potencial en estado estacionario, la magnitud del campo eléctrico y la magnitud de la densidad de corriente que rodean la corona inferior de múltiples puntos se representan en la **Figura 4**. A la escala de toda la corona (**Figura 4a**), cada uno de los cinco puntos metálicos produce una depresión distinta en el campo de potencial. Estos "embudos" locales, típicamente 20-40 V más profundos que el aire circundante a la misma altura, se fusionan en una perturbación más amplia a unos pocos cm de la corona. El zoom cerca del punto central (**Figura 4b**) muestra un canal de potencial estrecho y verticalmente alargado cuyo mínimo se encuentra alrededor de 250-260 V, correspondiendo a una caída de potencial lateral de 30-40 V sobre escalas de mm-

a cm. Esto resulta tanto de la fuerte curvatura del vértice central como del confinamiento lateral impuesto por los puntos vecinos de la corona.

La magnitud del campo eléctrico (**Figura 4c** y especialmente 4d) exhibe cinco lóbulos de alto campo distintos, uno por vértice. Su superposición forma un envoltorio estructurado en lugar de máximos aislados, reflejando fuertes interacciones inter-puntos. Dentro del zoom central (**Figura 4d**) el campo alcanza 𝐸~𝑚𝑎𝑥~ ≈ 80,9 𝑘𝑉. 𝑚^−1^, casi 700 veces el campo ambiental de tiempo despejado. Este campo cae a unos pocos kV/m dentro de aproximadamente 1 cm, regresando a valores cercanos al ambiente dentro de

varios cm. La amplificación permanece al menos un orden de magnitud por debajo de los umbrales típicos de arranque de corona para conductores afilados a presión de suelo, confirmando la operación en el régimen pre-corona, óhmico.

Los mapas de densidad de corriente (**Figuras 4e** y **4f**) indican la estructura del campo eléctrico. Cada punto de la corona genera un estrecho chorro de corriente que se difunde hacia abajo y se fusiona con la corriente de conducción de fondo. El vértice central nuevamente produce el valor más alto, 𝐽~max~ ≈ 1,34 𝑛𝐴. 𝑚^−2^ que corresponde a un flujo microscópico similar al estimado en el colector de varilla de punto único, *es decir* 𝑁̇ ≈ 8 × 10^9^𝑐ℎ𝑎𝑟𝑔𝑒𝑠. 𝑠^−1^. 𝑚^−2^. Dado que la conductividad varía solo débilmente dentro de la región de 5-15 cm que rodea la corona, la estructura de |𝐽| está gobernada casi enteramente por el modelado geométrico del campo en lugar de la estratificación atmosférica.

Bajo forzamiento de tiempo despejado, todos los campos simulados permanecen bien por debajo de los umbrales de ruptura del aire, confirmando la operación en un régimen lineal, óhmico pre-corona. La amplificación del campo surge únicamente de la concentración geométrica en los puntos metálicos, produciendo patrones suaves y monótonos de campo eléctrico y densidad de corriente consistentes con 𝐽 = 𝜎𝐸. Estos resultados definen una línea de base cuantitativa para potenciales, factores de amplificación y chorros de conducción, contra los cuales se puede comparar un forzamiento más fuerte. Ahora examinamos cómo responde la geometría bajo condiciones idealizadas de tormenta, donde los campos ambientales aumentan dramáticamente.

## Condiciones de tiempo tormentoso

La respuesta de la varilla superior de punto único se estudia bajo un forzamiento idealizado de tipo tormenta, usando los parámetros de la Tabla 2. El campo eléctrico de fondo se aumenta a 𝐸~0,atm~ ≈ 5000 𝑉. 𝑚^−1^ y la corriente de conducción impuesta invierte dirección, alcanzando

𝐽~0,𝑎𝑡𝑚~ ≈ +5 𝑛𝐴. 𝑚^−2^. Esta configuración proporciona un sustituto lineal para campos mejorados por tormenta sin modelar explícitamente la carga de nubes, la carga espacial o la estructura electrostática tridimensional de las nubes tormentosas. Como consecuencia, los campos obtenidos cerca de las puntas representan límites superiores sobre el estado pre-corona; una atmósfera real transicionaría a una corona dominada por carga espacial antes de que se mantengan tales campos.

La **Figura 5** muestra el potencial en estado estacionario, la magnitud del campo eléctrico y la magnitud de la densidad de corriente alrededor de la punta superior para este escenario de tipo tormenta. El pozo de potencial alrededor del vértice (**Figura 5a**) es significativamente más profundo y comprimido que bajo tiempo despejado, reflejando tanto el forzamiento más fuerte como la corriente ascendente más alta. El potencial local cerca del vértice de la punta única cae por debajo de −12 𝑘𝑉, comparado con el rango de −260 𝑉 visto anteriormente, indicando una intensificación de un orden de magnitud de los gradientes. El campo eléctrico resultante (**Figura 5b**) alcanza un pico de 𝐸~𝑚𝑎𝑥~ ≈ 735 𝑘𝑉. 𝑚^−1^ localizado en una región sub-centimétrica. Este valor aún está por debajo de las estimaciones canónicas de ruptura para aire a presión de suelo (∼ 2,5 − 2,8 𝑀𝑉. 𝑚^−1^) pero cae dentro del rango inferior de mediciones empíricas de arranque de corona para conductores afilados en condiciones húmedas o pre-tormenta. Dentro de 1 cm del vértice, el campo cae a unos pocos cientos de kV/m y regresa a valores de fondo dentro de unos pocos cm, preservando el patrón de amplificación fuertemente localizado observado en tiempo despejado.

La magnitud de la densidad de corriente correspondiente (**Figura 5c**) tiene un pico en

𝐽~𝑚𝑎𝑥~ ≈ 5,4 µ𝐴. 𝑚^−2^ consistente con el escalado 𝐽 = 𝜎𝐸, dada la conductividad elevada a la altitud de la punta. Esto representa un aumento de casi tres órdenes de magnitud en relación con los valores de tiempo despejado (∼ 1,36 𝑛𝐴. 𝑚^−2^), sin embargo la estructura espacial permanece como un estrecho chorro axial que se difunde suavemente hacia la corriente ascendente de fondo.

A pesar de los grandes campos y corrientes absolutos, la solución calculada retiene la firma cualitativa de un régimen de conducción lineal: las superficies equipotenciales continúan convergiendo monótonamente, |𝐸| aumenta suavemente hacia el vértice y no se forma bloqueo de campo ni meseta. Este comportamiento indica que, dentro de las limitaciones de un modelo sin carga espacial, el sistema permanece matemáticamente óhmico incluso en intensidades donde una atmósfera real ya habría iniciado la corona. Los resultados deben, por lo tanto, interpretarse como un estado pre-corona cercano al umbral, con el inicio físico de la descarga inferido de criterios externos, no de desviaciones dentro de los campos simulados.

La respuesta del distribuidor de corona de cinco puntos bajo forzamiento de tipo tormenta se muestra en la **Figura 6**. Comparado con el caso de tiempo despejado, el campo de fondo más fuerte y la corriente de conducción invertida producen un pozo de potencial marcadamente más profundo y confinado alrededor de cada vértice. A la escala de toda la corona (**Figura 6a**), las superficies equipotenciales colapsan firmemente alrededor de los cinco puntos metálicos, con potenciales locales en la región de zoom (**Figura 6b**) cayendo alrededor de −10 𝑘𝑉. Como en la varilla de punto único anterior, estos mínimos forman canales estrechos y verticalmente alargados, pero el confinamiento lateral impuesto por los picos vecinos afila los gradientes aún más.

La magnitud del campo eléctrico correspondiente (**Figuras 6c-6d**) muestra un conjunto de 5 lóbulos de alto campo. Su superposición produce un envoltorio estructurado de campo amplificado, con el pico central alcanzando 𝐸~max~ ≈ 2845 𝑘𝑉. 𝑚^−1^. Este valor es aproximadamente 40 veces mayor que el máximo de la varilla de punto único tipo tormenta y se encuentra directamente dentro del rango empírico de ruptura para aire húmedo a nivel del suelo. También excede las estimaciones típicas de arranque de corona difusa para conductores afilados. Debido a que el modelo es estrictamente lineal y excluye procesos de carga espacial o ionización, estos campos simulados deben interpretarse como límites superiores del estado pre-descarga; una atmósfera real comenzaría la formación de corona y el bloqueo de campo antes de que se mantuvieran tales valores. Espacialmente, la amplificación permanece confinada en una región sub-centimétrica alrededor del vértice, decayendo al rango de cientos de kV/m dentro de ~1 cm y a niveles de fondo dentro de unos pocos cm.

Los mapas de densidad de corriente (**Figuras 6e-6f**) reproducen esta estructura. Un chorro axial nitidamente enfocado emerge de cada punto, con el central produciendo 𝐽~max~ ≈ 5,4 µ𝐴. 𝑚^−2^, más de tres órdenes de magnitud por encima de su homólogo de tiempo despejado y consistente con el 𝐸~max~ elevado a través de 𝐽 = 𝜎𝐸. Aunque extremadamente grandes para un modelo de solo conducción, el patrón espacial permanece suave y monótono, sin el bloqueo de campo o las características no lineales que acompañarían al inicio real de la corona.

En conjunto, estos resultados muestran que la corona de múltiples puntos actúa como un concentrador de campo excepcionalmente eficiente bajo forzamiento de tipo tormenta,

mucho más que el colector superior de punto único. Sin embargo, porque el modelo descuida la carga espacial, la ionización y la física de descarga, los picos predichos en escala MV/m representan límites superiores idealizados en lugar de valores operativos realistas; en

la práctica, la corona, la actividad de streamers y la regulación de carga asociada intervenirían bien antes de que se pudieran alcanzar los campos simulados.

> ![](./images/image5.jpeg)

> ***Figura 5. Respuesta del colector de varilla de punto único bajo forzamiento idealizado de tipo tormenta (***𝑬𝟎,𝒂𝒕𝒎 ≈ 𝟓 𝒌𝑽. 𝒎^−𝟏^***,*** 𝑱𝟎,𝒂𝒕𝒎 ≈ 𝟓 𝒏𝑨. 𝒎^−𝟐^***). (a) Potencial V mostrando profunda compresión de isopotenciales cerca del vértice metálico flotante. (b) Magnitud del campo eléctrico*** |𝑬| ***alcanzando*** 𝑬𝒎𝒂𝒙 = 𝟕𝟑𝟓 𝒌𝑽. 𝒎^−𝟏^***, acercándose a rangos empíricos de arranque de corona. (c) Magnitud de la densidad de corriente*** |𝑱| ***con pico en*** 𝑱𝒎𝒂𝒙 = 𝟓. 𝟒 µ𝑨. 𝒎^−𝟐^***. Los valores representan límites superiores pre-corona dentro del modelo lineal sin carga espacial.***

![](./images/image6.jpeg)

> ***Figura 6. Respuesta de la corona inferior de cinco puntos bajo forzamiento idealizado de tipo tormenta (***𝑬𝟎,𝒂𝒕𝒎 ≈ 𝟓 𝒌𝑽. 𝒎^−𝟏^***,*** 𝑱𝟎,𝒂𝒕𝒎 ≈ 𝟓 𝒏𝑨. 𝒎^−𝟐^***) con ángulo de vértice*** θ ***= 4°. (a,b) Potencial V mostrando un pozo colapsado profundamente y fuerte confinamiento de isopotenciales alrededor de cada vértice. (c,d) Magnitud del campo eléctrico*** |𝑬| ***con un máximo localizado*** 𝑬𝒎𝒂𝒙 = 𝟐. 𝟖𝟒 𝑴𝑽. 𝒎^−𝟏^***, acercándose a rangos empíricos de ruptura. (e,f) Magnitud de la densidad de corriente*** |𝑱| ***con pico en*** 𝑱𝒎𝒂𝒙 = 𝟐. 𝟖 µ𝑨. 𝒎^−𝟐^***. Estos valores representan campos superiores, pre-descarga dentro del modelo lineal sin carga espacial.***

## Influencia del ángulo de vértice

Para evaluar la sensibilidad de la respuesta del electrovegetómetro a laafilado del colector superior de Bertholon, se realiz un barrido paramétrico para diferentes valores del ángulo de vértice θ de la varilla de punto único, manteniendo todos los demás parámetros geométricos y atmosféricos sin cambios. El ángulo θ se define aquí como el ángulo de apertura completo de la punta triangular en la configuración 2D (**Figura 2b**). Se exploraron valores desde 2° hasta 90° (cuña roma de ángulo recto). Para cada θ, se extrajo la magnitud máxima del campo eléctrico (Emax) del aire adyacente a la punta superior y a la corona inferior. Además, la densidad de corriente de conducción máxima (Jmax) también se extrajo en esas mismas regiones. Los resultados se resumen en la **Figura 7**.

La **Figura 7a** muestra que el campo pico cerca de la varilla de punto único disminuye monotónicamente a medida que la punta se rompe. Bajo forzamiento de tiempo despejado (triángulos rojos), Emax cae desde aproximadamente 20 kV/m para vértices muy afilados hasta 13 kV/m a 90°. La dependencia es suave y relativamente débil: en todo el rango de 0-90°, la variación permanece dentro de un factor ≲1,5. La misma tendencia se mantiene bajo forzamiento de tipo tormenta (triángulos azules), con Emax disminuyendo desde 800 kV/m para puntas agudas hasta 450 kV/m para la cuña más roma. Por lo tanto, afilar

el vértice amplifica el campo local, pero solo al nivel de decenas de porcentaje para ángulos realistas. Esta suave sensibilidad angular se espera en una configuración de conductor flotante dominada por el forzamiento de columna a gran escala: cambiar θ modifica la curvatura local, por lo tanto el factor de amplificación geométrica, pero el potencial general del metal se ajusta de manera autoconsistente para satisfacer la corriente de conducción atmosférica impuesta. En otras palabras, la filo de la punta controla cómo una caída de potencial casi fija se concentra en gradientes de mm-cm, en lugar de cambiar el voltaje global disponible para la estructura.

Para comparación, la **Figura 7a** también informa el campo máximo en la corona de cinco puntos (estrellas). En ambos regímenes atmosféricos, el campo pico de la corona permanece esencialmente constante a medida que θ varía. En tiempo despejado, se mantiene cerca de 80 kV/m y bajo forzamiento de tipo tormenta cerca de 2700-3000 kV/m. Esta insensibilidad indica que la corona inferior está controlada casi enteramente por su propia geometría de vértice y por el forzamiento ambiental, con solo un acoplamiento despreciable a la filo del colector superior distante. Prácticamente, esto significa que las incertidumbres en la fabricación histórica de la punta superior no se propagan a la amplificación de campo cercana al dosel producida por la corona terminal.

> ![](./images/image7.png)

> ***Figura 7. (a) Campo eléctrico máximo*** 𝑬𝒎𝒂𝒙 ***y (b) densidad de corriente*** 𝑱𝒎𝒂𝒙 ***como funciones del ángulo de vértice para el colector superior, bajo forzamiento de tiempo despejado (rojo) y de tipo tormenta (azul). Los valores de tiempo despejado muestran débil dependencia de la geometría de la punta, mientras que las condiciones de tipo tormenta producen fuerte amplificación geométrica. La corona inferior alcanza los campos más altos (***𝟐. 𝟖 𝑴𝑽. 𝒎^−𝟏^***) y corrientes (***𝟓 𝒎𝑨. 𝒎^−𝟐^***), representando estimaciones superiores pre-descarga en el modelo óhmico lineal.***

Los máximos correspondientes de densidad de corriente de conducción se muestran en la **Figura 7b**. Como predice la relación óhmica, Jmax cerca de la punta superior sigue la misma disminución monótona con θ que Emax. En tiempo despejado (triángulos rojos), la densidad de corriente pico disminuye suavemente (nuevamente por menos de un factor de dos) entre puntas afiladas y romas. En condiciones de tipo tormenta (triángulos azules) ocurre la misma reducción, pero a valores que son tres órdenes de magnitud más altos

que en tiempo despejado, reflejando el aumento impuesto tanto en el campo de fondo como en la conductividad. En cuanto al campo eléctrico, los máximos de corriente de la corona (estrellas) son esencialmente planos con θ, confirmando que el comportamiento del distribuidor inferior está desacoplado de la filo del colector en este régimen pre-corona.

Una característica adicional de la **Figura 7b** es que, bajo forzamiento de tipo tormenta, la punta superior exhibe un Jmax más grande que la corona aunque la corona alcanza un Emax más alto. Esta reversión surge de la estratificación de conductividad: el colector superior opera a mayor altitud donde σ(z) es mayor, por lo que un campo dado produce una corriente de conducción proporcionalmente más grande. En contraste, el campo más fuerte de la corona se encuentra en una capa de menor σ y, por lo tanto, lleva una densidad de corriente óhmica más pequeña a pesar de su mayor amplificación geométrica.

En conjunto, el barrido del ángulo de vértice muestra que las predicciones pre-corona para el colector superior son robustas a incertidumbres plausibles en la filo de la punta. Si la punta metálica del siglo XVIII era afilada como una aguja o moderadamente roma, cambia Emax y Jmax solo por un factor modesto, no por órdenes de magnitud. Por lo tanto, las conclusiones cualitativas extraídas de la geometría base de θ

≈ 4° (a saber, que la operación de tiempo despejado permanece seguramente sub-coronal mientras que el forzamiento de tiempo de tormenta puede empujar la punta hacia rangos de arranque) no dependen críticamente de una reconstrucción exacta de la forma de la punta. La fuerte amplificación producida por la corona de múltiples puntos, por otro lado, está gobernada por la propia filo y espaciado de la corona y es efectivamente independiente del ángulo del colector. Finalmente, debe recordarse que estas tendencias angulares se obtienen en una aproximación de cuña 2D. Una punta cónica completamente 3D produciría diferentes factores de amplificación absolutos, pero se espera que la sensibilidad monótona y débil a θ persista, ya que refleja el ajuste de potencial flotante y la localización de la caída de potencial en lugar de cualquier particularidad de la geometría 2D.

## Influencia de la geometría del conductor

La Configuración I del electrovegetómetro parece efectiva bajo condiciones de tiempo de tormento pero esencialmente inactiva en tiempo despejado. Para explorar si geometrías alternativas podrían mejorar su respuesta de tiempo despejado, se examinaron cuatro variantes del diseño del conductor:

-   La configuración I con colector de varilla de punto único y distribuidor de corona

-   La configuración II: el punto superior único se reemplaza por una pequeña corona de puntas afiladas montada en la cabeza del mástil, mientras que el distribuidor inferior permanece sin cambios.

-   La configuración I extendida: retiene un punto superior único pero extiende el mástil metálico aproximadamente 1 m, de modo que la punta ahora sobresale más alto en la columna atmosférica. La corona inferior y los soportes permanecen sin cambios. Esta

> configuración no corresponde a un dibujo histórico específico pero sirve para probar la sensibilidad del dispositivo a la altura del colector y a los cambios asociados en el potencial y la conductividad de fondo.

-   La configuración de corona aislada: se retira todo el ensamblaje metálico de mástil-brazo para dejar solo la corona de cinco puntos a la altura del dosel. Esta configuración "mínima" proporciona un caso de control en el que la corona interactúa directamente con el campo ambiental sin ninguna guía o concentración por un conductor elevado.

Para las cuatro configuraciones, los valores máximos del campo eléctrico obtenidos en la corona inferior se presentan en la **Figura 8a** bajo forzamiento de tiempo despejado y de tipo tormenta. En tiempo despejado, todas las configuraciones producen campos pico casi idénticos del orden de 10^2^ kV.m^−1^, indicando que la geometría local de la corona domina la amplificación del campo y que la presencia, forma o altura del colector superior tiene solo una influencia menor en el régimen de campo débil. Bajo forzamiento de tipo tormenta, sin embargo, las tres configuraciones con mástil (I, II e I extendida) alcanzan todos campos pico comparables de aproximadamente 2,5-3 × 10^3^ kV.m^−1^, mientras que la configuración de solo corona permanece significativamente más baja (aproximadamente la mitad de ese valor). Este contraste muestra que el mástil metálico elevado canaliza eficientemente el potencial de columna mejorado por tormenta hacia la región de la corona, pero que reemplazar un colector de punto único por un colector de múltiples puntos o extender modestamente su altura no cambia materialmente el campo máximo local en el distribuidor.

Los máximos correspondientes de densidad de corriente de conducción, 𝐽~max~, se muestran en la **Figura 8c** en una escala logarítmica. En condiciones de tiempo despejado, las cuatro configuraciones se agrupan alrededor de 𝐽~max~ ≈ 10^−3^ 𝜇A.m^−2^, confirmando que las corrientes débiles y sub-coronas están esencialmente determinadas por la corriente de conducción atmosférica ambiental y por la geometría de la corona. Cuando se aplica forzamiento de tipo tormenta,

𝐽~max~ aumenta casi tres órdenes de magnitud, alcanzando unos pocos

𝜇A.m^−2^ para las tres configuraciones con mástil, mientras que el caso de solo corona nuevamente permanece más bajo en un factor de aproximadamente dos. El comportamiento paralelo de 𝐸~max~ y 𝐽~max~ en las cuatro configuraciones es consistente con el escalado óhmico 𝐽 = 𝜎𝐸 y confirma que el rol principal del mástil y el colector superior es aumentar la cantidad de corriente de fondo interceptada y canalizada a través de la corona, en lugar de introducir diferencias cualitativas fuertes entre los diseños específicos del colector.

> ![](./images/image8.jpeg)

> ***Figura 8. (a) Cuatro geometrías distintas del electrovegetómetro utilizadas en las simulaciones. Las regiones marrones denotan soportes de madera, las líneas rojas conductores metálicos. (b) Campo eléctrico máximo en el distribuidor de corona inferior, Emax, bajo forzamiento de tiempo despejado y de tipo tormenta, mostrando que todas las configuraciones con mástil producen campos pico similares mientras que el caso de solo corona permanece más bajo en el régimen de tormenta. (c) Densidad de corriente de conducción máxima correspondiente, Jmax, en escala logarítmica, ilustrando el aumento de tres órdenes de magnitud de condiciones despejadas a tormentosas y las corrientes mejoradas obtenidas cuando está presente un mástil metálico elevado.***

# Discusión

Las simulaciones presentadas anteriormente proporcionan un primer puente cuantitativo entre la descripción cualitativa de Bertholon de su electrovegetómetro y los conceptos modernos del circuito eléctrico atmosférico global y la amplificación de campo pre-corona. Varios puntos emergen con respecto a (i) la plausibilidad física de la narrativa original de Bertholon, (ii) la magnitud esperada y localización de los efectos eléctricos cerca del dosel y (iii) las limitaciones del marco de modelado actual y sus implicaciones tanto para la interpretación histórica como para las reclamaciones modernas de "electrocultura".

## Operación de tiempo despejado: amplificación localizada pero modesta

Bajo forzamiento de tiempo despejado, el electrovegetómetro reconstruido se comporta como una perturbación débil de la corriente de conducción global. El colector superior y la corona inferior generan ambas fuertes amplificaciones locales del campo (de dos a tres órdenes de magnitud en relación con el campo ambiental de ≈10² V.m⁻¹) pero estas regiones amplificadas permanecen confinadas en vecindarios de mm-cm alrededor de las puntas. El punto superior único concentra la caída de potencial de fondo en un embudo estrecho y alcanza campos pico del orden de unos pocos ×10⁴ V.m⁻¹, mientras que la corona de cinco puntos alcanza aproximadamente 8×10⁴ V.m⁻¹ cerca del vértice central.

Desde un punto de vista puramente electrodinámico, estos campos son lo suficientemente altos como para distorsionar significativamente las trayectorias iónicas y aumentar localmente las tasas de ionización y adjunción, si la atmósfera ya está débilmente ionizada. Sin embargo, las densidades de corriente óhmicas asociadas permanecen en el rango de pA.m⁻² a nA.m⁻² bajo, solo

moderadamente por encima de la corriente de conducción de fondo. La corriente total que puede canalizarse a través de una huella realista de corona, por lo tanto, permanece extremadamente pequeña.

Para el microentorno de la planta, esto implica que, en clima sin perturbaciones, el dispositivo podría plausiblemente crear estrechos "puntos calientes" de campo amplificado y flujo iónico inmediatamente alrededor de cada punta, pero estas perturbaciones decaerían hasta valores cercanos al fondo sobre distancias comparables o menores que las escalas típicas de longitud de hoja y dosel. Cualquier forzamiento electrodinámico directo sobre el tejido vegetal (a través de cargas superficiales inducidas, flujos iónicos impulsados por campo en la capa límite de la hoja o modificación de patrones de deposición de aerosoles) sería, por lo tanto, altamente localizado y probablemente intermitente.

En consecuencia, el régimen de tiempo despejado parece compatible con la idea cualitativa de Bertholon de una influencia continua pero "suave" de la electricidad atmosférica, sin embargo los resultados actuales sugieren que esta influencia es físicamente sutil: el electrovegetómetro no actúa como un fuerte inyector de carga o como un sumidero/fuente significativo en el circuito global. Más bien, remodela la corriente de conducción preexistente local en estrechos chorros sin aumentar significativamente su magnitud.

## Forzamiento de tormenta y la plausibilidad de "aigrettes" luminosas

Bajo forzamiento idealizado de tipo tormenta, la misma geometría opera en un régimen muy diferente. Cuando el campo de fondo y la conductividad se aumentan a valores representativos de condiciones pre-tormenta o afectadas por tormenta, el punto superior y la corona inferior pueden alcanzar campos eléctricos pico que van desde varios 10⁵ V.m⁻¹ hasta la escala de MV.m⁻¹ en el modelo lineal. Estos niveles son comparables a o exceden los umbrales empíricos de arranque de corona para conductores afilados

a presión de suelo y se acercan a las estimaciones convencionales de ruptura.

Es importante enfatizar que, porque el modelo descuida la carga espacial y la retroalimentación de ionización, estos valores en escala MV.m⁻¹ deben interpretarse como *límites superiores* del estado pre-corona en lugar de como campos sostenidos realistas: en una atmósfera real, la corona se activaría antes y la carga espacial resultante filtraría parcialmente las puntas, limitando el crecimiento adicional del campo. No obstante, el hecho de que la solución óhmica pre-corona se acerque naturalmente a los umbrales de arranque de corona bajo forzamiento GEC mejorado es significativo. Proporciona una justificación cuantitativa para los informes de Bertholon de brillos luminosos tenues ("aigrettes lumineuses") en las puntas bajo clima perturbado y para las observaciones históricas del fuego de San Elmo en mástiles de barcos y agujas de iglesias.

En esta imagen, el electrovegetómetro puede actuar como un facilitador de descargas de corona durante períodos cuando la columna atmosférica ya está altamente estresada por la carga de tormenta cercana. El mástil elevado asegura que el colector superior muestree una región de ligeramente mayor conductividad y potencial, mientras que la corona inferior de múltiples puntos concentra esta caída de potencial a la altura del dosel. Las simulaciones muestran que las corrientes de tiempo de tormenta pueden aumentar aproximadamente tres órdenes de magnitud en comparación con el tiempo despejado mientras retienen perfiles de conducción suaves y monótonos alrededor de las puntas. Una vez que se alcanza el arranque de corona, la producción de iones y el transporte de carga cerca del dosel podrían ser sustancialmente mayores que en el régimen de tiempo despejado, potencialmente produciendo brillos visibles y flujos iónicos mejorados.

Sin embargo, esta operación mejorada permanecería episódica, ligada a la presencia de nubes electrificadas cercanas y puede no corresponder a la "mejora" benigna y en estado estacionario de la vegetación que Bertholon tenía en mente. Además, la corona puede producir estrés químico y mecánico localizado (ozono, NOx, UV, calentamiento a micro-escala y cizalla de viento iónico) cuyos impactos en las plantas son complejos y no necesariamente beneficiosos. El presente modelo no puede abordar estos aspectos y, por lo tanto, no puede apoyar o refutar directamente ningún beneficio agronómico reclamado de la operación de tiempo de tormenta.

## Robustez a incertidumbres geométricas y el papel del mástil

Los barridos paramétricos indican que varios aspectos de la respuesta del dispositivo son relativamente robustos a las incertidumbres históricas en la geometría. Variar el ángulo de vértice del colector superior en un amplio rango solo altera el campo máximo y la densidad de corriente cerca de la punta por factores del orden de la unidad, no por órdenes de magnitud. Esto refleja el hecho de que el potencial global disponible para la estructura flotante está establecido por la columna atmosférica impuesta, mientras que la filo de la punta controla cómo esa caída de potencial se localiza en escalas de mm. Del mismo modo, reemplazar el punto superior único por una pequeña corona o extender modestamente el mástil, apenas afecta los campos pico en la corona inferior en condiciones de tiempo despejado o de tormenta. Las simulaciones muestran que, en el régimen de tormenta, todas las configuraciones con mástil (Configuraciones I, II e I extendida) producen Emax y Jmax similares en la corona a nivel del dosel, mientras que una corona aislada sin mástil alcanza máximos significativamente más bajos. Esto sugiere que el rol electrodinámico principal del mástil es interceptar una

porción mejorada de la corriente y el potencial de la columna de fondo, canalizándolos hacia el distribuidor, en lugar de codificar sensiblemente los detalles del diseño del colector.

Desde una perspectiva de reconstrucción histórica, esto es tranquilizador: incluso si el hardware real de Bertholon se desviaba de la geometría estilizada utilizada aquí, las conclusiones cualitativas sobre la operación de tiempo despejado versus de tormenta, la localización de campos y la importancia relativa del colector versus el distribuidor es improbable que cambien drásticamente. La corona de múltiples puntos cerca del dosel de cultivos surge como la característica dominante para la amplificación local del campo, mientras que el mástil y el colector condicionan principalmente cuánto "voltaje" se entrega a ella.

## Limitaciones del modelo actual

A pesar de su utilidad como herramienta exploratoria, el presente modelo 2D, lineal, óhmico tiene varias limitaciones importantes que restringen la interpretación de los resultados:

-   El modelo asume un perfil de conductividad prescrito y la ley lineal de Ohm, sin tratamiento explícito de producción de carga, adjunción, recombinación o deriva más allá de lo que está codificado en σ(z). Una vez que los campos se acercan a los umbrales de arranque de corona, esta aproximación se rompe. Los campos pico simulados en el régimen de tipo tormenta deben, por lo tanto, verse como indicativos de dónde es probable el arranque, no como predicciones literales de valores sostenidos de MV.m⁻¹.

-   La configuración en sección transversal del electrovegetómetro representa una estructura infinitamente larga, lo que conduce a puntas de tipo cuña en lugar de puntas cónicas 3D realistas. Esto afecta los factores de amplificación locales y la topología de las líneas de campo cerca de los vértices. Una simulación 3D completa probablemente produciría diferentes valores absolutos de Emax y posiblemente regiones de campo alto más amplias, aunque las tendencias básicas (amplificación localizada, decaimiento decimétrico al fondo, insensibilidad relativa al ángulo de vértice del colector) deberían permanecer cualitativamente similares.

-   Los soportes de madera se modelan con conductividades fijas y bajas y el suelo se trata implícitamente a través de condiciones de contorno en lugar de como un conductor estratificado y dependiente de la humedad. En la práctica, sin embargo, Bertholon dedicó considerable atención a mejorar el aislamiento: la sección enterrada del mástil se secó al fuego, se alquitranó, se envolvió en polvo de carbón y cemento, luego se asentó en albañilería, mientras que la parte sobre el suelo se pintó o cubrió con betún; la cabeza del mástil se protegió aún más con inserciones saturadas en resina y mangas de vidrio/mastique y los brazos horizontales se llevaron sobre caballetes aislantes con cuerdas de seda (Tabla 1). Estas medidas probablemente redujeron las fugas y aumentaron la resistencia del soporte, sin embargo sus propiedades aún dependían de la humedad, el envejecimiento y la contaminación, por lo que las rutas de fuga y el potencial flotante (y por lo tanto Emax y Jmax) pueden haber cambiado solo por factores moderados.

-   Los regímenes de "tiempo despejado" y "tipo tormenta" se representan perfiles simples y horizontales uniformes con J0,atm y E0,atm prescritos. Los entornos eléctricos atmosféricos reales sobre campos agrícolas están influenciados por la topografía, estructuras cercanas, carga de aerosoles e inhomogeneidades horizontales en la carga de tormenta. El campo local en el electrovegetómetro podría, por lo tanto, desviarse

> significativamente de los perfiles idealizados adoptados aquí, especialmente bajo condiciones convectivas complejas.

-   Las simulaciones no incluyen representaciones explícitas de vegetación. Las hojas, tallos y estructura del dosel pueden distorsionar el campo y actuar como conductores adicionales o aislantes parciales, redistribuyendo corrientes y modificando el paisaje de potencial cercano a la superficie. También pueden participar en el intercambio de carga a través de películas de conducción superficial, aberturas estomatales o capas de humectación. Los resultados actuales proporcionan, por lo tanto, una imagen de primer orden del campo "en el aire", no una descripción completa del acoplamiento planta-campo.

## Implicaciones para la historia y la práctica moderna de la "electrocultura"

Dentro de estas limitaciones, los resultados del modelado apoyan una reevaluación matizada del electrovegetómetro de Bertholon. Por un lado, el dispositivo es físicamente capaz de generar fuertes amplificaciones locales de campo y, bajo condiciones de tiempo de tormenta, de acercarse o exceder los umbrales de arranque de corona, haciendo que las "aigrettes" luminosas sean plausibles. Por otro lado, en su estado operativo principal de tiempo despejado (que dominaría la exposición diaria), la estructura parece actuar principalmente como un concentrador pasivo de campo con corrientes totales pequeñas y perturbaciones altamente localizadas.

Esta imagen dual sugiere que la intuición conceptual de Bertholon sobre la existencia de una influencia eléctrica persistente sobre la vegetación no estaba completamente equivocada, pero que sus expectativas sobre la fuerza y las consecuencias agronómicas de esta influencia podrían haber sido optimistas. El electrovegetómetro es mejor interpretado como una sonda delicada del circuito eléctrico global en la capa cercana a la superficie y como un demostrador de concentración de campo y fenómenos de corona, que como un "mejorador" agrícola robusto en el sentido de ingeniería moderno.

Para las discusiones contemporáneas de "electrocultura", un término que ha resurgido recientemente en contextos populares y a veces pseudocientíficos, el presente trabajo subraya la necesidad de un modelado cuidadoso y cuantitativo y experimentos controlados. Los dispositivos que se asemejan a electrovegetómetros históricos pueden efectivamente modificar el entorno eléctrico local alrededor de las plantas, pero la magnitud, el signo y la relevancia biológica de estas modificaciones no pueden inferirse solo de analogías cualitativas. Requieren una combinación de mediciones atmosférico-eléctricas, estudios detallados de fisiología vegetal y modelos que se extiendan más allá del régimen pre-corona, lineal considerado aquí.

# Conclusión

Reexaminando el electrovegetómetro del siglo XVIII de Bertholon dentro del marco de la electrodinámica atmosférica moderna, este estudio ha desarrollado un modelo cuasi-estacionario, bidimensional, resistivo del sistema aire-dispositivo, en el que la atmósfera se trata como un medio óhmico que transporta la corriente de conducción global y la estructura metálica se representa como un conductor flotante soportado por aislantes de madera con fugas. La resolución de la ecuación de conducción estacionaria con conductividad dependiente de la altitud

y configuraciones realistas ha producido estimaciones cuantitativas de potenciales, campos eléctricos y densidades de corriente alrededor del electrovegetómetro bajo forzamiento idealizado de tiempo despejado y de tipo tormenta.

Los hallazgos principales pueden resumirse de la siguiente manera:

-   Bajo condiciones típicas de tiempo despejado, las puntas afiladas del electrovegetómetro amplifican el campo eléctrico local entre dos y tres órdenes de magnitud en relación con el campo atmosférico de fondo, alcanzando decenas de kV.m⁻¹ en el punto superior único y aproximadamente 80 kV.m⁻¹ en la corona inferior de múltiples puntos. Las densidades de corriente asociadas permanecen en el rango de pA-nA/m2, consistente con una conducción débil en un medio ligeramente ionizado. Las perturbaciones de campo y corriente están fuertemente localizadas y decaen hasta valores cercanos al ambiente dentro de cm.

-   Cuando el campo de fondo y la conductividad se aumentan a valores representativos de condiciones pre-tormenta o afectadas por tormenta, la misma geometría produce campos pico en el rango de 10⁵-10⁶ V.m⁻¹. Estos niveles se acercan o exceden los umbrales empíricos de arranque de corona y se acercan a las estimaciones de ruptura, particularmente en la corona inferior. Dentro de los límites de una aproximación lineal sin carga espacial, estos resultados indican que el dispositivo de Bertholon podría haber producido brillos de corona y flujos iónicos mejorados durante clima perturbado, proporcionando una base física plausible para los informes históricos de "aigrettes" luminosas.

-   Las variaciones paramétricas del ángulo de vértice superior y la geometría del colector muestran que los campos pico y corrientes de tiempo despejado y de tormenta cerca de la corona inferior son en gran medida insensibles a los detalles finos del colector, siempre que esté presente un mástil elevado. La función principal del mástil es interceptar una porción del potencial de columna atmosférica y canalizarla hacia el distribuidor, mientras que la corona de múltiples puntos cerca de la altura del dosel permanece como la característica dominante que controla la amplificación local del campo.

-   Los resultados dependen de los supuestos de una geometría 2D, conducción óhmica lineal, perfiles de conductividad prescritos y propiedades de materiales simplificadas. Deben, por lo tanto, verse como límites superiores pre-corona en lugar de predicciones completamente realistas del comportamiento de descarga. Dentro de estos límites, el estudio sugiere que el electrovegetómetro de Bertholon era físicamente capaz de concentrar la electricidad atmosférica y ocasionalmente producir corona visible bajo forzamiento de tiempo de tormenta, mientras que su influencia de tiempo despejado sobre las plantas era probablemente sutil, localizada y difícil de cuantificar con instrumentos del siglo XVIII.

Finalmente, este trabajo ilustra cómo el modelado numérico moderno del circuito eléctrico atmosférico global, incluso en una forma simplificada pre-corona, puede afianzar nuestra comprensión de dispositivos electrotécnicos históricos y sus modos plausibles de operación. Las extensiones futuras podrían incluir simulaciones 3D completas, tratamiento explícito de carga espacial y dinámica de corona, representaciones más realistas de suelo y vegetación y experimentos acoplados en entornos atmosférico-eléctricos controlados. Tales estudios no solo refinarían la evaluación retrospectiva del electrovegetómetro de Bertholon sino que también informarían los debates contemporáneos sobre la significación física y biológica de las perturbaciones atmosférico-eléctricas débiles en entornos agrícolas.

# Referencias

[Aplin, 2008] K. L. Aplin, R. G. Harrison, M. J. Rycroft. Investigating Earth's Atmospheric Electricity: a Role Model for Planetary Studies. Space Sci Rev, Vol. 137, pp. 11-27 (2008). [https://doi.org/10.1007/s11214-008-9372-x]

[Winkler et al., 1898] J. H. Winkler, B. Franklin, T. F. Dalibard, L. G. Le Monnier. Ueber Luftelektricität. Neudruck Von Schriften Und Karten Über Meteorologie Und Erdmagnetismus Herausgegeben Von Professor Dr. G. Hellmann. N°11. Berlin, A. Asher & Co. (1898).

[Bailey, 2001] A. G. Bailey. The charging of insulator surfaces. Journal of Electrostatics. Vol. 51-52, pp. 82-90 (2001). [https://doi.org/10.1016/S0304-3886(01)00106-1]00106-1)

[Bertholon, 1783] Bertholon. De l'électricité des végétaux. A Paris, chez P. F. Didot Jeune, quai des Augustins (1783).

[Guha, 2010] A. Guha, B. K. De, S. Gurubaran, S. S. De, K. Jeeva. First results of fair-weather atmospheric electricity measurements in Northeast India. J. Earth Syst. Sci., Vol. 119, pp. 221-228 (2010). [https://doi.org/10.1007/s12040-010-0014-9]

[Herbert, 2012] K. B. H. Herbert. John Canton — Pioneer investigator of atmospheric electricity. Weather, RMetS, Vol. 52, Issue 9, pp. 286-290 (1997). [https://doi.org/10.1002/j.1477-8696.1997.tb06326.x]

[Kudintseva, 2016] I. G. Kudintseva, A. P. Nickolaendro, M. J. Rycroft, A. Odzimek. AC and DC global electric circuit properties and the height profile of atmospheric conductivity. Annals of geophysics, Vol. 59, 5, A0545 (2016). [https://www.doi.org/10.4401/ag-6870]

[Kundt, 1999] W. Kundt, G. Thuma. Geoelectricity: atmospheric charging and thunderstorms. Journal of Atmospheric and Solar-Terrestrial Physics, Vol. 61, pp. 955-963 (1999). [https://doi.org/10.1016/S1364-6826(99)00061-9]00061-9)

[Mareev, 2014] E. A. Mareev, E. M. Volodin. Variation of the global electric circuit and Ionospheric potential in a general circulation model. Geophysical Research Letters, Vol. 41, Issue 24, pp. 9009-9016 (2014). [https://doi.org/10.1002/2014GL062352]

[McGinness, 2025] B. P. S. McGinness, R. Giles Harrison, K. L. Aplin,

M. W. Airey. The role of point discharge in the historical development of atmospheric electricity. Hist. Geo Space Sci., 16, 51-63 (2025). [https://doi.org/10.5194/hgss-16-51-2025]

[Standler, 1979] R. B. Standler, W. P. Winn. Effects of coronae on electric fields beneath thunderstorms. Quaterly J. of Royal Meteorological Society, Vol. 105, 443, pp. 285-302 (1979). [https://doi.org/10.1002/qj.49710544319Ci]

[Tinsley, 2007] B. A. Tinsley, G. B. Burns, L. Zhou. The role of the global electric circuit in solar and internal forcing of clouds and climate. Advances in Space Research Vol. 40, Issue 7, pp. 1126-1139 (2007). [https://doi.org/10.1016/j.asr.2007.01.071]

[Williams, 2009] E. R. Williams. C.T.R. Wilson versus G.C. Simpson: Fifty years of controversy in atmospheric electricity. Atmospheric Research; Vol. 91, Issues 2-4, pp. 259-271 (2009). [https://doi.org/10.1016/j.atmosres.2008.03.024]
