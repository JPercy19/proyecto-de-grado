# Marco teórico: referentes conceptuales

## Seguridad eléctrica

La seguridad eléctrica de un equipo electromédico se relaciona con el control de peligros derivados de la energía eléctrica, las partes conductivas accesibles, la conexión a tierra de protección y las partes aplicadas. IEC 60601-1 establece requisitos generales para seguridad básica y desempeño esencial de equipos electromédicos. En este proyecto se usa como marco conceptual para comprender riesgos y organizar la discusión de pruebas; no se usa para declarar que el prototipo o un equipo ensayado cumple la norma (IEC, 2020).

IEC 62353 se ocupa de pruebas recurrentes y posteriores a reparación. Por ello, orienta una secuencia de aprendizaje sobre preparación, configuración, registro e interpretación de una práctica, pero no sustituye las instrucciones del fabricante ni es equivalente a la evaluación de diseño de IEC 60601-1 (IEC, 2014). IEC 60990 complementa este marco al definir métodos de medición para corriente de contacto y corriente del conductor de protección (IEC, 2016).

| Concepto | Definición operativa en el proyecto |
|---|---|
| Tierra de protección | Ruta conductora que conecta partes accesibles con la protección eléctrica, estudiada mediante escenarios controlados. |
| Corriente de fuga | Corriente no intencional cuya interpretación depende de la ruta y configuración de ensayo. |
| Parte aplicada | Parte que entra en contacto físico con el paciente para cumplir la función del equipo; su clasificación no se asigna sin revisar documentación del fabricante. |
| Condición normal y falla única | Situaciones de operación usadas para razonar cómo una falla puede afectar la seguridad. |
| Red de medición | Conjunto de conexiones, impedancias, rango y protección que da significado a una lectura. |

## Gestión del riesgo

ISO 14971 propone identificar peligros, estimar y evaluar riesgos, aplicar controles y revisar el riesgo residual. ISO/TR 24971 ayuda a aplicar este proceso en dispositivos médicos (ISO, 2019, 2020). Para la plataforma se consideran peligros como contacto con tensión, energía almacenada, error de conexión, falla de aislamiento, interpretación errónea, uso clínico indebido y modificación no autorizada.

La estrategia de control debe privilegiar la reducción por diseño. Por ejemplo, la simulación de fallas de baja energía reduce el riesgo antes de recurrir a advertencias. Los enclavamientos, cubiertas, conectores diferenciados, fusibles y procedimientos de práctica son controles complementarios, no sustitutos de una arquitectura inherentemente más segura.

## Metrología y trazabilidad

La trazabilidad metrológica relaciona un resultado con referencias reconocidas mediante una cadena documentada de calibraciones. La expresión de incertidumbre y las reglas de decisión son necesarias cuando una medición respalda una declaración de conformidad (JCGM, 2008; ISO/IEC, 2017; ILAC, 2019). Por esta razón, el proyecto diferenciará entre un resultado de aprendizaje y una medición profesional.

La plataforma podrá registrar valores y configuraciones para fines pedagógicos, pero sus reportes incluirán la advertencia de que no son certificados de conformidad. Esta distinción es central: enseñar el método no equivale a producir una medición trazable para liberar un equipo.

## Arquitectura abierta

Una arquitectura abierta documenta interfaces, esquemáticos, firmware, lista de materiales, protocolo de montaje, pruebas y versiones. La apertura favorece inspección, adaptación, reparación y aprendizaje, especialmente en laboratorios con recursos limitados (Chagas, 2018; Oellermann et al., 2022). No significa retirar controles de seguridad. El proyecto abrirá los módulos de baja tensión, adquisición, visualización y software; el acceso a zonas con energía peligrosa permanecerá restringido.

## Educación práctica y diseño centrado en personas

La plataforma se fundamenta en aprendizaje activo: cada práctica debe llevar al estudiante a predecir, configurar, observar, registrar y explicar. La evidencia de aprendizaje debe incluir tareas y explicaciones, además de encuestas de satisfacción (Deslauriers et al., 2019). El aprendizaje basado en proyectos y retos aporta una forma de conectar una necesidad real de ingeniería con prototipado, reflexión y evaluación (Lavado-Anguera et al., 2024).

ISO 9241-210, IEC 62366-1 y la guía de FDA establecen la importancia de conocer usuarios, contexto, tareas críticas y posibles errores de uso antes de definir una interfaz. En consecuencia, la indagación social se integra desde el inicio del proceso, y no solo al final como una prueba de aceptación (ISO, 2019; IEC, 2020; FDA, 2016).

