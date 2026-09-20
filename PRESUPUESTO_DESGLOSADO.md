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
| **6** | **Administración Institucional (Overhead 10%), Costos Financieros y Previsión** | $10.900,00 | 21,8% |
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

### Rubro 6: Costos de Administración Institucional (Overhead 10%), Costos Financieros y Previsión ($10.900,00 USD)
*Gestión institucional vía FUNDACEN o Hacienda, contribuciones reglamentarias universitarias, comisiones bancarias por divisas y fondo de previsión ante variaciones de costos.*

Dado que la percepción y administración de los fondos de la Beca Leonardo de la Fundación BBVA se tramita de forma institucional a través de la sede universitaria, se incluye un **overhead institucional del 10,0% ($5.000,00 USD)** (dentro del rango normativo de 7,5% a 10%), distribuido según la reglamentación aplicable entre la entidad administradora/gestora, la facultad y el departamento o instituto ejecutor. El remanente presupuestario de este rubro ($5.900,00 USD) cubre las comisiones bancarias por transferencias internacionales de divisas en los tres desembolsos de la Fundación BBVA, gravámenes locales y un fondo de contingencia operativa frente a variaciones de costos.

1.  **Overhead Institucional - Entidad Administradora / Gestora (FUNDACEN o Hacienda FCEN-UBA, 5,0%):**
    *   *Descripción:* Retención reglamentaria institucional para la administración contable y financiera, compras y contrataciones, liquidación de estipendios a estudiantes, rendiciones de cuentas periódicas y gestión integral de los fondos del convenio a través de la Fundación de la Facultad de Ciencias Exactas y Naturales (FUNDACEN) o la Dirección General de Hacienda de la FCEN-UBA.
    *   *Monto:* **$2.500,00 USD** (5,0% de la ayuda total de USD 50.000)
2.  **Overhead Institucional - Facultad de Ciencias Exactas y Naturales (FCEN-UBA, 2,5%):**
    *   *Descripción:* Aporte institucional a la sede central universitaria por el uso y soporte de la infraestructura edilicia, laboratorios, servicios generales, seguridad y conectividad de alta velocidad que sustentan el proyecto.
    *   *Monto:* **$1.250,00 USD** (2,5% de la ayuda total de USD 50.000)
3.  **Overhead Institucional - Unidad Académica Ejecutora (Departamento de Física / Instituto, 2,5%):**
    *   *Descripción:* Contribución asignada al Departamento de Física (y/o instituto de investigación FCEN-UBA/CONICET sede de trabajo del investigador postulante y los estudiantes becarios), destinada al sostenimiento operativo de talleres mecánicos y electrónicos, laboratorios de docencia/investigación y facilidades computacionales de base.
    *   *Monto:* **$1.250,00 USD** (2,5% de la ayuda total de USD 50.000)
4.  **Comisiones Bancarias por Transferencias Internacionales de Divisas e Impuestos:**
    *   *Descripción:* Cobertura de gastos bancarios de corresponsalía internacional, transferencias de divisas y comisiones de recepción en los tres desembolsos preceptivos de la Fundación BBVA (50% anticipo inicial, 40% desembolso intermedio y 10% liquidación final), así como retenciones o gravámenes fiscales locales aplicables.
    *   *Monto:* **$2.500,00 USD**
5.  **Fondo de Previsión ante Variaciones de Costos y Contingencias Operativas:**
    *   *Descripción:* Fondo de reserva técnica para absorber eventuales fluctuaciones cambiarias, variaciones en las cotizaciones de plaza de insumos y servicios técnicos durante los 14 a 18 meses de ejecución del plan de trabajo, garantizando el blindaje financiero del proyecto sin comprometer ninguna actividad sustantiva.
    *   *Monto:* **$3.400,00 USD**

