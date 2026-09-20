# Resumen del Proyecto - Becas Leonardo 2026

**Programa:** Becas Leonardo a Investigadores y Creadores Culturales 2026 (Argentina, Colombia y Perú)  
**Entidad Convocante:** Fundación BBVA  
**Área de Postulación:** Ciencias de la Computación, Ciencia de Datos e Inteligencia Artificial  
**Límite Convocatoria:** Máximo 2.000 caracteres (con espacios incluidos)  
**Institución Sede de Ejecución:** Facultad de Ciencias Exactas y Naturales - Universidad de Buenos Aires (FCEN-UBA)  
**Institución en Colaboración Clínica:** Hospital de Niños Dr. Ricardo Gutiérrez (Buenos Aires, Argentina)  

---

## 1. Título Oficial del Proyecto

### En Español:
> **Desarrollo de Plataforma Computacional Integral de Bioimagen, Visión Artificial y Genómica para el Diagnóstico de la Disquinesia Ciliar Primaria**

### En Inglés:
> **Development of an Integrated Computational Platform Combining Bioimaging, Computer Vision, and Genomics for the Diagnosis of Primary Ciliary Dyskinesia**

---

## 2. Texto Oficial del Resumen para la Plataforma (1.923 caracteres)

> [!IMPORTANT]
> **Conteo exacto verificado:** **1.923 caracteres** (con espacios y saltos de línea incluidos; límite de la convocatoria: máx. 2.000 caracteres).  
> **Enfoque de área:** Ciencias de la Computación, Ciencia de Datos e Inteligencia Artificial, articulando visión por computadora (HSVM), modelos de aprendizaje automático (TEM) y bioinformática genómica (*in-silico*) para resolver el cuello de botella del diagnóstico pediátrico de la DCP.  
> **Alineación con la Memoria Técnica (Secciones 1 y 2):** Resalta la reevaluación epidemiológica de la DCP (antes catalogada como infrecuente hasta que las mejoras diagnósticas revelaron su verdadera prevalencia), datos clínicos locales del Hospital Gutiérrez / SAP y el desglose metodológico por paquetes de trabajo (WPs 1 a 5). Sin citas bibliográficas.

```text
Las Ciencias de la Computación, la Ciencia de Datos y la Inteligencia Artificial revolucionan el diagnóstico biomédico al aportar objetividad, velocidad y reproducibilidad en el análisis de datos complejos. Un caso paradigmático donde estas disciplinas resultan determinantes es la Disquinesia Ciliar Primaria (DCP), enfermedad genética considerada infrecuente (1:15.000 a 1:30.000) hasta que mejoras en el diagnóstico demostraron una prevalencia mucho más alta (al menos 1:7.500). En Argentina, el severo retraso diagnóstico (mediana: 8,8 años en el Hospital Gutiérrez) propicia tratamientos erróneos (52%) y deriva en daño pulmonar irreversible. En menores de 5 años, el óxido nítrico nasal (técnica habitual de screening) es inviable al requerir cooperación activa; por ello, la confirmación clínica depende ineludiblemente de la videomicroscopía de alta velocidad (HSVM), la microscopía electrónica (TEM) y/o la genética, métodos hoy limitados por análisis manuales, subjetivos y sin control térmico.

Para superar estas barreras, este proyecto (FCEN-UBA y Hospital Gutiérrez) implementará una plataforma computacional abierta: 1) estandarización instrumental in situ con cámara de incubación termostatizada y sensor de alta velocidad; 2) flujo de visión artificial para HSVM que cuantifica la frecuencia de batido (CBF) mediante FFT píxel a píxel y el patrón cinético (CBP) por flujo óptico y kimogramas, computando sincronía y disquinesia; 3) bioimagen cuantitativa en TEM mediante aprendizaje automático y perfilometría para clasificar defectos ultraestructurales de dineína; 4) flujo bioinformático in-silico con Ensembl VEP, predictores de IA (AlphaMissense) y AlphaFold para priorizar variantes en >60 genes e integrar reportes moleculares con fenotipos de imagen; y 5) transferencia mediante capacitación a médicos del hospital, protocolos estandarizados y liberación del software en código abierto (Open Science).
```

---

## 3. Matriz de Trazabilidad y Evidencia Documental (Citas de papers/overview.md)

