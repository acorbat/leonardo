# Memoria Técnica del Proyecto - Becas Leonardo 2026

**Convocatoria:** Becas Leonardo a Investigadores y Creadores Culturales 2026 (Argentina, Colombia y Perú)  
**Fundación BBVA**  
**Área Temática:** Ciencias de la Computación, Ciencia de Datos e Inteligencia Artificial  
**Institución Sede de Ejecución:** Facultad de Ciencias Exactas y Naturales - Universidad de Buenos Aires (FCEN-UBA)  
**Institución en Colaboración Clínica:** Hospital de Niños Dr. Ricardo Gutiérrez (Buenos Aires, Argentina)  

---

# TÍTULO DEL PROYECTO:
## Desarrollo de Plataforma Computacional Integral de Bioimagen, Visión Artificial y Genómica para el Diagnóstico de la Disquinesia Ciliar Primaria

---

## 1. Resumen Ejecutivo, Justificación y Planteamiento del Problema

La **Disquinesia Ciliar Primaria (DCP)** es una ciliopatía genética hereditaria, multisistémica y de elevada heterogeneidad clínica, causada por alteraciones congénitas en la ultraestructura y función de las cilias móviles del epitelio respiratorio [1, 2, 3]. En individuos sanos, millones de cilias baten de forma coordinada a una frecuencia fisiológica de entre 10 y 15 Hz a 37 °C, propulsando la capa de moco y asegurando el aclaramiento mucociliar de microorganismos y partículas inhaladas [5, 7]. En pacientes con DCP, la disfunción ciliar interrumpe este mecanismo defensivo primario, desencadenando una cascada fisiopatológica descrita por el "círculo vicioso" de Cole: retención de secreciones, infección bacteriana crónica, inflamación neutrofílica persistente mediada por elastasa e interleucinas, y destrucción progresiva de la pared bronquial [4].

A nivel clínico, la enfermedad se manifiesta desde las primeras horas de vida: más del **80% de los recién nacidos a término presentan dificultad respiratoria neonatal no explicada** que inicia entre las 12 y 24 horas posteriores al parto, frecuentemente acompañada de atelectasias o colapso lobar [2, 3]. Durante la primera infancia, los pacientes sufren de congestión nasal y tos húmeda productiva diaria durante todo el año, otitis media serosa recurrente con efusión en más del 80% de los niños, y neumonías recurrentes en el 80% antes de la edad preescolar [2]. Como consecuencia del daño inflamatorio acumulado, el **50% de los niños desarrolla bronquiectasias a los 8 años de edad**, manifestación que se vuelve universal en la edad adulta [2]. Además, aproximadamente el 50% de los casos presenta defectos de lateralidad (*situs inversus totalis* o síndrome de Kartagener), al menos un 12% exhibe *situs ambiguus* / heterotaxia, entre un 5% y 17% padece cardiopatías congénitas asociadas, y existe una alta prevalencia de subfertilidad en ambos sexos [1, 2, 3]. Estudios genómicos poblacionales recientes han recalculado la prevalencia global de la DCP en **al menos 1:7.500 nacidos vivos**, duplicando o triplicando las estimaciones históricas que la catalogaban erróneamente como una enfermedad ultra-rara [1, 3].

### La Situación en Argentina y el Retraso Diagnóstico
En la República Argentina, las Guías Oficiales del Comité Nacional de Neumonología de la Sociedad Argentina de Pediatría (SAP) sobre bronquiectasias no relacionadas con fibrosis quística (no-FQ) en niños identifican a la **DCP como la causa del 7% de las bronquiectasias pediátricas** diagnosticadas en el país, ubicándose como la cuarta causa identificable tras las secuelas postinfecciosas (19%), las inmunodeficiencias primarias (17%) y la aspiración recurrente por cuerpo extraño (10%) [4]. Las guías de la SAP destacan un principio clínico crítico: **la dilatación bronquial cilíndrica precoz es potencialmente reversible** si se instaura tempranamente kinesioterapia respiratoria y tratamiento antibiótico específico antes de que se consolide la destrucción transmural fibrótica e irreversible [4].