## Articulacion entre norma, riesgo y medicion

IEC 60601-1, IEC 62353 e IEC 60990 no son documentos intercambiables. IEC 60601-1 aporta el marco de seguridad basica, desempeño esencial y gestión del riesgo de un equipo electromédico. IEC 62353 organiza pruebas de seguridad durante la vida útil, particularmente después de reparación y de manera recurrente. IEC 60990 aporta el método de medición de determinadas corrientes. En consecuencia, una práctica responsable debe enseñar tres preguntas distintas: qué peligro se intenta controlar, qué procedimiento se está ejecutando y qué significa técnicamente el resultado de la medición. Confundir estas preguntas lleva a interpretar que una lectura aislada demuestra conformidad de diseño, algo que no puede concluirse con el prototipo.

IEC 60479-1 complementa la explicación al estudiar los efectos de la corriente en el cuerpo humano. Su aporte pedagógico es justificar que el aprendizaje se realice con simulación de baja energía, barreras físicas y secuencias controladas. Esta referencia no permite trasladar límites fisiológicos a criterios de aceptación de una prueba específica, pues estos dependen de la norma aplicable, del método, de la configuración y del equipo evaluado.

Para el diseño, ISO 14971 transforma estos conceptos en decisiones: se identifican peligros, se estiman riesgos, se seleccionan controles y se verifica su eficacia. El análisis de riesgo no debe limitarse al circuito; también debe incluir errores de conexión, interpretación equivocada de una lectura, acceso no autorizado, modificación de módulos y uso clínico indebido. ISO/TR 24971 se utiliza para orientar la aplicación de ese proceso y documentar por qué un control fue elegido.

## Interpretacion metrologica del resultado

ISO/IEC 17025 define requisitos de competencia para laboratorios de ensayo y calibración. JCGM 100 desarrolla la evaluación y expresión de incertidumbre; ILAC P10, P14 y G8 relacionan trazabilidad, incertidumbre y reglas de decisión. Estas fuentes aportan un límite metodológico fundamental: una pantalla que muestre un valor no equivale a un resultado apto para aprobar o rechazar un equipo clínico.

El registro didáctico debe incluir, como mínimo, el código de escenario, la versión del protocolo, la configuración de conexiones, el rango usado, el resultado visualizado, la interpretación del estudiante y la advertencia de alcance educativo. Si en fases futuras se requiere comparar mediciones, será necesario diseñar un método de calibración, identificar las fuentes de incertidumbre y definir una regla de decisión antes de emitir cualquier declaración de conformidad.

## Arquitectura abierta como estrategia de aprendizaje

Chagas (2018) aporta el argumento de acceso: el hardware científico abierto puede reducir barreras económicas y permitir adaptación local. Pearce (2017) amplía esa idea al señalar que la apertura sostenible requiere documentación reproducible, lista de componentes, licencias, mantenimiento y soporte. Oellermann et al. (2022) enfatizan que la electrónica abierta favorece reparación, reproducibilidad y comunidades de práctica cuando la documentación permite reconstruir el sistema.

Estas referencias no justifican exponer a estudiantes a partes energizadas. La decisión resultante es una arquitectura por capas: la capa pedagógica muestra el diagrama funcional; la capa de baja tensión permite inspección y modificación documentada; y la capa potencialmente peligrosa, si se incorporara, permanece protegida, separada físicamente y sometida a control de cambios. Cada versión deberá conservar esquemáticos, firmware, BOM, protocolo de pruebas y registro de modificaciones.

## Fundamento pedagogico y de usabilidad

Deslauriers et al. (2019) muestran que el aprendizaje percibido y el aprendizaje demostrado pueden diferir. Por ello, el éxito de la plataforma no se medirá solamente con una encuesta de satisfacción: se observará si el estudiante predice un comportamiento, conecta el escenario de forma correcta, identifica un error, interpreta el resultado y explica sus limitaciones. *How People Learn II* (National Academies of Sciences, Engineering, and Medicine, 2018) sustenta una secuencia de activación de conocimientos previos, práctica guiada, retroalimentación y reflexión.