*Subtotal Rubro 6:* **$10.900,00 USD** (21,8%)

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
    7.  Cubrir rigurosamente el overhead institucional normativo del 10% ($5.000 USD: 5% FUNDACEN/Hacienda, 2,5% FCEN y 2,5% Departamento de Física/Instituto), las comisiones bancarias de transferencias internacionales e impuestos ($2.500 USD), y una reserva técnica de previsión ante variaciones de costos y contingencias ($3.400 USD), totalizando $10.900 USD.

---

## 4. Planilla de Ejecución Presupuestaria Cronológica (Modelo Excel Convocatoria)

La siguiente tabla replica la estructura del modelo en planilla de cálculo (Excel) requerido para la presentación del presupuesto ante la Fundación BBVA. Los meses de ejecución están estrictamente coordinados con los paquetes de trabajo (WPs) y las tareas del cronograma detallado en la **Memoria Técnica** (`MEMORIA_TECNICA.tex`):

### 4.1 Tabla Principal de Erogaciones Presupuestarias Solicitadas (USD 50.000,00)

| Rubro/actividad | Mes de ejecución | Monto en dólares |
| :--- | :---: | :---: |
| **Hardware e Instrumentación:** Componentes para diseño, calibración y fabricación de cámara ambiental termostatizada (37 °C ± 0,3 °C) y control de humedad relativa saturada (>90%) con sensores digitales, platina calefactora, microcontrolador Arduino/ESP32 y manufactura aditiva PETG (WP1.1) | Meses 1–2 | $1.000,00 |
| **Hardware e Instrumentación:** Cámara científica monocromática de alta velocidad Axiocam 705 mono (>200 fps en ROI 512×512 px) provista por distribuidor oficial en plaza local (Bioingeniería) para videomicroscopía in situ (WP1.2) | Meses 3–4 | $9.000,00 |
| **Equipamiento Informático:** Estación de trabajo (Workstation) de alto rendimiento con GPU dedicada (NVIDIA con Tensor Cores) para desarrollo algorítmico de visión artificial, deep learning (*convpaint*) y procesamiento de bioimágenes en FCEN-UBA (Soporte WP2 y WP3) | Meses 1–2 | $3.000,00 |
| **Equipamiento Informático:** Computadora (desktop o laptop de alta potencia con 32–64 GB RAM y disco NVMe ultrarrápido) dedicada a la estación del microscopio en el Hospital Gutiérrez para adquisición sincrónica in situ y streaming a >200 fps sin pérdida de fotogramas (WP1.3) | Meses 4–5 | $2.000,00 |
| **Recursos Humanos / Estipendios:** Estipendio de estímulo a la investigación para 2 estudiantes avanzados de grado de la Licenciatura en Ciencias Físicas (FCEN-UBA) dedicados al diseño, validación e implementación de la cámara ambiental y control térmico (WP1.1) (12 meses × $350,00 USD/mes cada uno) | Meses 1–12 | $8.400,00 |
| **Recursos Humanos / Estipendios:** Estipendio de investigación para 1 estudiante de finalización de carrera / tesista de grado (FCEN-UBA) a cargo del análisis computacional de bioimágenes de videomicroscopía (CBF/CBP por FFT y flujo óptico) y microscopía electrónica TEM (*convpaint*) (WP2 y WP3) (12 meses × $350,00 USD/mes) | Meses 2–13 | $4.200,00 |
| **Servicios Técnicos Especializados:** Servicio integral institucional de Microscopía Electrónica de Transmisión (TEM): preparación y procesamiento ultraestructural de muestras biológicas (fijación química, inclusión en resina epoxi, ultramicrotomía de 70–90 nm, tinción de contraste doble) y horas de uso de microscopio TEM institucional (WP3.1) | Meses 5–8 | $2.500,00 |
| **Difusión Científica y Congresos:** Inscripciones, pasajes, traslados y viáticos para presentación de ponencias y resultados del proyecto en congresos científicos nacionales e internacionales de bioimagen, visión artificial y neumonología pediátrica (WP5.3) | Meses 10–14 | $3.000,00 |
| **Difusión Científica y Publicaciones:** Cargos por procesamiento de artículos (APCs) para la publicación de 2 a 3 artículos científicos en revistas internacionales indexadas de primer cuartil (Q1) bajo modalidad de acceso abierto (*Open Access*) (WP5.3) | Meses 12–14 | $6.000,00 |
| **Administración Institucional (Overhead 5,0%):** Entidad gestora del convenio (FUNDACEN o Dirección General de Hacienda FCEN-UBA) para administración financiera, rendición de cuentas, compras y contrataciones | Meses 1–14 | $2.500,00 |
| **Administración Institucional (Overhead 2,5%):** Facultad de Ciencias Exactas y Naturales (FCEN-UBA), sede institucional del proyecto, por uso de infraestructura edilicia, conectividad y servicios generales | Meses 1–14 | $1.250,00 |
| **Administración Institucional (Overhead 2,5%):** Departamento de Física / Instituto de adscripción (FCEN-UBA), unidad ejecutora, para soporte operativo de talleres, laboratorios y equipamiento | Meses 1–14 | $1.250,00 |
| **Costos Financieros e Impuestos:** Comisiones bancarias por transferencias internacionales de divisas en los 3 desembolsos de BBVA (50%, 40% y 10%) y gravámenes locales aplicables | Meses 1–14 | $2.500,00 |
| **Previsión y Contingencia:** Fondo de reserva técnica ante variaciones de costos de plaza, fluctuaciones cambiarias o arancelarias durante la ejecución | Meses 1–14 | $3.400,00 |
| **TOTAL GENERAL SOLICITADO (USD)** | **Meses 1–14** | **$50.000,00** |

