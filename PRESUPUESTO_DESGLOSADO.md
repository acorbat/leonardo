# Presupuesto Total Bruto Desglosado - Becas Leonardo 2026

**Convocatoria:** Becas Leonardo a Investigadores y Creadores Culturales 2026 (Argentina, Colombia y Perú)  
**Entidad Convocante:** Fundación BBVA  
**Solicitante:** Investigador Postulante  
**Proyecto:** *Desarrollo de Plataforma Computacional Integral de Bioimagen, Visión Artificial y Genómica para el Diagnóstico de la Disquinesia Ciliar Primaria*  
**Institución Sede de Ejecución:** Facultad de Ciencias Exactas y Naturales - Universidad de Buenos Aires (FCEN-UBA)  
**Institución en Colaboración Clínica:** Hospital de Niños Dr. Ricardo Gutiérrez (Buenos Aires, Argentina)  
**Moneda de Presentación:** Dólares Estadounidenses (USD)  
**Plazo de Ejecución:** 18 meses  
**Monto Total Solicitado:** **USD 50.000,00** (Cincuenta mil dólares brutos - Asignación 100%)  

---

## 1. Tabla Resumen por Rubro Presupuestario

| N° | Rubro de Gasto | Monto Bruto (USD) | % del Total Solicitado |
| :---: | :--- | :---: | :---: |
| **1** | **Hardware e Instrumentación** | $10.000,00 | 20,0% |
| **2** | **Equipamiento Informático (Hospital y FCEN-UBA)** | $5.000,00 | 10,0% |
| **3** | **Patrones de Calibración, Reactivos e Insumos** *(Aportados por FCEN y Hospital)* | $0,00 | 0,0% |
| **4** | **Recursos Humanos, Estipendios y Servicio de Microscopía TEM** | $15.100,00 | 30,2% |
| **5** | **Difusión Científica, Publicaciones Open Access y Congresos** | $9.000,00 | 18,0% |
| **6** | **Costos de Administración Institucional, Impuestos y Variaciones de Costos** | $10.900,00 | 21,8% |
| | **TOTAL BRUTO GENERAL SOLICITADO:** | **$50.000,00** | **100,0%** |

---

## 2. Desglose Detallado por Ítem y Justificación Técnica

### Rubro 1: Hardware e Instrumentación ($10.000,00 USD)
*Este rubro moderniza la estación de videomicroscopía in situ para diagnóstico funcional ciliar en colaboración con los médicos del Hospital Gutiérrez, dotándola de control térmico estricto a 37 °C y alta resolución temporal (>200 fps).*

1.  **Cámara Científica de Alta Velocidad Axiocam 705 mono:**
    *   *Descripción:* Cámara monocromática con sensor CMOS científico de alta sensibilidad y bajo ruido de lectura, adquirida en plaza nacional a través del distribuidor oficial en Argentina (**Bioingeniería**). El costo en plaza es del orden de 8.000 USD, presupuestándose en 9.000 USD para contar con margen de seguridad ante posibles variaciones arancelarias o de cotización de plaza y asegurar la concreción del gasto. Al adquirirse localmente, se prescinde de gestiones aduaneras y fletes internacionales. La cámara operará en una región de interés (ROI) de **512 x 512 píxeles**, superando los **200 fps**. Combinada con un objetivo de **20x** y el adaptador de reducción de 0,5x existente, corrige el actual problema de sobresampleo óptico (que utilizaba aumentos excesivos degradando el campo y la luminosidad), garantizando una excelente resolución espacial y temporal para el análisis cinético ciliar según estándares internacionales.
    *   *Monto:* **$9.000,00 USD**
2.  **Componentes para Cámara Ambiental Termostatizada (37 °C) y Humedad:**
    *   *Descripción:* Estructura y chasis hermético fabricados mediante manufactura aditiva (impresión 3D en filamento técnico termoplástico PETG), lazo de control térmico PID basado en microcontrolador de bajo costo (**Arduino o ESP32**), sensores digitales de temperatura de bajo costo calibrados, platina calefactora de bajo voltaje y reservorio higrométrico para humedad relativa >90% (evitando la desecación y alteración ciliar durante la ventana de viabilidad ex vivo de 3 a 9 horas).
    *   *Monto:* **$1.000,00 USD**
3.  **Adaptador Óptico C-Mount de Reducción:**
    *   *Descripción:* El microscopio óptico del hospital ya cuenta con un adaptador C-mount de reducción de 0,5x funcional y compatible, por lo que **no se requiere la compra** de una nueva óptica de acoplamiento (ítem disponible a costo cero).
    *   *Monto:* **$0,00 USD**
4.  **Costos de Importación, Fletes Internacionales y Aranceles Aduaneros:**
    *   *Descripción:* Al adquirirse la cámara Axiocam 705 mono a través del distribuidor local (Bioingeniería) y construirse la cámara ambiental con componentes comerciales locales e impresión 3D, no se generan costos de importación directa ni intermediación aduanera.
    *   *Monto:* **$0,00 USD**

---

