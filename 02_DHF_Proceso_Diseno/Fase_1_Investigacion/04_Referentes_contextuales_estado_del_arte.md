# Referentes contextuales y estado del arte

## Contexto normativo y regulatorio

El proyecto se sitúa en el entorno de los equipos electromédicos y su mantenimiento. IEC 60601-1 es el referente general para seguridad básica y desempeño esencial; IEC 62353 se orienta a pruebas recurrentes y posteriores a reparación. IEC 60990 define métodos de medición de corrientes de contacto y del conductor de protección. Estas normas se consultan legalmente mediante acceso institucional y se citan sin reproducir sus tablas, límites ni figuras protegidas.

En Colombia, el Decreto 4725 de 2005 regula el régimen de dispositivos médicos y la Resolución 4816 de 2008 reglamenta el Programa Nacional de Tecnovigilancia. El proyecto no pretende comercializar un dispositivo médico ni realizar tecnovigilancia; estos referentes permiten comprender por qué la seguridad, documentación, uso previsto y comunicación de límites son relevantes para la ingeniería biomédica.

## Referentes comerciales

Los instrumentos profesionales constituyen referencias contextuales porque muestran cómo el mercado resuelve pruebas, interfaces, almacenamiento de resultados y protección. Deben evaluarse desde manuales, fichas técnicas vigentes y cotizaciones, no desde publicidad aislada.

| Referente | Aporte observable | Aspecto para comparar | Diferencia frente al proyecto |
|---|---|---|---|
| Fluke Biomedical ESA615 | Analizador profesional de seguridad eléctrica. | Tipos de prueba, accesorios, interfaz, almacenamiento y uso previsto. | Producto cerrado para servicio profesional. |
| Rigel 288+ | Analizador portátil de seguridad eléctrica. | Automatización, registro, modos de prueba y seguridad declarada. | No se concibe para revelar bloques internos. |
| Pronk Safe-T Sim | Simulador para prácticas y verificación de analizadores. | Escenarios de simulación y control de fallas. | No sustituye una plataforma de aprendizaje de arquitectura abierta. |
| Kit de bioinstrumentación | Referente disímil de enseñanza. | Modularidad, guía de práctica, costo, currículo y usabilidad. | Puede no incorporar pruebas de seguridad eléctrica. |

El benchmark definitivo incluirá tres productos similares y uno disímil, como solicita la guía DB1. Se documentarán: pruebas disponibles, rangos y exactitud declarada, interfaces, accesorios, protecciones, evidencia de trazabilidad, costo, mantenimiento, arquitectura visible y uso previsto. No se afirmará que dos productos tienen el mismo desempeño sin revisar la documentación de cada fabricante.

## Estado actual de la oportunidad de diseño

Existen analizadores profesionales que automatizan la ejecución de ensayos y simuladores que permiten generar condiciones conocidas. También hay evidencia de kits de enseñanza que favorecen el aprendizaje de bioinstrumentación cuando son modulares, accesibles y se conectan con resultados de aprendizaje. La oportunidad aparece al combinar estas perspectivas en un banco educativo: una plataforma que enseñe el principio de la prueba, haga visible la arquitectura de baja energía, permita fallas simuladas y preserve las restricciones de seguridad.

El carácter abierto debe ser documentado y responsable. Chagas (2018), Pearce (2017) y Oellermann et al. (2022) señalan que el hardware abierto puede facilitar reproducibilidad, adaptación y mantenimiento; estos beneficios requieren esquemáticos, firmware, lista de materiales y control de versiones completos. En este proyecto, la apertura no puede convertirse en acceso indiscriminado a circuitos asociados a red eléctrica.

La revisión de educación en ingeniería respalda una práctica donde el estudiante resuelve una tarea, recibe retroalimentación y demuestra desempeño. Estudios recientes en aprendizaje basado en proyectos, retos y bioinstrumentación indican que el diseño de la actividad, la evaluación y el acompañamiento docente determinan el valor pedagógico (Galdames-Calderon et al., 2024; Nandram & Foster, 2025; Santos-Diaz et al., 2024).

## Brecha que aborda el proyecto

La brecha no se formula como “no existen analizadores”, sino como la falta de una herramienta educativa que reúna simultáneamente: arquitectura explicable, escenarios controlados, documentación abierta, guía de práctica, registro de evidencias y separación clara entre aprendizaje y medición profesional. Esta formulación se validará con el inventario de laboratorio y con los hallazgos de usuarios; puede ajustarse si el contexto muestra una necesidad diferente.

## Referencias

Chagas, A. M. (2018). Haves and have nots must find a better way: The case for open scientific hardware. *PLOS Biology, 16*(9), e3000014. https://doi.org/10.1371/journal.pbio.3000014

Galdames-Calderon, M., Pedersen, A. S., & Rodriguez-Gomez, D. (2024). Systematic review: Revisiting challenge-based learning teaching practices in higher education. *Education Sciences, 14*(9), 1008. https://doi.org/10.3390/educsci14091008

International Electrotechnical Commission. (2014). *IEC 62353:2014: Medical electrical equipment—Recurrent test and test after repair of medical electrical equipment*. https://webstore.iec.ch/en/publication/6913

International Electrotechnical Commission. (2016). *IEC 60990:2016: Methods of measurement of touch current and protective conductor current*. https://webstore.iec.ch/en/publication/24992

International Electrotechnical Commission. (2020). *IEC 60601-1:2005+AMD1:2012+AMD2:2020 CSV: Medical electrical equipment—Part 1: General requirements for basic safety and essential performance*. https://webstore.iec.ch/en/publication/67497

Ministerio de la Proteccion Social. (2005). *Decreto 4725 de 2005*. https://www.funcionpublica.gov.co/eva/gestornormativo/norma.php?i=17622

Ministerio de la Proteccion Social. (2008). *Resolucion 4816 de 2008*. https://normograma.invima.gov.co/normograma/compilacion/docs/resolucion_minproteccion_4816_2008.htm

Nandram, A. P., & Foster, J. A. (2025). Systematic review of teaching kits in biomedical engineering education. In *2025 ASEE annual conference and exposition proceedings*. https://doi.org/10.18260/1-2--57180

Oellermann, M., Jolles, J. W., Ortiz, D., Seabra, R., Wenzel, T., Wilson, H., & Tanner, R. L. (2022). Open hardware in science: The benefits of open electronics. *Integrative and Comparative Biology, 62*(4), 1061-1075. https://doi.org/10.1093/icb/icac043

Pearce, J. M. (2017). Emerging business models for open source hardware. *Journal of Open Hardware, 1*(1), 2. https://doi.org/10.5334/joh.4

Santos-Diaz, A., Montesinos, L., Barrera-Esparza, M., del Mar Perez-Desentis, M., & Salinas-Navarro, D. E. (2024). Implementing a challenge-based learning experience in a bioinstrumentation blended course. *BMC Medical Education, 24*, 528. https://doi.org/10.1186/s12909-024-05462-7
