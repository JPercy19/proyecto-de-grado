# Referentes conceptuales

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