Sin embargo, existe un **grave retraso diagnóstico**, con una edad mediana de confirmación de **5 años**, extendiéndose en numerosos casos hasta la adolescencia o la adultez [3]. Este retraso conlleva intervenciones inadecuadas y perjudiciales, tales como tratamientos prolongados con corticoides inhalados por diagnósticos erróneos de asma refractaria, o incluso lobectomías y resecciones quirúrgicas pulmonares innecesarias antes de alcanzar el diagnóstico de certeza [1, 2]. Asimismo, la falta de diagnóstico precoz acelera el deterioro de la función pulmonar, con una pérdida anual promedio del volumen espiratorio forzado en el primer segundo (**caída del FEV1 de ~0,8% por año**) y un incremento progresivo en la tasa de colonización crónica por patógenos agresivos como *Pseudomonas aeruginosa* [3, 6].

### El Cuello de Botella en el Hospital de Niños Dr. Ricardo Gutiérrez
El **Hospital de Niños Dr. Ricardo Gutiérrez** (CABA) es **un importante centro de referencia en el país** en la atención de patologías respiratorias pediátricas complejas y asiste a numerosos pacientes derivados de diversas provincias con sospecha de DCP. No obstante, las guías internacionales (*ERS / ATS / PCD Foundation*) señalan que el diagnóstico definitivo requiere de una batería técnica compleja [1, 2, 5]:
1.  **Videomicroscopía Digital de Alta Velocidad (DHSV / HSVM):** Estándar de evaluación funcional sobre cepillado nasal (*nasal brush biopsy*), que exige capturar a **120–500 cuadros por segundo (fps)** bajo **estricto control ambiental de temperatura a 37 °C**, evaluando obligatoriamente tanto la Frecuencia de Batido Ciliar (*CBF*) como el Patrón de Batido (*CBP*) [2, 5].
2.  **Microscopía Electrónica de Transmisión (TEM):** Análisis ultraestructural del axonema 9+2 (brazos de dineína, par central y espinas radiales) [2, 7].
3.  **Secuenciación Genética Masiva (NGS):** Paneles multigenéticos que analizan más de 50 genes asociados [3, 7].

Actualmente, el hospital cuenta únicamente con un microscopio óptico estándar de campo claro antiguo, acoplado a una cámara no apta que adquiere a tasas convencionales (≤30 fps), provocando un submuestreo severo (*aliasing*) frente a cilias que baten a 10–15 Hz [5]. Más crítico aún es la **ausencia total de control ambiental**: a temperatura ambiente no controlada (20–22 °C), la frecuencia de batido ciliar se deprime sustancialmente (la CBF es de 6,3–9,0 Hz a 32 °C y de 10–15 Hz a 37 °C) y la muestra se deseca rápidamente en el portaobjetos, induciendo discinesias secundarias y falsos positivos [5, 7]. Finalmente, la evaluación clínica actual es visual y manual, lo que genera una alta subjetividad y dependencia del operador [5].

### La Articulación Interinstitucional: FCEN-UBA y Hospital Gutiérrez
Para superar esta barrera, este proyecto establece una sinergia estratégica orientada a la ingeniería, la computación científica y la capacitación médica:
*   **Sede de Ejecución y Cómputo (FCEN-UBA):** La Facultad de Ciencias Exactas y Naturales de la UBA lidera el desarrollo de los algoritmos de visión artificial, los flujos bioinformáticos *in-silico* de bajo costo, el diseño y fabricación de la cámara ambiental termostatizada y la dirección de estudiantes de grado universitarios.
*   **Colaboración Hospitalaria (Hospital Gutiérrez):** Médicos especialistas de los Servicios de Neumonología y Patología del hospital colaboran en la definición de requisitos clínicos, pruebas del equipamiento óptico en banco de pruebas y reciben la capacitación metodológica para operar la plataforma. Dado que no se cuenta con autorizaciones éticas para investigación clínica experimental en pacientes pediátricos, **el proyecto prescinde de ensayos de validación clínica en seres humanos**, focalizándose en el desarrollo tecnológico, la calibración instrumental y la capacitación del equipo médico.

---

## 2. Estado del Arte, Novedad Científica e Hipótesis

### 2.1 Estado del Arte y Limitaciones de los Métodos Actuales
Las directrices de la *European Respiratory Society* (ERS 2017) recomiendan la videomicroscopía de alta velocidad (DHSV) como prueba diagnóstica confirmatoria de primera línea, con una **sensibilidad de 0,95–1,00 y especificidad de 0,93–0,95**, pero estipulan una **fuerte recomendación de NO utilizar el valor de CBF de manera aislada sin el análisis conjunto del patrón de batido (CBP)** [2, 5, 7]. Esto responde a que mutaciones en genes como *DNAH11* generan cilias con frecuencias normales o hipercinéticas pero con un patrón de batido rígido e inefectivo de baja amplitud angular [5, 7].