*(Nota para carga unificada en Excel: si el formulario de la convocatoria requiere consolidar el Rubro 6 en un único renglón, corresponde consignar: "Administración Institucional (Overhead 10%: FUNDACEN/Hacienda 5%, FCEN 2,5%, Depto. 2,5%), Costos Financieros e Impuestos ($2.500) y Fondo de Previsión ($3.400)", por un monto de $10.900,00 USD con período de ejecución en Meses 1–14).*

---

### 4.2 Aportes Institucionales y Recursos Preexistentes a Costo Cero (Contrapartida)

Para reflejar la integridad de la matriz de recursos del proyecto, a continuación se detallan las actividades e insumos esenciales provistos por la FCEN-UBA y el Hospital Gutiérrez sin erogación presupuestaria adicional para la Fundación BBVA:

| Rubro/actividad | Mes de ejecución | Monto en dólares |
| :--- | :---: | :---: |
| **Hardware Óptico:** Adaptador C-mount de reducción de 0,5x preexistente y compatible en el microscopio del Hospital Gutiérrez (optimización de muestreo y luminosidad con objetivo 20x) | Mes 1 | $0,00 |
| **Logística y Aduana:** Fletes internacionales y aranceles aduaneros (prescindibles por adquisición comercial en plaza local mediante distribuidor y manufactura aditiva in situ) | Meses 1–4 | $0,00 |
| **Infraestructura de Cómputo:** Servidores de almacenamiento masivo y clústeres de cálculo centralizados de la FCEN-UBA para resguardo de bioimágenes y grandes repositorios genómicos | Meses 1–14 | $0,00 |
| **Insumos y Reactivos:** Reactivos químicos, tampones, portaobjetos especiales y patrones ópticos micrométricos de calibración espacial aportados por laboratorios de FCEN-UBA y Hospital Gutiérrez | Meses 1–14 | $0,00 |
| **Recursos Humanos / Genómica:** Pasantes de la carrera de Licenciatura en Ciencia de Datos (FCEN-UBA) para proyectos curriculares específicos de minería bioinformática y análisis genómico in-silico (WP4.1 y WP4.2) | Meses 3–8 | $0,00 |
| **Servicios Técnicos Mecánicos:** Mecanizado de precisión y rectificado de platina térmica de aluminio realizado por el Taller Mecánico institucional de la FCEN-UBA | Meses 1–4 | $0,00 |
| **Software y Herramientas Computacionales:** Suite completa de código abierto y entornos reproducibles sin costos de licencias comerciales (Python, Micro-Manager, Napari, Ensembl VEP, AlphaFold DB, Docker) | Meses 1–14 | $0,00 |
| **TOTAL APORTES INSTITUCIONALES (USD)** | **Meses 1–14** | **$0,00** |

