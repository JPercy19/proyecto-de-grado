# Estado del arte: referentes contextuales

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

## Analisis critico de los referentes comerciales

Fluke Biomedical ESA615 se toma como referente de una arquitectura profesional que integra pruebas de seguridad eléctrica, identificación y almacenamiento de datos. Su aporte al proyecto es mostrar que el procedimiento de prueba no termina con una cifra: se requiere asociar la actividad con un activo o escenario, una configuración y un registro. De este referente se derivan requisitos pedagógicos como una secuencia visible, separación entre interacción del usuario y conexiones de ensayo, e identificación de cada práctica. No se pretende copiar su electrónica, reproducir prestaciones ni afirmar equivalencia de exactitud o cobertura normativa.

Rigel 288+ aporta un referente de portabilidad y de organización de procedimientos y resultados. El aspecto relevante no es replicar su formato físico, sino comprender que una práctica puede estructurarse como una secuencia configurable: selección de escenario, preparación, conexiones, ejecución, registro y revisión. Para el prototipo, esta lógica se traduce en reportes que conserven el contexto de la lectura. Cualquier comparación de rango, incertidumbre, protección o desempeño debe realizarse desde manuales vigentes y ensayos definidos, no desde una interpretación general de la ficha comercial.

Pronk Safe-T Sim debe analizarse como un referente de automatización, perfiles configurables y reportes; no basta llamarlo “simulador”. Su aporte es inspirar escenarios controlados y retroalimentación según condiciones predefinidas. La decisión de diseño derivada es que la plataforma pueda crear fallas simuladas seguras y asociarlas a una explicación, no que alcance el desempeño o las certificaciones declaradas por ese producto.

| Criterio de benchmark | Fluke ESA615 | Rigel 288+ | Pronk Safe-T Sim | Implicación para el prototipo |
|---|---|---|---|---|
| Uso previsto | Instrumento profesional de seguridad eléctrica. | Instrumento profesional portátil. | Plataforma comercial de prueba automatizada. | Declarar explícitamente uso didáctico y no clínico. |
| Aporte observado | Flujo de prueba, identificación y registro. | Procedimientos y gestión de resultados. | Perfiles, automatización y reportes. | Construir una secuencia de práctica trazable. |
| Arquitectura | Cerrada y orientada al servicio. | Cerrada y orientada al servicio. | Comercial y automatizada. | Exponer solo módulos de baja tensión y documentación segura. |
| Comparación válida | Funciones documentadas y experiencia de uso. | Organización de protocolos. | Diseño de escenarios. | No comparar exactitud o conformidad sin pruebas. |

## Aporte de la bibliografia al estado del arte

El estado del arte no se limita a describir productos. IEC 60601-1, IEC 62353 e IEC 60990 establecen el vocabulario técnico que permite comparar funciones sin afirmar conformidad. ISO 14971 permite valorar las diferencias de seguridad entre una plataforma educativa y un instrumento de servicio. ISO/IEC 17025, JCGM e ILAC explican por qué el benchmark no debe presentar una lectura didáctica como medición trazable.

Chagas (2018) aporta la justificación de acceso y adaptación de hardware abierto; Pearce (2017) añade sostenibilidad, documentación y soporte; Oellermann et al. (2022) vinculan la electrónica abierta con reproducción, reparación y comunidades de práctica. En conjunto, estas fuentes permiten evaluar “apertura” como documentación, mantenibilidad y control de versiones, no solo como acceso físico a circuitos.

Deslauriers et al. (2019) y NASEM (2018) sustentan que el referente disímil no debe compararse únicamente por componentes: su valor es pedagógico y se observa en tareas, retroalimentación y reflexión. Las revisiones de Lavado-Anguera et al. (2024) y Galdames-Calderon et al. (2024) indican que proyectos y retos requieren problema auténtico, acompañamiento y evaluación coherente. Santos-Diaz et al. (2024) conecta este enfoque con bioinstrumentación; Nandram y Foster (2025) amplían el análisis a kits biomédicos y sus criterios de accesibilidad, currículo, seguridad, costo y evidencia de efectividad.

## Brecha validable y contribucion esperada

La brecha de diseño se define como la necesidad de una herramienta que combine cuatro dimensiones: seguridad controlada, explicabilidad de la arquitectura, documentación abierta y evaluación pedagógica. Los instrumentos profesionales resuelven con alta integración el servicio técnico; los materiales educativos resuelven aspectos de acceso y aprendizaje; el prototipo propuesto busca conectar ambas perspectivas sin confundirse con un analizador profesional.