Sin embargo, el diagnóstico actual a nivel mundial enfrenta tres limitaciones no resueltas [5]:
1.  **Falsos Negativos de TEM y Genética:** La microscopía electrónica de transmisión (TEM) detecta defectos estructurales en el **70–79% de los casos** (ausencia de brazos de dineína externos [ODA], internos [IDA] o desorganización microtubular [MTD]) [2, 7]. Esto implica que **un 20–30% de los pacientes con DCP confirmada presentan ultraestructura en TEM completamente normal o no concluyente**, incluyendo mutaciones en genes como *DNAH11, DRC2, OFD1, GAS2L2, LRRC56, CFAP57, CFAP221, SPEF2* y *RSPH1* [5, 7]. En estos pacientes, la videomicroscopía funcional (DHSV) es el único método capaz de evidenciar la anomalía motil [5].
2.  **Falta de Estandarización Ambiental:** La literatura demuestra que la CBF varía linealmente con la temperatura (la CBF fisiológica de 10–15 Hz solo se alcanza a 37 °C) y que la estabilidad óptima de la muestra de cepillado nasal se preserva durante 3 a 9 horas a temperaturas controladas de transporte [5]. La ausencia de cámaras de incubación termostatizadas en microscopios clínicos compromete la reproducibilidad diagnóstica.
3.  **Subjetividad del Análisis Manual:** La inspección cualitativa del CBP depende enteramente de la experiencia del observador. Métodos computacionales emergentes como el flujo óptico (*optical flow*), el kymograph digital y la microscopía dinámica diferencial (DDM) han demostrado capacidad para parametrizar la asimetría y coordinación ciliar de forma objetiva, pero requieren validación integrada en software clínico amigable [5].

En el aspecto genético, se conocen más de 50 genes asociados a DCP (>2.000 variantes patogénicas) [3, 7]. Mutaciones en *DNAH5* y *DNAI1* codifican componentes de los ODA y representan más del **30% de todos los casos de DCP** [3]. Por su parte, variantes en *CCDC39* y *CCDC40* provocan defectos combinados de IDA y desorganización microtubular (MTD), cursando con fenotipos clínicos muy agresivos de rápida progresión hacia bronquiectasias severas e insuficiencia respiratoria [6, 7]. Si bien la secuenciación comercial resulta prohibitiva para hospitales públicos, las bases de datos abiertas y herramientas bioinformáticas *in-silico* permiten priorizar y clasificar variantes patogénicas a costo prácticamente nulo.

### 2.2 Novedad y Carácter Innovador
Frente a equipamientos comerciales cerrados cuyo costo supera los USD 150.000, esta propuesta ofrece una innovación de **muy alta costo-efectividad** basada en:
1.  **Instrumentación in situ y control ambiental estricto:** Prototipado y fabricación aditiva de una cámara de incubación para platina con control térmico en lazo cerrado a 37 °C ± 0,3 °C y saturación de humedad (>90%), dirigida por estudiantes de grado de la FCEN-UBA, acoplada a un sensor industrial CMOS de alta velocidad (>200 fps) operado por software abierto (*Micro-Manager*) [5].
2.  **Visión por computadora para DHSV:** Algoritmo que calcula la CBF píxel a píxel mediante Transformada Rápida de Fourier (FFT) y clasifica el CBP utilizando flujo óptico denso (Farnebäck) y kymographs automáticos ortogonales a la pared celular, eliminando el sesgo del observador [5].
3.  **Cuantificación digital de micrografías de TEM:** Segmentación de axonemas 9+2 y perfilometría radial automatizada para medir densidad de brazos de dineína (ODA/IDA) en micrografías electrónicas de archivo [2, 7].
4.  **Bioinformática In-Silico de Bajo Costo:** Pipeline computacional reproducible para la anotación y priorización clínica de variantes patogénicas en >50 genes, minando bases públicas abiertas sin generar costos de secuenciación masiva *de novo* [3, 6, 7].
5.  **Transferencia y Capacitación Médica en Open Science:** Capacitación directa a los especialistas del hospital y liberación íntegra del software bajo código abierto, allanando el camino para futuras fases diagnósticas.

