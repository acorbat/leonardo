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

## 2. Texto Oficial del Resumen para la Plataforma (1.908 caracteres)

> [!IMPORTANT]
> **Conteo exacto verificado:** **1.908 caracteres** (con espacios y saltos de línea incluidos).  
> **Trazabilidad bibliográfica:** Cada cifra, rango fisiológico, parámetro diagnóstico y concepto clínico proviene estrictamente de la literatura de referencia (*papers/overview.md*: Robson et al., 2026; Shapiro et al., 2016; Collison et al., 2025; Smith et al. / SAP, 2020; Bricmont et al., 2021; Paff et al., 2021; Wrona et al., 2025).

```text
La Disquinesia Ciliar Primaria (DCP) es una ciliopatía genética (prevalencia ≥1:7.500; Robson 2026, Collison 2025) que causa distrés respiratorio neonatal en ≥80% de neonatos y bronquiectasias en 50% a los 8 años (Shapiro 2016). En Argentina causa el 7% de las bronquiectasias no-FQ pediátricas, donde la dilatación cilíndrica inicial puede revertirse con tratamiento precoz (Smith, SAP 2020). No obstante, existe un severo retraso diagnóstico (mediana: 5 años; Collison 2025) que genera tratamientos inadecuados (Robson 2026) y pérdida de función pulmonar (caída FEV1 ~0,8%/año; Paff 2021). TEM y genética omiten 20-30% de casos (Bricmont 2021). Las guías ERS exigen videomicroscopía de alta velocidad (DHSV) a 120-500 fps y 37 °C (frecuencia fisiológica: 10-15 Hz) evaluando frecuencia (CBF) y patrón de batido (CBP) (Bricmont 2021, Wrona 2025). El proyecto se radicará en FCEN-UBA en colaboración con médicos del Hospital de Niños Dr. Ricardo Gutiérrez, un importante centro de referencia en el país con equipamiento óptico limitado para DHSV.

Se modernizará in situ el microscopio acoplando un sensor CMOS de alta velocidad (>200 fps) y diseñando —con estudiantes de FCEN-UBA— una cámara de incubación con control térmico (37 °C) y de humedad para evitar la alteración del batido ciliar (Bricmont 2021). Se desarrollará un pipeline de visión por computadora para segmentación automática y cuantificación de CBF por FFT píxel a píxel y de CBP por flujo óptico y kymographs, superando la subjetividad del análisis manual (Bricmont 2021, Wrona 2025). En bioimágenes de TEM se medirá cuantitativamente la arquitectura 9+2 y brazos de dineína (defectos en 70-79%; Wrona 2025). Finalmente, un pipeline bioinformático priorizará variantes en >50 genes (DNAH5, DNAI1, CCDC39, CCDC40; Collison 2025, Paff 2021) para caracterizar la epidemiología molecular en Argentina. El software se liberará en código abierto.
```

---

## 3. Matriz de Trazabilidad y Evidencia Documental (Citas de papers/overview.md)