| Parámetro / Frase en el Resumen | Valor / Evidencia | Fuente Bibliográfica (*papers/overview.md*) |
| :--- | :--- | :--- |
| **Prevalencia global de DCP** | $\ge 1:7.500$ nacidos vivos | Robson et al. (2026) *ERJ Open Res*; Collison et al. (2025) *Clin Med* |
| **Distrés respiratorio neonatal** | $\ge 80\%$ en recién nacidos a término | Shapiro et al. (2016) *Pediatr Pulmonol*; Collison et al. (2025) *Clin Med* |
| **Desarrollo de bronquiectasias** | 50% de niños a los 8 años (universal en adultos) | Shapiro et al. (2016) *Pediatr Pulmonol* |
| **Etiología de bronquiectasias en Argentina** | 7% de bronquiectasias no fibroquísticas pediátricas; reversibilidad de dilatación cilíndrica inicial | Smith et al. / Comité Nacional de Neumonología SAP (2020) *Arch Argent Pediatr* |
| **Retraso diagnóstico** | Edad mediana diagnóstica de 5 años; tratamientos inapropiados (corticoides por asma no confirmada) | Collison et al. (2025) *Clin Med*; Robson et al. (2026) *ERJ Open Res* |
| **Deterioro pulmonar progresivo** | Caída anual promedio de FEV1 de ~0,8%/año | Paff et al. (2021) *Int J Mol Sci* |
| **Falsos negativos en TEM y genética** | TEM + genética omiten 20–30% de casos (genes con TEM normal como *DNAH11*) | Bricmont et al. (2021) *Diagnostics*; Collison et al. (2025) *Clin Med* |
| **Estándares DHSV / HSVM (ERS)** | Adquisición a 120–500 fps; requerimiento obligatorio de CBF + CBP | Bricmont et al. (2021) *Diagnostics*; Shapiro et al. (2016) *Pediatr Pulmonol* |
| **Frecuencia ciliar y control térmico** | 10–15 Hz a 37 °C (vs. 6,3–9,0 Hz a 32 °C); la falta de control térmico altera la CBF | Bricmont et al. (2021) *Diagnostics*; Wrona et al. (2025) *J Clin Med* |
| **Subjetividad y automatización** | Evaluación manual subjetiva; necesidad de flujo óptico (*optical flow*) y kymographs | Bricmont et al. (2021) *Diagnostics*; Wrona et al. (2025) *J Clin Med* |
| **Detección ultraestructural en TEM** | Detecta defectos axonémicos en 70–79% de los casos (ODA, IDA+MTD, par central) | Wrona et al. (2025) *J Clin Med*; Shapiro et al. (2016) *Pediatr Pulmonol* |
| **Bioinformática de bajo costo in-silico** | >50 genes causales; *DNAH5* y *DNAI1* (>30% casos); *CCDC39* y *CCDC40* causan fenotipos graves con MTD | Collison et al. (2025) *Clin Med*; Paff et al. (2021) *Int J Mol Sci*; Wrona et al. (2025) *J Clin Med* |
| **Capacitación y Open Science** | Transferencia de software y capacitación médica prescindiendo de ensayos clínicos por autorizaciones éticas | Adecuación estratégica BBVA / Requerimiento de usuario |

---

## 4. Palabras Clave / Keywords

*   **Español:** Bioanálisis de Imágenes, Visión por Computadora, Disquinesia Ciliar Primaria, Videomicroscopía de Alta Velocidad (DHSV/HSVM), Frecuencia de Batido Ciliar (CBF), Patrón de Batido (CBP), Microscopía Electrónica de Transmisión (TEM), Bioinformática In-Silico, Ciencia Abierta, Capacitación Hospitalaria.
*   **Inglés:** Bioimage Analysis, Computer Vision, Primary Ciliary Dyskinesia, Digital High-Speed Videomicroscopy (DHSV), Ciliary Beat Frequency, Ciliary Beat Pattern, Transmission Electron Microscopy, In-Silico Bioinformatics, Open Science, Medical Training.

---

## 5. Versión de Cortesía en Inglés (Reference Translation)

```text
Primary Ciliary Dyskinesia (PCD) is a genetic ciliopathy (prevalence ≥1:7,500; Robson 2026, Collison 2025) causing unexplained neonatal respiratory distress in ≥80% of term newborns and bronchiectasis in 50% by age 8 (Shapiro 2016). In Argentina, PCD accounts for 7% of pediatric non-CF bronchiectasis, where early cylindrical dilation can be reversed with prompt treatment (Smith, SAP 2020). However, severe diagnostic delay (median age: 5 years; Collison 2025) leads to inappropriate treatments (Robson 2026) and lung function decline (FEV1 drop ~0.8%/year; Paff 2021). TEM and genetics miss 20-30% of cases (Bricmont 2021). ERS guidelines mandate digital high-speed videomicroscopy (DHSV) at 120-500 fps and 37 °C (physiological frequency: 10-15 Hz) analyzing both ciliary beat frequency (CBF) and beat pattern (CBP) (Bricmont 2021, Wrona 2025). This project will be based at FCEN-UBA in collaboration with physicians from Dr. Ricardo Gutiérrez Children's Hospital, an important referral center in Argentina with limited optical equipment for DHSV.

The microscope will be upgraded with a high-speed CMOS sensor (>200 fps) and a 37 °C humidified incubation chamber engineered with FCEN-UBA students to prevent thermal ciliary motility impairment (Bricmont 2021). A computer vision pipeline will objectively quantify CBF via FFT and CBP via optical flow and kymographs (Bricmont 2021, Wrona 2025). In TEM bioimages, 9+2 ultrastructure and dynein arms (defective in 70-79%; Wrona 2025) will be measured. In genomics, a low-cost in-silico bioinformatics workflow will prioritize variants in >50 genes (DNAH5, DNAI1, CCDC39, CCDC40; Collison 2025, Paff 2021) from public databases. Finally, since ethical authorizations for clinical validation on patients are not in place, the project will focus on training medical specialists at Hospital Gutiérrez and releasing the software as open-source tools (Open Science).
```