### 2.3 Hipótesis de Trabajo
La integración de instrumentación óptica in situ de bajo costo (cámara ambiental a 37 °C y sensor de alta velocidad) con una suite de visión computacional, análisis bioinformático *in-silico* y capacitación médica interdisciplinaria permitirá dotar al Hospital Gutiérrez de las capacidades técnicas y formativas necesarias para el diagnóstico cuantitativo de la DCP según estándares internacionales, eliminando la subjetividad del operador y sin depender de equipamientos comerciales privativos.

---

## 3. Objetivos

### Objetivo General
Desarrollar, implementar y transferir una plataforma computacional integral de bioimagen, visión artificial y genómica de bajo costo para el diagnóstico de la Disquinesia Ciliar Primaria, ejecutada en la Facultad de Ciencias Exactas y Naturales (UBA) en colaboración con médicos del Hospital de Niños Dr. Ricardo Gutiérrez.

### Objetivos Específicos
1.  **OE1:** Diseñar, construir y calibrar una cámara ambiental con control térmico a 37 °C y humedad relativa saturada (>90%), acoplando un sensor digital CMOS industrial de alta velocidad (≥200 fps) al microscopio óptico del hospital mediante software de código abierto (*Micro-Manager*).
2.  **OE2:** Desarrollar un pipeline computacional de visión artificial en Python para la segmentación del epitelio ciliado, cálculo espectral de CBF píxel a píxel por FFT y cuantificación de descriptores cinéticos de CBP mediante flujo óptico y kymographs.
3.  **OE3:** Desarrollar un algoritmo de análisis digital de bioimágenes de Microscopía Electrónica de Transmisión (TEM) para la cuantificación objetiva de la geometría axonémica 9+2 y la integridad de los brazos de dineína externos e internos (ODA/IDA).
4.  **OE4:** Implementar un flujo bioinformático *in-silico* de bajo costo para la priorización y anotación funcional de variantes en genes causales de DCP (>50 genes) a partir de repositorios genómicos públicos abiertos, correlacionando los perfiles moleculares con los fenotipos cinéticos (DHSV) y ultraestructurales (TEM).
5.  **OE5:** Capacitar a los médicos especialistas del Hospital Gutiérrez y liberar el software como herramienta de código abierto (*Open Science*).

---

## 4. Metodología y Plan de Trabajo (Work Packages)

El proyecto se estructura en **5 Paquetes de Trabajo (WPs)** a lo largo de **18 meses**:

```mermaid
gantt
    title Cronograma de Ejecución - Becas Leonardo 2026 (18 Meses)
    dateFormat  YYYY-MM
    axisFormat  %m
    section WP1 Hardware & Adquisición
    Diseño y calibración cámara ambiental 37°C (FCEN-UBA): 2027-03, 4M
    Integración sensor CMOS alta velocidad (>200 fps)  : 2027-05, 3M
    Puesta a punto in situ en el microscopio            : 2027-06, 2M
    section WP2 Algoritmos DHSV
    Preprocesamiento y segmentación ciliar activa       : 2027-06, 4M
    Cuantificación CBF (FFT) y CBP (Flujo Óptico)      : 2027-08, 5M
    Interfaz gráfica asistencial (PyQt / Napari)        : 2027-11, 4M
    section WP3 Bioimágenes TEM
    Digitalización y curaduría de micrografías axonema  : 2027-09, 4M
    Algoritmo de cuantificación 9+2 y dineína (ODA/IDA) : 2027-11, 5M
    section WP4 Bioinformática In-Silico
    Pipeline in-silico y minería en bases abiertas     : 2027-12, 5M
    Priorización funcional de variantes en >50 genes    : 2028-03, 4M
    section WP5 Capacitación & Open Science
    Talleres de capacitación a médicos especialistas    : 2028-02, 4M
    Liberación de software abierto y documentación      : 2028-05, 4M
    Publicaciones científicas e informe final BBVA      : 2028-07, 2M
```

---