Lavado-Anguera et al. (2024) proponen el aprendizaje basado en proyectos como una forma de articular problema, colaboración, prototipado y reflexión en ingeniería. Galdames-Calderon et al. (2024) advierten que el aprendizaje basado en retos requiere un reto auténtico, facilitación docente y criterios de evaluación explícitos. Santos-Diaz et al. (2024) aporta evidencia situada en bioinstrumentación y señala la necesidad de planeación y mentoría. Nandram y Foster (2025) muestran que los kits educativos biomédicos son heterogéneos; por tanto, la evaluación debe cubrir seguridad, accesibilidad, integración curricular, costo, documentación y evidencia de aprendizaje.

IEC 62366-1, ISO 9241-210 y FDA (2016) aportan el enfoque de factores humanos. El diseño debe partir de usuarios, tareas y errores previsibles. En la práctica, esto se traduce en conectores diferenciados, pasos visibles, confirmación antes de iniciar, advertencias contextualizadas y una interfaz que explique por qué se bloquea una acción. Design Council (2019) y Ulrich et al. (2020) organizan estas decisiones en un proceso iterativo: descubrir necesidades, definir requisitos, desarrollar alternativas, seleccionar con criterios medibles y evaluar prototipos.

## Aporte de los referentes al proyecto

| Referencia | Aporte conceptual específico | Decisión de diseño sustentada | Límite de interpretación |
|---|---|---|---|
| IEC 60601-1 | Relaciona seguridad básica, desempeño esencial y gestión del riesgo. | Identificar peligros, límites de uso y barreras de seguridad. | No certifica el prototipo ni equipos evaluados con él. |
| IEC 62353 | Estructura pruebas recurrentes y posteriores a reparación. | Diseñar guías de preparación, ejecución, registro y cierre. | No evalúa conformidad de diseño con IEC 60601-1. |
| IEC 60990 | Muestra que la corriente depende de red y configuración de medición. | Mostrar escenario, ruta, rango y método junto a cada lectura. | No define toda la seguridad de un equipo médico. |
| IEC 60479-1 | Explica la relevancia fisiológica del peligro eléctrico. | Priorizar simulación de baja energía y barreras. | No fija por sí sola criterios de aceptación. |
| ISO 14971 e ISO/TR 24971 | Ofrecen proceso sistemático de gestión del riesgo. | Matriz de peligros, controles, verificación y riesgo residual. | No reemplazan requisitos regulatorios si el alcance cambia. |
| ISO/IEC 17025, JCGM 100 e ILAC | Distinguen medición educativa de declaración de conformidad. | Etiquetar reportes como didácticos y documentar el método. | No acreditan automáticamente al equipo. |
| Chagas; Pearce; Oellermann et al. | Vinculan apertura con acceso, documentación, reparación y sostenibilidad. | Repositorio versionado, BOM, firmware y módulos seguros inspeccionables. | No justifican acceso a circuitos peligrosos. |
| Deslauriers; NASEM | Separan aprendizaje demostrado de percepción de aprendizaje. | Evaluar tareas, rúbricas y explicaciones, no solo satisfacción. | La transferencia a la cohorte local debe validarse. |
| PBL/CBL y kits biomédicos | Definen el valor de reto, mentoría y currículo. | Guías, escenarios, rúbricas y tiempo de acompañamiento docente. | No garantizan aprendizaje sin una implementación adecuada. |
| IEC 62366-1; ISO 9241-210; FDA | Analizan uso, contexto y errores de interacción. | Pruebas de usabilidad y prevención de errores de conexión. | No sustituyen la gestión de riesgo eléctrico. |
| Design Council; Ulrich et al. | Estructuran el proceso de diseño y selección. | Casa de la Calidad, generación de alternativas y matriz ponderada. | No fijan requisitos IEC ni métricas clínicas. |

## Referencias

Chagas, A. M. (2018). Haves and have nots must find a better way: The case for open scientific hardware. *PLOS Biology, 16*(9), e3000014. https://doi.org/10.1371/journal.pbio.3000014

Deslauriers, L., McCarty, L. S., Miller, K., Callaghan, K., & Kestin, G. (2019). Measuring actual learning versus feeling of learning in response to being actively engaged in the classroom. *Proceedings of the National Academy of Sciences, 116*(39), 19251-19257. https://doi.org/10.1073/pnas.1821936116

International Electrotechnical Commission. (2014). *IEC 62353:2014: Medical electrical equipment—Recurrent test and test after repair of medical electrical equipment*. https://webstore.iec.ch/en/publication/6913

International Electrotechnical Commission. (2016). *IEC 60990:2016: Methods of measurement of touch current and protective conductor current*. https://webstore.iec.ch/en/publication/24992

