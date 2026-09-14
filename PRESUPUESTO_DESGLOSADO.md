# Presupuesto Total Bruto Desglosado - Becas Leonardo 2026

**Convocatoria:** Becas Leonardo a Investigadores y Creadores Culturales 2026 (Argentina, Colombia y Perú)  
**Entidad Convocante:** Fundación BBVA  
**Solicitante:** Investigador Postulante  
**Proyecto:** *Desarrollo de Plataforma Computacional Integral de Bioimagen, Visión Artificial y Genómica para el Diagnóstico de la Disquinesia Ciliar Primaria*  
**Institución Sede de Ejecución:** Facultad de Ciencias Exactas y Naturales - Universidad de Buenos Aires (FCEN-UBA)  
**Institución en Colaboración Clínica:** Hospital de Niños Dr. Ricardo Gutiérrez (Buenos Aires, Argentina)  
**Moneda de Presentación:** Dólares Estadounidenses (USD)  
**Plazo de Ejecución:** 18 meses  
**Monto Total Solicitado:** **USD 50.000,00** (Cincuenta mil dólares brutos)  

---

## 1. Tabla Resumen por Rubro Presupuestario

| N° | Rubro de Gasto | Monto Bruto (USD) | % del Total |
| :---: | :--- | :---: | :---: |
| **1** | **Hardware e Instrumentación Óptica in situ** | $17.200,00 | 34,4% |
| **2** | **Equipamiento Informático, Almacenamiento y Cómputo** | $6.800,00 | 13,6% |
| **3** | **Reactivos, Insumos de Laboratorio y Muestreo Clínico** | $4.600,00 | 9,2% |
| **4** | **Formación de RRHH, Estipendios Estudiantiles y Asistencia Técnica** | $10.900,00 | 21,8% |
| **5** | **Difusión Científica, Publicaciones Open Access y Congresos** | $5.500,00 | 11,0% |
| **6** | **Costos de Administración Institucional, Retenciones y Bancarios** | $5.000,00 | 10,0% |
| | **TOTAL BRUTO GENERAL:** | **$50.000,00** | **100,0%** |

---

## 2. Desglose Detallado por Ítem y Justificación Técnica

### Rubro 1: Hardware e Instrumentación Óptica in situ ($17.200,00 USD)
*Este rubro moderniza el equipamiento óptico utilizado para el diagnóstico en colaboración con los médicos del Hospital Gutiérrez, dotándolo de capacidades de videomicroscopía de alta velocidad y control ambiental estricto.*

1.  **Cámara CMOS Industrial de Alta Velocidad (Global Shutter):**
    *   *Descripción:* Sensor CMOS monocromático de alta sensibilidad cuántica y bajo ruido de lectura, con montura C-mount estándar, conexión USB 3.0 / GigE industrial. Capaz de adquirir a ≥200-400 fps en el área de interés diagnóstica (ROI), indispensable para muestrear el batido ciliar (>10-16 Hz) cumpliendo el criterio de Nyquist sin *aliasing* ni distorsión por persiana (*rolling shutter*).
    *   *Monto:* **$8.200,00 USD**
2.  **Componentes para Cámara Ambiental Termostatizada (37 °C) y Control de Humedad:**
    *   *Descripción:* Platina calefactora transparente/metálica con resistencia integrada de bajo voltaje, controlador industrial de lazo cerrado (PID) con resolución de 0.1 °C, termorresistencias de platino (Pt100 de grado médico), sensor digital de humedad relativa, microcontrolador para adquisición de datos (ESP32), fuente de poder estabilizada y bobinas de filamento técnico PETG de grado médico para fabricación aditiva (impresión 3D) del chasis hermético.
    *   *Monto:* **$3.300,00 USD**
3.  **Adaptador Óptico C-Mount de Reducción y Acoples Mecánicos:**
    *   *Descripción:* Lente de acoplamiento óptico 0.5x / 0.63x de alta transmisión lumínica para adaptar la cámara al puerto trinocular del microscopio, optimizando el campo visual y la coincidencia con el tamaño del sensor.
    *   *Monto:* **$1.200,00 USD**