### WP1: Modernización Instrumental in-situ y Control Ambiental (Meses 1-6)
*   **Sede:** Laboratorio en FCEN-UBA / Instalación en Hospital Gutiérrez.
*   **Responsable:** Investigador Postulante (dirigiendo a 2 estudiantes avanzados de grado de FCEN-UBA / Ingeniería).
*   **Metodología:**
    1.  *Cámara de incubación ambiental:* Modelado en software CAD de una cámara cerrada adaptada a la platina. Chasis fabricado por manufactura en impresión 3D. Implementación de circuito de control en lazo cerrado PID con microcontrolador ESP32 o Arduino y sensores térmicos, garantizando **37 °C ± 0,3 °C** en la muestra para neutralizar el sesgo térmico (donde la CBF desciende a 6,3–9,0 Hz a 32 °C o menos) [5, 7]. Reservorio de humidificación para humedad relativa >90%, evitando la desecación durante la observación (ventana de estabilidad celular de 3 a 9 horas) [5].
    2.  *Sensor CMOS de alta velocidad:* Montaje de cámara industrial monocromática USB 3.0 con obturador global (*global shutter*), velocidad de muestreo de **200 a 400 fps** a resolución útil diagnóstica (800x600 px), y lente de reducción óptica C-mount acoplada al puerto trinocular del microscopio, cumpliendo con el rango de 120–500 fps estipulado por las guías [5].
    3.  *Software de control:* Configuración de adquisición en **Micro-Manager** / Python para grabación continua en memoria RAM de alta velocidad.
*   **Entregables:** Cámara ambiental calibrada a 37 °C; microscopio adaptado adquiriendo video a >200 fps.

---

### WP2: Pipeline Computacional de Visión Artificial para DHSV (Meses 4-12)
*   **Sede:** FCEN-UBA.
*   **Responsable:** Investigador Postulante.
*   **Metodología:**
    1.  *Preprocesamiento:* Corrección de desplazamiento de tejido mediante correlación de fase y realce de bordes.
    2.  *Segmentación automatizada:* Detección de regiones epiteliales activas mediante varianza temporal píxel a píxel, discriminando moco estático, eritrocitos y detritos celulares.
    3.  *Cuantificación de CBF (Frecuencia):* Análisis espectral de potencia mediante **Transformada Rápida de Fourier (FFT)** aplicada a la serie temporal de intensidad píxel a píxel. Generación de mapas de calor de frecuencia dominante (rango fisiológico: 10–15 Hz a 37 °C), CBF media y áreas inmóviles (<4 Hz) [5, 7].
    4.  *Cuantificación de CBP (Patrón de Batido):* Conforme al mandato ERS de no evaluar CBF aisladamente [2, 5], se calculará el campo vectorial de velocidad mediante **flujo óptico denso (Farnebäck)** y se generarán kymographs digitales automáticos perpendiculares a la membrana para medir: amplitud angular de batido, asimetría de carrera efectiva vs. recuperación (*effective/recovery stroke*), e índice de disquinesia ciliar (CDI) para clasificar movimientos normales, rígidos (*DNAH11*), rotacionales (*HYDIN, RSPH*) o inmovilidad completa (*DNAH5, DNAI1*) [5, 7].
*   **Entregables:** Módulo de visión por computadora en Python con interfaz gráfica (GUI en PyQt/Napari) para uso médico.

---

### WP3: Procesamiento Cuantitativo de Bioimágenes en TEM (Meses 6-14)
*   **Sede:** FCEN-UBA en articulación con el Servicio de Patología del Hospital Gutiérrez.
*   **Responsable:** Investigador Postulante.
*   **Metodología:**
    1.  *Curaduría y digitalización:* Digitalización calibrada de micrografías electrónicas de archivo de cortes transversales de axonemas ciliares respiratorios.
    2.  *Segmentación geométrica del axonema:* Algoritmo basado en transformada circular de Hough para localizar el par central de microtúbulos simples y los 9 dobletes periféricos de microtúbulos A y B (geometría canónica 9+2) [2, 7].
    3.  *Cuantificación de brazos de dineína (ODA/IDA):* Perfilometría radial de intensidad óptica normalizada en las coordenadas del microtúbulo A para cuantificar objetivamente la presencia o ausencia de brazos de dineína externos (ODA) e internos (IDA). Aplicación de promediado de partículas 2D (*sub-axonemal averaging*) para optimizar la relación señal-ruido [2, 7].
*   **Entregables:** Algoritmo validado de cuantificación ultraestructural con reporte automatizado de integridad axonémica.

---