International Electrotechnical Commission. (2020). *IEC 60601-1:2005+AMD1:2012+AMD2:2020 CSV: Medical electrical equipment—Part 1: General requirements for basic safety and essential performance*. https://webstore.iec.ch/en/publication/67497

International Organization for Standardization. (2019). *ISO 14971:2019: Medical devices—Application of risk management to medical devices*. https://www.iso.org/standard/72704.html

International Organization for Standardization. (2020). *ISO/TR 24971:2020: Medical devices—Guidance on the application of ISO 14971*. https://www.iso.org/standard/74437.html

International Organization for Standardization. (2019). *ISO 9241-210:2019: Ergonomics of human-system interaction—Part 210: Human-centred design for interactive systems*. https://www.iso.org/standard/77520.html

International Organization for Standardization. (2017). *ISO/IEC 17025:2017: General requirements for the competence of testing and calibration laboratories*. https://www.iso.org/standard/66912.html

Joint Committee for Guides in Metrology. (2008). *Evaluation of measurement data—Guide to the expression of uncertainty in measurement* (JCGM 100:2008). https://doi.org/10.59161/JCGM100-2008E

Lavado-Anguera, S., Velasco-Quintana, P.-J., & Terron-Lopez, M.-J. (2024). Project-based learning as an experiential pedagogical methodology in engineering education: A review of the literature. *Education Sciences, 14*(6), 617. https://doi.org/10.3390/educsci14060617

Oellermann, M., Jolles, J. W., Ortiz, D., Seabra, R., Wenzel, T., Wilson, H., & Tanner, R. L. (2022). Open hardware in science: The benefits of open electronics. *Integrative and Comparative Biology, 62*(4), 1061-1075. https://doi.org/10.1093/icb/icac043

Design Council. (2019). *The framework for innovation: Design Council's evolved Double Diamond*. https://www.designcouncil.org.uk/our-resources/framework-for-innovation/

Galdames-Calderon, M., Pedersen, A. S., & Rodriguez-Gomez, D. (2024). Systematic review: Revisiting challenge-based learning teaching practices in higher education. *Education Sciences, 14*(9), 1008. https://doi.org/10.3390/educsci14091008

International Electrotechnical Commission. (2018). *IEC 60479-1:2018: Effects of current on human beings and livestock—Part 1: General aspects*. https://webstore.iec.ch/en/publication/62980

International Electrotechnical Commission. (2020). *IEC 62366-1:2015/AMD1:2020: Medical devices—Part 1: Application of usability engineering to medical devices*. https://webstore.iec.ch/en/publication/66794

International Laboratory Accreditation Cooperation. (2019). *ILAC G8:09/2019: Guidelines on decision rules and statements of conformity*. https://ilac.org/publications-and-resources/ilac-guidance-series/

International Laboratory Accreditation Cooperation. (2020). *ILAC P10:07/2020: ILAC policy on metrological traceability of measurement results*. https://ilac.org/publications-and-resources/ilac-policy-series/

International Laboratory Accreditation Cooperation. (2020). *ILAC P14:09/2020: ILAC policy for measurement uncertainty in calibration*. https://ilac.org/publications-and-resources/ilac-policy-series/

National Academies of Sciences, Engineering, and Medicine. (2018). *How people learn II: Learners, contexts, and cultures*. National Academies Press. https://doi.org/10.17226/24783

Nandram, A. P., & Foster, J. A. (2025). Systematic review of teaching kits in biomedical engineering education. In *2025 ASEE annual conference and exposition proceedings*. https://doi.org/10.18260/1-2--57180

Pearce, J. M. (2017). Emerging business models for open source hardware. *Journal of Open Hardware, 1*(1), 2. https://doi.org/10.5334/joh.4

Santos-Diaz, A., Montesinos, L., Barrera-Esparza, M., del Mar Perez-Desentis, M., & Salinas-Navarro, D. E. (2024). Implementing a challenge-based learning experience in a bioinstrumentation blended course. *BMC Medical Education, 24*, 528. https://doi.org/10.1186/s12909-024-05462-7

U.S. Food and Drug Administration. (2016). *Applying human factors and usability engineering to medical devices: Guidance for industry and Food and Drug Administration staff*. https://www.fda.gov/media/80481/download

Ulrich, K. T., Eppinger, S. D., & Yang, M. C. (2020). *Product design and development* (7th ed.). McGraw-Hill Education.