4.  **Costos de Importación, Fletes Internacionales, Seguros y Aranceles Aduaneros:**
    *   *Descripción:* Gastos de envío internacional courier (puerta a puerta), despacho aduanero y tributos de nacionalización en Argentina para el equipamiento óptico y sensores no producidos localmente.
    *   *Monto:* **$4.500,00 USD**

---

### Rubro 2: Equipamiento Informático, Almacenamiento y Cómputo ($6.800,00 USD)
*El procesamiento de video a alta tasa de cuadros sin compresión genera flujos de datos intensivos (~400 MB/s) que requieren hardware de computación de alto rendimiento instalado en la sede del proyecto (FCEN-UBA).*

1.  **Workstation de Adquisición y Procesamiento de Bioimágenes:**
    *   *Descripción:* Estación de trabajo equipada con procesador multinúcleo de alto rendimiento (ej. AMD Ryzen 9 / Intel Core i9), 64 GB de memoria RAM DDR5 de alta velocidad (para albergar secuencias de video en memoria volátil durante la captura sincrónica), arreglo en RAID0 de 2 unidades NVMe PCIe 4.0 de 2 TB para streaming de escritura sin pérdida de cuadros, y placa de procesamiento gráfico dedicada (GPU NVIDIA RTX con núcleos Tensor) para aceleración de algoritmos de visión por computadora y flujo óptico.
    *   *Monto:* **$4.600,00 USD**
2.  **Sistema de Almacenamiento Masivo y Backup Redundante (NAS):**
    *   *Descripción:* Servidor de almacenamiento en red (NAS de 4 bahías configurado en RAID5 con discos duros empresariales de alta durabilidad, capacidad neta útil de 24 TB) para resguardo centralizado, backup y versionado de gigabytes de videomicroscopía, micrografías de TEM y archivos de secuenciación genómica.
    *   *Monto:* **$2.200,00 USD**

---

### Rubro 3: Reactivos, Insumos de Laboratorio y Muestreo Clínico ($4.600,00 USD)
*Insumos necesarios para la recolección estéril y preservación de biopsias nasofaríngeas en pacientes pediátricos en el hospital, así como el procesamiento histológico para microscopía electrónica.*

1.  **Insumos para Cepillado Nasal y Preservación Celular:**
    *   *Descripción:* Cepillos citológicos estériles especiales de uso pediátrico (*cytobrushes*), medio de transporte y mantenimiento de epitelio ciliar (Medium 199 / RPMI 1640 con búfer HEPES, suplementado con antibióticos y antimicóticos para evitar contaminación en el muestreo nasofaríngeo), portaobjetos de precisión de alta planitud óptica, cubreobjetos Nº 1.5 y selladores siliconados para cámaras húmedas descartables.
    *   *Monto:* **$2.400,00 USD**
2.  **Reactivos para Microscopía Electrónica de Transmisión (TEM):**
    *   *Descripción:* Glutaraldehído y tetróxido de osmio de grado microscopía para fijación ultraestructural de axonemas, resinas epoxídicas de inclusión (tipo Epon / Araldite), rejillas de microscopía de cobre/níquel con soporte de formvar/carbono, y sales de contrastación (acetato de uranilo y citrato de plomo).
    *   *Monto:* **$2.200,00 USD**

---

### Rubro 4: Recursos Humanos, Estipendios Estudiantiles y Asistencia Técnica ($10.900,00 USD)
*Clave para el desarrollo local de hardware y software en FCEN-UBA, promoviendo la formación de jóvenes investigadores en el área de ingeniería biomédica y ciencias de la computación.*

1.  **Estipendio Estudiantil de Iniciación - Estudiante de Ingeniería / Prototipado (FCEN-UBA / Ingeniería):**
    *   *Descripción:* Asignación económica de estímulo a la investigación para 1 estudiante avanzado de grado de Ingeniería Electrónica / Mecatrónica / Física, dedicado al modelado CAD, fabricación del chasis, programación del microcontrolador PID, integración de sensores y calibración térmica de la cámara ambiental (12 meses x $350,00 USD/mes).
    *   *Monto:* **$4.200,00 USD**