### WP4: Bioinformática In-Silico de Bajo Costo y Caracterización de Variantes Genéticas (Meses 8-16)
*   **Sede:** FCEN-UBA.
*   **Responsable:** Investigador Postulante.
*   **Metodología:**
    Con el fin de garantizar una **estrategia de bajo costo que prescinda de costosos reactivos o servicios de secuenciación masiva *de novo***, este paquete de trabajo se desarrollará íntegramente mediante flujos computacionales *in-silico*, minería de repositorios genómicos de acceso abierto y herramientas de software libre:
    1.  *Minería en repositorios genómicos abiertos:* Recopilación y curaduría sistemática de variantes patogénicas y de significado incierto (VUS) en el catálogo de **más de 50 genes asociados a DCP** [3, 7] desde bases de datos públicas internacionales y regionales (ClinVar, gnomAD v4, 1000 Genomes, Ensembl y LatinGen / ABraOM para poblaciones latinoamericanas).
    2.  *Pipeline automatizado de anotación y priorización liviana:* Implementación de un flujo en Python / Bash que ejecuta la anotación funcional mediante Variant Effect Predictor (VEP) de Ensembl y SnpEff, combinando herramientas de predicción de patogenicidad *in-silico* de acceso libre (CADD, REVEL, AlphaMissense). El pipeline prioriza variantes en genes ODA mayores (*DNAH5, DNAI1*, responsables de >30% de casos) [3], genes con ultraestructura normal en TEM (*DNAH11*) [5, 7] y genes asociados a fenotipos agresivos con desorganización microtubular (*CCDC39, CCDC40*) [6, 7].
    3.  *Análisis de variantes de parada prematura (PTC) y modelado estructural:* Identificación de variantes *nonsense* y frameshift que generan codones de terminación prematura (PTC, presentes en hasta un 28% de pacientes) [6], evaluando el impacto conformacional en los complejos axonémicos mediante bases de estructuras predichas (AlphaFold DB / Foldseek).
    4.  *Generador de reportes clínicos moleculares de código abierto:* Desarrollo de un módulo computacional liviano que permita a los profesionales ingresar archivos de variantes estándar (VCF) y obtener un reporte automatizado estandarizado bajo criterios ACMG/AMP sin costos de licenciamiento privativo.
*   **Entregables:** Pipeline bioinformático *in-silico* de bajo costo publicado; catálogo estructurado y anotado de variantes en >50 genes de DCP; módulo de generación automatizada de reportes clínicos moleculares.

---

### WP5: Capacitación a Médicos Especialistas del Hospital Gutiérrez y Liberación en Acceso Abierto (Meses 12-18)
*   **Sede:** Hospital Gutiérrez / FCEN-UBA.
*   **Responsable:** Investigador Postulante.
*   **Metodología:**
    Este paquete de trabajo orienta sus actividades a la transferencia tecnológica, la capacitación profesional interdisciplinaria y la consolidación de la ciencia abierta (*Open Science*):
    1.  *Talleres de capacitación médica especializada:* Dictado de jornadas teórico-prácticas y talleres de entrenamiento dirigidos a médicos neumonólogos, patólogos y bioquímicos del Hospital de Niños Dr. Ricardo Gutiérrez. Los módulos comprenderán la operación de la cámara ambiental termostatizada a 37 °C, la adquisición sincrónica de videomicroscopía a alta velocidad (>200 fps) en el microscopio óptico y la correcta interpretación de los reportes automatizados de CBF, CBP y métricas axonémicas de TEM [1, 2, 5].
    2.  *Protocolos operativos estándar (SOP) y guías asistenciales:* Elaboración y transferencia de manuales ilustrados de buenas prácticas basados en las recomendaciones de consenso internacional (ERS / PCD Foundation) para la toma adecuada de cepillado nasal y su mantenimiento térmico ex vivo [1, 2, 5].
    3.  *Liberación del software en código abierto (Open Science):* Publicación de la suite computacional completa en GitHub bajo licencia libre (GPL/MIT), con imágenes de contenedor Docker y entornos Conda documentados para garantizar la instalación y reproducibilidad sin barreras económicas en cualquier institución pública de salud de la región.
    4.  *Difusión científica y memoria institucional:* Redacción y envío de dos artículos científicos sobre la metodología computacional e instrumentación abierta a revistas internacionales indexadas de acceso abierto (Q1/Q2); presentación de resultados en congresos de microscopía y neumonología; elaboración de la memoria final para la Fundación BBVA.
*   **Entregables:** Personal médico y técnico del Hospital Gutiérrez formalmente capacitado; manuales de procedimiento y guías de buenas prácticas transferidos; suite de software libre publicada en GitHub; 2 manuscritos científicos internacionales enviados; informe final de la Beca Leonardo.

---

## 5. Cronograma de Hitos y Entregables (18 Meses)