Esta contribución se validará con una comparación documentada y con usuarios del laboratorio. La plataforma será pertinente si permite ejecutar escenarios seguros, explicar cómo se configura una prueba, conservar evidencia de la práctica y demostrar mejora en tareas seleccionadas. No será suficiente que el circuito funcione; debe demostrar utilidad pedagógica, límites de seguridad claros y viabilidad para el contexto institucional.

## Evolucion del problema: de la prueba profesional a la experiencia de aprendizaje

La evolución de los analizadores de seguridad eléctrica responde a necesidades de servicio: reducir la variabilidad de procedimientos, acelerar tareas repetitivas, guardar resultados y apoyar la gestión de equipos. Por esa razón, los productos comerciales concentran su valor en la integración funcional, protección, portabilidad y trazabilidad de operaciones. Esa evolución es relevante para el proyecto, pero no define por sí sola una solución educativa. Un estudiante puede completar una secuencia automatizada sin comprender qué representa cada etapa, qué condición de ensayo está activa o qué limitaciones tiene el resultado.

La revisión de referentes permite plantear una diferencia entre **fidelidad funcional** y **fidelidad pedagógica**. La fidelidad funcional se refiere a la cercanía de una plataforma con los métodos o interfaces de un instrumento profesional. La fidelidad pedagógica se refiere a la capacidad de hacer visible el razonamiento, provocar predicción, permitir error seguro, dar retroalimentación y exigir explicación. El prototipo no necesita maximizar la primera para aportar al aprendizaje; debe seleccionar el nivel de fidelidad funcional que permita una experiencia segura y comprensible.

Esta distinción orienta la selección de escenarios. Un escenario con señales equivalentes o una falla controlada puede tener menos realismo que un ensayo conectado a red, pero puede ser más útil en una primera práctica si permite observar causa y efecto sin introducir un riesgo desproporcionado. A medida que el estudiante demuestre competencia y el laboratorio cuente con protocolos autorizados, se podrán considerar escenarios de mayor complejidad. La progresión no debe ser una decisión improvisada: debe responder a resultados de aprendizaje y al análisis de riesgo.

## Criterios de comparacion y evidencia requerida

El benchmark debe evitar comparaciones de marketing. Cada celda de la matriz competitiva debe indicar la fuente, la fecha de consulta y si el dato procede de un manual, ficha técnica, cotización o demostración observada. Las especificaciones de exactitud, incertidumbre, protección y cumplimiento no se transferirán de un referente al prototipo. La comparación servirá para identificar decisiones de interfaz, documentación y experiencia de uso, no para afirmar superioridad técnica sin evidencia.

| Criterio | Pregunta de comparacion | Fuente válida | Uso en la decision de diseño |
|---|---|---|---|
| Uso previsto | ¿Para qué contexto declara el fabricante el producto? | Manual o ficha oficial vigente. | Definir con claridad el alcance educativo del banco. |
| Secuencia de prueba | ¿Cómo organiza preparación, ejecución y cierre? | Manual de usuario y observación autorizada. | Diseñar flujo de práctica y lista de verificación. |
| Registro | ¿Qué contexto acompaña el resultado? | Manual, formato de reporte o demostración. | Definir campos mínimos de registro educativo. |
| Interfaz física | ¿Cómo diferencia conexiones, accesorios y zonas de usuario? | Fotografías oficiales, manual y observación. | Elegir codificación, etiquetas y disposición física. |
| Seguridad declarada | ¿Qué advertencias y restricciones de uso comunica? | Manual y documentación de seguridad. | Redactar advertencias y controles de acceso. |
| Mantenimiento | ¿Qué accesorios, repuestos o actualizaciones requiere? | Manual, soporte y cotización. | Definir modularidad, BOM y estrategia de mantenimiento. |
| Costo | ¿Cuál es costo de adquisición y operación? | Cotización con fecha y condiciones. | Fijar restricción económica realista. |

## Referentes educativos y pedagogicos

Los kits de enseñanza de bioinstrumentación constituyen un referente disímil porque su valor no se mide por cumplir una función clínica, sino por permitir que un estudiante explore, construya y evalúe. Nandram y Foster (2025) muestran que los kits disponibles son heterogéneos: cambian la tecnología, la forma de documentación, los niveles de costo y la evidencia de efectividad. La contribución de esa revisión es establecer que un kit debe evaluarse como parte de un sistema de aprendizaje, con guía docente, material de apoyo, posibilidades de réplica y resultados de aprendizaje explícitos.