---

### 4.3 Alineación Temporal con el Cronograma de la Memoria Técnica (`MEMORIA_TECNICA.tex`)

La temporalidad asignada a cada partida presupuestaria se deduce de manera unívoca del diagrama de Gantt y los paquetes de trabajo de la propuesta científica:
1.  **Meses 1 a 2:** Se efectiviza la compra de componentes de hardware electrónico/mecánico ($1.000 USD) para el desarrollo inmediato de la cámara ambiental termostatizada (**WP1.1**, meses 1–4) y se instala la Workstation de desarrollo GPU ($3.000 USD) en FCEN-UBA para disponibilizar el entorno de cómputo previo al inicio del desarrollo algorítmico de **WP2** (mes 2). Comienza la ejecución de las becas de los estudiantes de física (**WP1.1**).
2.  **Meses 3 a 4:** Coincidiendo con la ventana estipulada en el cronograma para la tarea **WP1.2** ("Cámara de alta velocidad", meses 3–4), se adquiere la cámara científica Axiocam 705 mono ($9.000 USD) a través del proveedor local, posibilitando su integración al tren óptico.
3.  **Meses 4 a 5:** En coincidencia con **WP1.3** ("Software de control y estación in situ", meses 4–6), se incorpora la computadora del Hospital Gutiérrez ($2.000 USD) para dejar operativa la estación de adquisición sincronizada antes de la finalización de WP1.
4.  **Meses 5 a 8:** Durante la ejecución de la tarea **WP3.1** ("Curaduría y adquisición de micrografías de TEM", meses 5–8), se contrata el Servicio Integral de Microscopía Electrónica de Transmisión ($2.500 USD) para el procesamiento químico y ultraestructural de las muestras y la obtención de micrografías de alta resolución.
5.  **Meses 1 a 12 y 2 a 13:** Los estipendios de los 3 estudiantes universitarios ($12.600 USD en total) se abonan mensualmente a lo largo de 12 meses, garantizando la dedicación continua durante la construcción instrumental (WP1), el desarrollo de visión por computadora para HSVM (WP2, meses 2–7) y la segmentación con *convpaint* en TEM (WP3, meses 5–11).
6.  **Meses 10 a 14:** Coincidiendo con el despliegue de **WP5** ("Capacitación Médica, Transferencia y Ciencia Abierta", meses 9–14) y específicamente la tarea **WP5.3** ("Liberación en código abierto y difusión científica", meses 11–14), se ejecutan las partidas destinadas a congresos científicos ($3.000 USD) y cargos por publicación Open Access APC ($6.000 USD).
7.  **Meses 1 a 14 (Transversal):** La partida de administración institucional cubre el **overhead institucional regulatorio del 10,0% ($5.000 USD)** —discriminado en 5% ($2.500 USD) para FUNDACEN o Hacienda, 2,5% ($1.250 USD) para la FCEN y 2,5% ($1.250 USD) para el Departamento de Física / Instituto—, junto con las comisiones bancarias por transferencias internacionales de divisas en los 3 desembolsos de la Fundación BBVA ($2.500 USD) y un fondo de contingencia ($3.400 USD). Esta partida se devenga proporcionalmente a lo largo del proyecto, blindando financieramente la ejecución frente a contingencias macroeconómicas o cambiarias y acompañando los tres desembolsos estipulados por la Fundación BBVA (50% anticipo inicial, 40% hito intermedio y 10% tras la aprobación del informe final).