| Mes | Hito Clave / Entregable | Paquete | Respaldo en Literatura |
| :---: | :--- | :---: | :--- |
| **M03** | Prototipo de cámara ambiental termostatizada (37 °C) calibrado en laboratorio de FCEN-UBA. | WP1 | Requisito de temperatura fisiológica [5, 7] |
| **M06** | Sensor CMOS de alta velocidad (>200 fps) adaptado al microscopio del Hospital Gutiérrez con Micro-Manager. | WP1 | Estándar ERS de muestreo a 120–500 fps [5] |
| **M09** | Pipeline de visión por computadora para cálculo de CBF (FFT) y CBP (flujo óptico) operativo en videos piloto. | WP2 | Análisis conjunto mandatario CBF+CBP [2, 5] |
| **M11** | Interfaz gráfica interactiva (GUI en PyQt/Napari) validada para uso por el personal médico asistencial. | WP2 | Eliminación de subjetividad y sesgo del operador [5] |
| **M13** | Algoritmo de procesamiento cuantitativo de micrografías de TEM (axonema 9+2 y brazos de dineína) calibrado. | WP3 | Detección objetiva de ODA/IDA en TEM [2, 7] |
| **M15** | Pipeline bioinformático *in-silico* de bajo costo ejecutado y catálogo de variantes en >50 genes completado. | WP4 | Minería en bases genómicas abiertas [3, 6, 7] |
| **M17** | Talleres de capacitación a médicos especialistas del Hospital Gutiérrez y transferencia de manuales completados. | WP5 | Estándares de formación y buenas prácticas [1, 4] |
| **M18** | Liberación de código abierto en GitHub, remisión de artículos científicos y reporte final a Fundación BBVA. | WP5 | Ciencia abierta y difusión preceptiva BBVA [1, 5] |

---

## 6. Factibilidad, Gestión de Riesgos y Plan de Mitigación

*   **Factibilidad Institucional y Marco Ético Simplificado:** La propuesta posee una factibilidad institucional óptima gracias a la capacidad computacional y de instrumentación de la FCEN-UBA y a la estrecha articulación con los médicos del Hospital Gutiérrez. Al haberse excluido la realización de ensayos clínicos prospectivos o experimentales en pacientes pediátricos, el proyecto no enfrenta barreras bioéticas, objeciones regulatorias ni retrasos en comités de ética que condicionen su ejecución. La calibración del sistema óptico, la cámara ambiental y los algoritmos se llevará a cabo en banco de pruebas con preparaciones de referencia in vitro, especímenes de control y datos retrospectivos anonimizados de repositorios públicos, enfocando la transferencia hacia la capacitación profesional de los médicos del hospital y la liberación de software abierto [1, 4].
*   **Factibilidad Técnica del Postulante:** El postulante posee trayectoria comprobada en bioanálisis de imágenes, microscopía óptica y electrónica, y bioinformática traslacional, con experiencia previa en desarrollo de software científico y dirección de estudiantes universitarios.
*   **Matriz de Riesgos y Mitigaciones:**
    1.  *Riesgo: Demoras aduaneras en la importación del sensor CMOS o componentes electrónicos.*  
        *Mitigación:* Se iniciarán los trámites de importación en el Mes 1. Se dispone provisionalmente de cámaras industriales de laboratorios de la FCEN-UBA para avanzar en el desarrollo de los algoritmos de visión artificial.
    2.  *Riesgo: Heterogeneidad en formatos de video y bioimágenes de archivo.*  
        *Mitigación:* El algoritmo de preprocesamiento (WP2) incorpora conversores de formato universales (TIFF, AVI, HDF5) y normalizadores de histograma temporal para procesar datos independientemente del dispositivo de captura.
    3.  *Riesgo: Dificultad para clasificar variantes genéticas de significado incierto (VUS).*  
        *Mitigación:* El pipeline bioinformático *in-silico* (WP4) integra múltiples predictores ortogonales de patogenicidad y modelos estructurales basados en AlphaFold DB para brindar una clasificación multifactorial robusta según guías ACMG/AMP.

---

## 7. Impacto Esperado, Beneficio Social y Transferencia Sanitaria