### Rubro 2: Equipamiento Informático (Hospital y FCEN-UBA) ($5.000,00 USD)
*Unidades de cómputo dedicadas tanto a la adquisición sincrónica in situ en el servicio clínico como al desarrollo algorítmico y procesamiento intensivo por parte de los estudiantes en la universidad.*

1.  **Computadora para Control del Microscopio y Adquisición in situ (Hospital Gutiérrez):**
    *   *Descripción:* Computadora de alta potencia dedicada a la estación del microscopio en el Hospital Gutiérrez para la captura sincrónica de secuencias de video a alta velocidad (>200 fps) con la cámara Axiocam 705 mono y el software Micro-Manager. Se adquirirá como **laptop de alto rendimiento o computadora de escritorio (desktop)** según resulte más conveniente en función del espacio físico y la ergonomía del servicio clínico. Equipada con procesador multinúcleo moderno (Intel Core i7 / AMD Ryzen 7), 32 a 64 GB de memoria RAM de alta velocidad (esencial para streaming de video continuo a memoria volátil sin saturar el búfer ni perder fotogramas), disco sólido SSD NVMe ultrarrápido y puertos USB 3.2 / GigE dedicados.
    *   *Monto:* **$2.000,00 USD**
2.  **Estación de Trabajo para Estudiantes de Desarrollo (FCEN-UBA):**
    *   *Descripción:* Workstation de cómputo de alto rendimiento instalada en los laboratorios de la FCEN-UBA, destinada al puesto de trabajo de los estudiantes del proyecto. Equipada con procesador multinúcleo de alta gama, placa gráfica dedicada (GPU NVIDIA con núcleos Tensor) para aceleración del entrenamiento de modelos de deep learning y machine learning (**convpaint**), 64 GB de memoria RAM DDR5 y arreglo de almacenamiento rápido SSD NVMe para procesamiento intensivo de videomicroscopía y bioimágenes de TEM.
    *   *Monto:* **$3.000,00 USD**
3.  **Infraestructura de Servidores y Almacenamiento Masivo de la Facultad:**
    *   *Descripción:* La FCEN-UBA ya cuenta con clústeres de cálculo y servidores de almacenamiento centralizado para resguardo masivo y backup de repositorios genómicos y bioimágenes, complementando la estación de trabajo sin costo adicional para la subvención (ítem disponible a costo cero).
    *   *Monto:* **$0,00 USD**

---

### Rubro 3: Patrones de Calibración, Reactivos e Insumos ($0,00 USD)
*Insumos provistos íntegramente por las instituciones participantes.*

1.  **Reactivos, Portaobjetos Especiales y Patrones Micrométricos:**
    *   *Descripción:* Tanto los patrones ópticos de calibración micrométrica, como los insumos de banco de pruebas, soluciones buffer y preparados de referencia son provistos por los laboratorios de la FCEN-UBA y el Hospital Gutiérrez, no requiriendo financiamiento presupuestario en esta propuesta (ítem disponible a costo cero).
    *   *Monto:* **$0,00 USD**

---

### Rubro 4: Recursos Humanos, Estipendios y Servicio de Microscopía TEM ($15.100,00 USD)
*Formación de 3 estudiantes universitarios en FCEN-UBA (2 estudiantes de grado y 1 estudiante de finalización de carrera) y contratación integral del servicio institucional de microscopía electrónica de transmisión.*

1.  **Estipendios Estudiantiles de Iniciación - Estudiantes de Grado de Física (FCEN-UBA, 2 estudiantes por 12 meses):**
    *   *Descripción:* Asignación económica de estímulo a la investigación para **2 estudiantes avanzados de grado de la Licenciatura en Ciencias Físicas** de la FCEN-UBA. Tendrán como responsabilidad específica **diseñar, validar e implementar** la cámara de control de temperatura y humedad para el microscopio (12 meses x $350,00 USD/mes cada uno = $4.200 x 2).
    *   *Monto:* **$8.400,00 USD**
2.  **Estipendio para Estudiante de Finalización de Carrera (FCEN-UBA, 1 estudiante por 12 meses):**
    *   *Descripción:* Asignación económica para **1 estudiante de finalización de carrera / próximo a graduarse** (tesista) de la FCEN-UBA. Tendrá a su cargo el **análisis computacional de bioimágenes de videomicroscopía** (flujo óptico, FFT para CBF/CBP) y **microscopía electrónica de transmisión** (detección de axonemas con convpaint y análisis de brazos de dineína) (12 meses x $350,00 USD/mes).
    *   *Monto:* **$4.200,00 USD**
3.  **Pasantes de Ciencia de Datos para Análisis Genéticos (FCEN-UBA):**
    *   *Descripción:* Para los análisis bioinformáticos de genética (anotación de variantes patogénicas, minería en repositorios abiertos y modelado estructural), la FCEN-UBA cuenta con **pasantes de la carrera de Ciencia de Datos** que realizan proyectos de análisis cortos y específicos integrados en su formación académica, colaborando sin generar erogaciones presupuestarias directas (ítem disponible a costo cero).
    *   *Monto:* **$0,00 USD**