Santos-Diaz et al. (2024) aporta un caso de aprendizaje basado en retos en bioinstrumentación. El valor de esta fuente es metodológico: la experiencia de diseño se organiza alrededor de un reto, prototipado, prueba, retroalimentación y reflexión. Para el proyecto, un reto no consiste en “usar el analizador”; consiste en explicar por qué un escenario controlado produce un resultado, qué conexión o condición lo modifica y qué decisión responsable corresponde. Galdames-Calderon et al. (2024) complementan al advertir que el reto debe ser claro, relevante y acompañado por facilitación.

Las fuentes de PBL y aprendizaje activo obligan a valorar la plataforma en dos niveles. En el primer nivel, se evalúa el dispositivo: si es seguro, disponible, mantenible y comprensible. En el segundo, se evalúa la actividad: si plantea objetivos claros, requiere razonamiento, entrega retroalimentación, permite colaboración y recoge evidencia. Un banco técnicamente correcto puede fracasar como recurso educativo si no incluye esta segunda capa.

## Sintesis critica de la brecha

La literatura técnica ofrece normas y analizadores de alto nivel de integración; la literatura de hardware abierto ofrece principios de documentación, acceso y reparación; la literatura educativa ofrece estrategias para aprendizaje activo y evaluación. La brecha aparece en la intersección de los tres campos. No se trata de reproducir un instrumento comercial a menor costo, sino de diseñar una infraestructura de aprendizaje que traduzca conceptos normativos y metrológicos en experiencias controladas.

La contribución proyectada se puede formular en cuatro componentes. Primero, un conjunto de escenarios didácticos de baja energía que represente decisiones y fallas relevantes. Segundo, una arquitectura visible de módulos de baja tensión con documentación suficiente para inspección y mantenimiento. Tercero, una interfaz que guíe la práctica, registre el contexto e impida interpretar el resultado como certificado clínico. Cuarto, un protocolo de evaluación que mida tareas, comprensión y usabilidad.

La originalidad no se sostendrá con la afirmación de que “no existe” un producto similar. Se sostendrá si el análisis muestra que los referentes profesionales no priorizan transparencia pedagógica y que los referentes educativos no integran de forma explícita la lógica de seguridad eléctrica y los límites metrológicos. Esta proposición deberá contrastarse con un benchmark ampliado, manuales vigentes, cotizaciones y evidencia de usuarios.

## Lineas de evaluacion derivadas del estado del arte

| Dimension | Pregunta de evaluación | Evidencia esperada |
|---|---|---|
| Seguridad | ¿El escenario de práctica evita exposición no aceptable y comunica sus límites? | Matriz de riesgos, inspección y protocolo de prueba. |
| Aprendizaje | ¿El estudiante puede configurar, interpretar y explicar el escenario? | Rúbrica, pretest/postest y observación de tarea. |
| Usabilidad | ¿La interfaz permite completar la práctica con errores controlados? | Prueba de tareas, tasa de error y cuestionario. |
| Apertura | ¿La documentación permite comprender y mantener módulos autorizados? | Repositorio, BOM, esquemáticos y control de versiones. |
| Viabilidad | ¿El banco se adapta a presupuesto, tiempo y espacio disponibles? | Cotizaciones, inventario y cronometraje. |
| Alcance | ¿Usuarios y reportes distinguen uso educativo de uso profesional? | Entrevista, revisión de interfaz y auditoría de reporte. |

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

Deslauriers, L., McCarty, L. S., Miller, K., Callaghan, K., & Kestin, G. (2019). Measuring actual learning versus feeling of learning in response to being actively engaged in the classroom. *Proceedings of the National Academy of Sciences, 116*(39), 19251-19257. https://doi.org/10.1073/pnas.1821936116

Fluke Biomedical. (s. f.). *ESA615 electrical safety analyzer*. https://www.flukebiomedical.com/products/electrical-safety-analyzers/esa615-electrical-safety-analyzer

National Academies of Sciences, Engineering, and Medicine. (2018). *How people learn II: Learners, contexts, and cultures*. National Academies Press. https://doi.org/10.17226/24783

Pronk Technologies. (s. f.). *Safe-T Sim electrical safety analyzer simulator*. https://www.pronktech.com/

Rigel Medical. (s. f.). *Rigel 288+ electrical safety analyzer*. https://www.rigelmedical.com/product/406a910-288-plus/