1.  **Impacto en la Salud Infantil y Transferencia Asistencial:** La capacitación brindada a los médicos especialistas del Hospital Gutiérrez y la provisión de una estación de videomicroscopía termostatizada y calibrada deja instalada en el hospital la capacidad técnica para que, una vez tramitadas las autorizaciones correspondientes en etapas posteriores, los profesionales dispongan de herramientas objetivas para un diagnóstico precoz, permitiendo instaurar oportunamente kinesioterapia respiratoria y tratamiento antibiótico que reviertan las dilataciones cilíndricas iniciales y prevengan el daño pulmonar permanente (bronquiectasias irreversibles) [1, 2, 4, 6].
2.  **Soberanía Tecnológica en Salud Pública:** Se demuestra que la conjunción entre la universidad pública (FCEN-UBA) y el hospital pediátrico permite modernizar instrumental preexistente a una fracción del costo de equipos comerciales cerrados importados, creando capacidad diagnóstica local sustentable.
3.  **Aporte a la Genómica Médica de Código Abierto:** Generación de un flujo bioinformático reproducible y de libre uso para la anotación y priorización de variantes de DCP en bases públicas, enriqueciendo los recursos bioinformáticos disponibles para la región [3, 7].
4.  **Ciencia Abierta y Formación de Recursos Humanos:** Formación de estudiantes de grado universitarios en ingeniería biomédica y computación, capacitación continua de médicos del hospital y liberación del software en acceso abierto para cualquier hospital público de América Latina.
5.  **Reconocimiento Institucional Preceptivo:** Todos los resultados, publicaciones científicas y presentaciones mencionarán de forma explícita: *«Proyecto realizado con la Beca Leonardo de la Fundación BBVA 2026. Argentina»*.

---

## 8. Referencias Bibliográficas (Fuentes del Proyecto)

1.  **Robson, E. A., Spoletini, G., Bercusson, A., Carr, S. B., Carroll, M., Dexter, K., Dixon, L., Hogg, C., Jones, A., Kenia, P., Loebinger, M., Lucas, J. S., Moya, E., O’Callaghan, C., Patel, D., Peckham, D. G., Range, S., & Walker, W. T. (2026).** Primary ciliary dyskinesia: a national expert consensus statement on standards of care. *ERJ Open Research*, DOI: 10.1183/23120541.00892-2025.
2.  **Shapiro, A. J., Zariwala, M. A., Ferkol, T., Davis, S. D., Sagel, S. D., Dell, S. D., Rosenfeld, M., Olivier, K. N., Milla, C., Daniel, S. J., Kimple, A. J., Manion, M., Knowles, M. R., & Leigh, M. W. (2016).** Diagnosis, monitoring, and treatment of primary ciliary dyskinesia: PCD foundation consensus recommendations based on state of the art review. *Pediatric Pulmonology*, 51(2), 115–132. DOI: 10.1002/ppul.23304.
3.  **Collison, R., Hyatali, S. A., Kamenova, A., Rashed, A., Riley, D., Kumar, K., Stowell, J. M., & Loebinger, M. R. (2025).** Primary ciliary dyskinesia: aetiology, diagnosis and clinical management. *Clinical Medicine*, 25(1), 100288. DOI: 10.1016/j.clinme.2024.100288.
4.  **Comité Nacional de Neumonología, Sociedad Argentina de Pediatría (Smith, S., Salim, M., Bujedo, E., Martinchuk Migliazza, G., Tognini, C., Nociti, Y., Garetto, S., Olguín Ciancio, M., Pinto, F., et al.) (2020).** Bronquiectasias no relacionadas con fibrosis quística en niños: guías de diagnóstico, seguimiento y tratamiento. *Archivos Argentinos de Pediatría*, 118(Supl 1), S1–S24. DOI: 10.5546/aap.2020.S1.
5.  **Bricmont, N., Alexandru, M., Louis, B., Papon, J.-F., & Kempeneers, C. (2021).** Ciliary videomicroscopy: a long beat from the European Respiratory Society guidelines to the recognition as a confirmatory test for primary ciliary dyskinesia. *Diagnostics*, 11(4), 666. DOI: 10.3390/diagnostics11040666.
6.  **Paff, T., Omran, H., Nielsen, K. G., & Haarman, E. G. (2021).** Current and future treatments in primary ciliary dyskinesia. *International Journal of Molecular Sciences*, 22(18), 9834. DOI: 10.3390/ijms22189834.
7.  **Wrona, J., Krupa, Z., Zawadzka, M., Rydzek, J., Dorobisz, K., & Bania, J. (2025).** Primary ciliary dyskinesia—current diagnostic and therapeutic approach. *Journal of Clinical Medicine*, 14(3), 856. DOI: 10.3390/jcm14030856.