2.  **Estipendio Estudiantil de Iniciación - Estudiante de Computación / Bioimagen (FCEN-UBA):**
    *   *Descripción:* Asignación económica para 1 estudiante avanzado de Ciencias de la Computación / Bioinformática de la FCEN-UBA, dedicado a la implementación de la interfaz gráfica (PyQt/Napari), estructuración de bases de datos de pacientes y asistencia en la optimización de código en Python (12 meses x $350,00 USD/mes).
    *   *Monto:* **$4.200,00 USD**
3.  **Servicios Técnicos Especializados de Taller:**
    *   *Descripción:* Contratación de servicios externos de mecanizado de precisión en aluminio para la platina térmica, anodizado protector, y calibración metrológica certificada de las sondas de temperatura en laboratorio acreditado.
    *   *Monto:* **$2.500,00 USD**

---

### Rubro 5: Difusión Científica, Publicaciones Open Access y Congresos ($5.500,00 USD)
*Garantiza la transferencia de conocimiento, visibilidad de la Fundación BBVA y acceso abierto de los avances generados.*

1.  **Cargos por Procesamiento de Artículos en Acceso Abierto (Open Access APCs):**
    *   *Descripción:* Financiamiento de costos de publicación (APC) en 2 revistas internacionales indexadas de alto impacto (Q1/Q2) en las áreas de Bioinformática, Visión por Computadora Médica o Neumonología Pediátrica, garantizando que el método y los hallazgos genómicos estén inmediatamente disponibles sin barreras de pago para la comunidad médica mundial.
    *   *Monto:* **$4.000,00 USD**
2.  **Participación en Congresos Científicos y Talleres de Difusión:**
    *   *Descripción:* Costos de inscripción, traslados y producción de material para la presentación de los resultados del proyecto en congresos nacionales e internacionales de microscopía y neumonología pediátrica, destacando el apoyo de las Becas Leonardo de la Fundación BBVA.
    *   *Monto:* **$1.500,00 USD**

---

### Rubro 6: Costos de Administración Institucional, Retenciones y Gastos Bancarios ($5.000,00 USD)
*Costos operativos ineludibles para la percepción y administración de fondos internacionales a través de la sede institucional (FCEN-UBA).*

1.  **Costos Administrativos, Retenciones e Imprevistos Bancarios:**
    *   *Descripción:* Previsión para gastos de administración del convenio institucional requeridos por la institución de adscripción (FCEN-UBA / fundación de apoyo a la investigación universitaria), comisiones bancarias por transferencias internacionales de divisas (tres desembolsos previstos en las bases: 50% inicial, 40% intermedio, 10% final), sellados fiscales y fluctuaciones de tipo de cambio legal.
    *   *Monto:* **$5.000,00 USD**

---

## 3. Justificación de la Costo-Efectividad de la Propuesta

El presente presupuesto demuestra una **muy alta costo-efectividad** en el uso de los fondos solicitados:
*   Un sistema comercial cerrado para análisis de videomicroscopía ciliar (HSVM) importado llave en mano cuesta entre **USD 120.000 y USD 180.000**, suma inaccesible para los presupuestos de los hospitales públicos en Argentina.
*   Con **USD 50.000**, este proyecto desarrollado en la Facultad de Ciencias Exactas y Naturales (UBA) en colaboración con el Hospital de Niños Dr. Ricardo Gutiérrez (un importante centro de referencia en el país) genera:
    1.  La modernización física in situ del equipamiento óptico (cámara de alta velocidad y cámara de incubación a 37 °C).
    2.  Una suite de software de visión computacional y bioinformática libre y de código abierto.
    3.  Capacidad de cuantificación en microscopía electrónica de transmisión (TEM).
    4.  El primer relevamiento de variantes genéticas de DCP en niños de Argentina.
    5.  Formación de recursos humanos universitarios en FCEN-UBA y transferencia tecnológica directa al equipo médico asistencial.