4.  **Servicios Técnicos de Mecanizado y Taller:**
    *   *Descripción:* Los mecanizados de precisión en aluminio requeridos para la platina térmica y los ajustes mecánicos serán realizados íntegramente por el personal técnico del Taller Mecánico de la FCEN-UBA, sin requerir contratación externa (ítem disponible a costo cero).
    *   *Monto:* **$0,00 USD**
5.  **Servicio Integral de Microscopía Electrónica de Transmisión (TEM):**
    *   *Descripción:* Contratación integral con el Servicio de Microscopía Electrónica institucional para cubrir en un único ítem consolidado tanto la **preparación y procesamiento ultraestructural de muestras biológicas** (fijación química con glutaraldehído y tetraóxido de osmio, inclusión en resina epoxi, ultramicrotomía de 70–90 nm y tinción de contraste doble) como las **horas de uso de microscopio TEM**, asegurando el banco de imágenes de alta resolución necesario para la calibración del modelo convpaint.
    *   *Monto:* **$2.500,00 USD**

---

### Rubro 5: Difusión Científica, Publicaciones Open Access y Congresos ($9.000,00 USD)
*Garantiza la máxima difusión del conocimiento, el estricto cumplimiento de la política de Ciencia Abierta y la alta visibilidad de la Fundación BBVA.*

1.  **Cargos por Procesamiento de Artículos en Acceso Abierto (Open Access APCs):**
    *   *Descripción:* Cobertura de cargos de publicación en acceso abierto (APC) en 2 a 3 revistas internacionales indexadas de primer cuartil (Q1) en computación médica, visión artificial o neumonología pediátrica, asegurando que las herramientas algorítmicas, el código fuente y los hallazgos metodológicos estén disponibles para la comunidad científica mundial sin barreras de suscripción.
    *   *Monto:* **$6.000,00 USD**
2.  **Participación en Congresos Científicos y Difusión:**
    *   *Descripción:* Inscripciones, pasajes, viáticos y materiales para la presentación de los avances y resultados del proyecto en congresos nacionales e internacionales de microscopía, bioinformática e ingeniería biomédica, reconociendo el patrocinio de las Becas Leonardo de la Fundación BBVA.
    *   *Monto:* **$3.000,00 USD**

---

### Rubro 6: Costos de Administración Institucional, Impuestos y Variaciones de Costos ($10.900,00 USD)
*Gestión institucional, requerimientos bancarios e impositivos y fondo de contingencia operativa frente a variaciones de costos.*

1.  **Administración Universitaria, Impuestos y Fondo de Previsión ante Variaciones de Costos:**
    *   *Descripción:* Fondo destinado a cubrir los aranceles de administración institucional del convenio a través de la sede (FCEN-UBA / fundación universitaria gestora), comisiones bancarias por recepción y transferencia internacional de divisas (tres desembolsos preceptivos de BBVA: 50%, 40% y 10%), gravámenes impositivos locales y una sólida previsión de contingencia frente a eventuales fluctuaciones cambiarias, arancelarias y variaciones en las estimaciones de costos durante los 18 meses de ejecución del proyecto, asegurando la plena sustentabilidad y blindaje financiero de la propuesta.
    *   *Monto:* **$10.900,00 USD**

---

## 3. Justificación de la Costo-Efectividad de la Propuesta

### Muy Alta Costo-Efectividad de la Asignación Presupuestaria
*   Un sistema comercial cerrado de videomicroscopía ciliar de alta velocidad (HSVM) importado llave en mano cuesta entre **USD 120.000 y USD 180.000**, lo que resulta prohibitivo para hospitales públicos en Argentina y la región.
*   Con la asignación integral de los **USD 50.000** de la Beca Leonardo (100% de los fondos de la convocatoria), el proyecto logra:
    1.  Modernizar el microscopio del Hospital Gutiérrez con una cámara científica de alta velocidad (Axiocam 705 mono presupuestada con holgura en USD 9.000) y una cámara termostatizada a 37 °C fabricada aditivamente en FCEN-UBA ($1.000 USD).
    2.  Proveer una unidad de cómputo potente para el hospital ($2.000 USD, laptop o desktop) para control y adquisición sincrónica in situ, más una estación de trabajo GPU dedicada para los estudiantes en FCEN-UBA ($3.000 USD).
    3.  Aprovechar la infraestructura preexistente de servidores, talleres y laboratorios de la FCEN-UBA y del hospital (ítems de costo cero detallados en la factibilidad técnica e institucional).
    4.  Financiar el estipendio anual de **tres estudiantes universitarios** en FCEN-UBA (dos de grado de Física para hardware ambiental y uno de finalización de carrera para bioimágenes a $350 USD/mes cada uno, totalizando $12.600 USD), complementado con la articulación formativa de pasantes de ciencia de datos.
    5.  Financiar de manera integral el procesamiento ultraestructural de muestras y las horas de TEM mediante el servicio institucional ($2.500 USD).
    6.  Garantizar publicaciones en revistas de primer cuartil (Q1) en acceso abierto y difusión en congresos científicos ($9.000 USD).
    7.  Blindar el proyecto contra contingencias cambiarias, impuestos locales, aranceles universitarios y variaciones en las estimaciones de costos ($10.900 USD).