| Parámetro / Frase en el Resumen | Valor / Evidencia | Fuente Bibliográfica (*papers/overview.md*) |
| :--- | :--- | :--- |
| **Prevalencia global de DCP** | ≥ 1:7.500 nacidos vivos | Robson et al. (2026) *ERJ Open Res*; Collison et al. (2025) *Clin Med* |
| **Distrés respiratorio neonatal** | ≥ 80% en recién nacidos a término | Shapiro et al. (2016) *Pediatr Pulmonol*; Collison et al. (2025) *Clin Med* |
| **Desarrollo de bronquiectasias** | 50% de niños a los 8 años (universal en adultos) | Shapiro et al. (2016) *Pediatr Pulmonol* |
| **Etiología de bronquiectasias en Argentina** | 7% de bronquiectasias no fibroquísticas pediátricas; reversibilidad de dilatación cilíndrica inicial | Smith et al. / Comité Nacional de Neumonología SAP (2020) *Arch Argent Pediatr* |
| **Retraso diagnóstico** | Edad mediana diagnóstica de 5 años; tratamientos inapropiados (corticoides por asma no confirmada) | Collison et al. (2025) *Clin Med*; Robson et al. (2026) *ERJ Open Res* |
| **Deterioro pulmonar progresivo** | Caída anual promedio de FEV1 de ~0,8%/año | Paff et al. (2021) *Int J Mol Sci* |
| **Falsos negativos en TEM y genética** | TEM + genética omiten 20–30% de casos (genes con TEM normal como *DNAH11*) | Bricmont et al. (2021) *Diagnostics*; Collison et al. (2025) *Clin Med* |
| **Estándares DHSV / HSVM (ERS)** | Adquisición a 120–500 fps; requerimiento obligatorio de CBF + CBP | Bricmont et al. (2021) *Diagnostics*; Shapiro et al. (2016) *Pediatr Pulmonol* |
| **Frecuencia ciliar y control térmico** | 10–15 Hz a 37 °C (vs. 6,3–9,0 Hz a 32 °C); la falta de control térmico altera la CBF | Bricmont et al. (2021) *Diagnostics*; Wrona et al. (2025) *J Clin Med* |
| **Subjetividad y automatización** | Evaluación manual subjetiva; necesidad de flujo óptico (*optical flow*) y kymographs | Bricmont et al. (2021) *Diagnostics*; Wrona et al. (2025) *J Clin Med* |
| **Sensibilidad diagnóstica de HSVM** | 95–100% sensibilidad y 91–96% especificidad (CBF + CBP combinados) | Bricmont et al. (2021) *Diagnostics*; Wrona et al. (2025) *J Clin Med* |
| **Detección ultraestructural en TEM** | Detecta defectos axonémicos en 70–79% de los casos (ODA, IDA+MTD, par central) | Wrona et al. (2025) *J Clin Med*; Shapiro et al. (2016) *Pediatr Pulmonol* |
| **Base genética y genes agresivos** | >50 genes causales; *DNAH5* y *DNAI1* (>30% casos); *CCDC39* y *CCDC40* causan fenotipos graves con MTD | Collison et al. (2025) *Clin Med*; Paff et al. (2021) *Int J Mol Sci*; Wrona et al. (2025) *J Clin Med* |

---

## 4. Palabras Clave / Keywords

*   **Español:** Bioanálisis de Imágenes, Visión por Computadora, Disquinesia Ciliar Primaria, Videomicroscopía de Alta Velocidad (HSVM/DHSV), Frecuencia de Batido Ciliar (CBF), Patrón de Batido (CBP), Microscopía Electrónica de Transmisión (TEM), Bioinformática Médica.
*   **Inglés:** Bioimage Analysis, Computer Vision, Primary Ciliary Dyskinesia, Digital High-Speed Videomicroscopy (DHSV), Ciliary Beat Frequency, Ciliary Beat Pattern, Transmission Electron Microscopy, Translational Bioinformatics.

---

## 5. Versión de Cortesía en Inglés (Reference Translation)

```text
Primary Ciliary Dyskinesia (PCD) is a genetic ciliopathy (prevalence ≥1:7,500; Robson 2026, Collison 2025) causing unexplained neonatal respiratory distress in ≥80% of term newborns and bronchiectasis in 50% by age 8 (Shapiro 2016). In Argentina, PCD accounts for 7% of pediatric non-CF bronchiectasis, where early cylindrical dilation can be reversed with prompt treatment (Smith, SAP 2020). However, severe diagnostic delay (median age: 5 years; Collison 2025) leads to inappropriate treatments (Robson 2026) and lung function decline (FEV1 drop ~0.8%/year; Paff 2021). TEM and genetics miss 20-30% of cases (Bricmont 2021). ERS guidelines mandate digital high-speed videomicroscopy (DHSV) at 120-500 fps and 37 °C (physiological frequency: 10-15 Hz) analyzing both ciliary beat frequency (CBF) and beat pattern (CBP) (Bricmont 2021, Wrona 2025). This project will be based at FCEN-UBA in collaboration with physicians from Dr. Ricardo Gutiérrez Children's Hospital, an important referral center in Argentina with limited optical equipment for DHSV.

The optical microscope will be upgraded in situ by integrating a high-speed CMOS sensor (>200 fps) and engineering—mentoring FCEN-UBA undergraduate students—an incubation chamber with thermal (37 °C) and humidity control to prevent ciliary motility impairment (Bricmont 2021). A computer vision pipeline will be developed for automated segmentation and quantification of CBF via pixel-wise FFT and CBP via optical flow and kymographs, eliminating manual subjectivity (Bricmont 2021, Wrona 2025). In TEM bioimages, 9+2 ultrastructure and dynein arms (defective in 70-79%; Wrona 2025) will be quantitatively measured. Finally, a bioinformatics workflow will prioritize variants across >50 genes (DNAH5, DNAI1, CCDC39, CCDC40; Collison 2025, Paff 2021) to characterize molecular epidemiology in Argentina. The software will be released as open source.
```
