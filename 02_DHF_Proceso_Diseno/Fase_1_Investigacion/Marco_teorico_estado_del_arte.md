# Marco teorico, conceptual y estado del arte

## Proposito y delimitacion

Este documento sustenta la fase de investigacion del proyecto. El prototipo se concibe exclusivamente como una plataforma didactica de laboratorio: no es un producto sanitario, no reemplaza un analizador calibrado y no puede emitir declaraciones de conformidad ni autorizar el uso clinico de un equipo. Las practicas se limitaran a simuladores, cargas protegidas o equipos expresamente autorizados, sin pacientes conectados y bajo supervision docente.

La bibliografia prioriza publicaciones de 2016 a 2026. Se conservan como excepciones justificadas IEC 62353:2014, la Resolucion 4816:2008 y JCGM 100:2008: son los documentos vigentes o normativos que definen, respectivamente, el procedimiento de prueba recurrente, el contexto colombiano de tecnovigilancia y la expresion de incertidumbre.

## Marco teorico y conceptual

### Seguridad electrica en equipos electromedicos

Un equipo electromedico puede incorporar una conexion a tierra de proteccion, partes conductivas accesibles y partes aplicadas que establecen contacto funcional con el paciente. La seguridad electrica controla que la energia electrica no produzca un riesgo inaceptable para paciente, operador o personal de mantenimiento. IEC 60601-1 estructura este objetivo desde la seguridad basica, el desempeno esencial y la gestion del riesgo; IEC 60479-1 explica los efectos fisiologicos de la corriente electrica en el cuerpo humano (IEC, 2020a, 2018).

Para la experiencia didactica se estudiaran cuatro ideas sin reproducir tablas ni limites protegidos por las normas:

| Concepto | Explicacion para la practica | Evidencia de aprendizaje esperada |
|---|---|---|
| Tierra de proteccion | Camino conductor entre el terminal de proteccion y las partes conductivas accesibles. | El estudiante identifica el recorrido y reconoce una discontinuidad simulada. |
| Corriente de fuga | Corriente no intencional que puede circular por tierra, envolvente o parte aplicada segun el metodo de ensayo. | El estudiante diferencia la configuracion de la lectura de su valor numerico. |
| Red de medicion | Red, rango, proteccion y conexion que condicionan el significado de una lectura de corriente. | El estudiante no conecta un amperimetro de forma arbitraria y explica el montaje. |
| Condicion normal y falla unica | Escenarios definidos para analizar si una barrera o una falla modifican el riesgo. | El estudiante reconoce que un resultado depende de la condicion de ensayo. |

IEC 60990 especifica métodos de medicion de corriente de contacto y de conductor de proteccion. Por tanto, el sistema no debe presentar una “corriente de fuga” como un dato aislado: debe informar el escenario, la red empleada, el rango, la conexion y las restricciones del ejercicio (IEC, 2016). IEC 62353 sirve para organizar pruebas recurrentes y posteriores a reparacion; no sustituye el manual del fabricante ni demuestra que un equipo cumple IEC 60601-1 (IEC, 2014).

### Metrologia, riesgo y trazabilidad

Una lectura didactica se diferencia de un resultado apto para una decision de conformidad. Este ultimo exige instrumentos calibrados, cadena de trazabilidad, incertidumbre, reglas de decision y competencia de laboratorio, conforme a ISO/IEC 17025, JCGM 100, ILAC P10 y P14 (ISO, 2017; JCGM, 2008; ILAC, 2020a, 2020b). El prototipo registrara la configuracion de la practica y sus resultados para favorecer la reproducibilidad pedagogica, pero mostrara el estado “uso didactico; no apto para liberacion clinica”.

La gestion del riesgo comienza en la fase de requisitos. ISO 14971 e ISO/TR 24971 permiten identificar peligros, estimar riesgos, definir controles y evaluar el riesgo residual (ISO, 2019a, 2020). Para este proyecto se consideran como minimo: tension de red, energia residual, conexion incorrecta, falla de aislamiento, acceso a una zona restringida, error de interpretacion, uso clinico indebido y modificacion no autorizada. El orden de control sera: eliminacion o reduccion por diseno, barreras y enclavamientos, informacion de seguridad y capacitacion. La documentacion abierta solo se aplicara a los modulos seguros de baja energia, adquisicion, visualizacion y software; las interfaces asociadas a red permaneceran protegidas y con acceso restringido.

### Arquitectura abierta y aprendizaje practico

La arquitectura abierta se entiende como la disponibilidad de esquematicos, lista de materiales, firmware, interfaces, protocolo de montaje, pruebas y control de versiones. Esta apertura facilita la inspeccion, reparacion y apropiacion de la instrumentacion, siempre que la documentacion comunique límites de seguridad. La literatura sobre hardware abierto destaca beneficios de acceso, reproducibilidad y adaptacion local, pero tambien exige documentación suficiente y gobernanza de cambios (Chagas, 2018; Pearce, 2017; Oellermann et al., 2022).

El valor educativo no procede solamente de “usar” un instrumento. El estudiante debe predecir el resultado, configurar el escenario, observar el efecto de una falla simulada, comparar la lectura con el procedimiento y explicar sus limites. El aprendizaje activo se debe valorar con desempeño observable y no unicamente con satisfacción percibida (Deslauriers et al., 2019). El aprendizaje basado en proyectos y retos aporta una estructura adecuada porque integra un problema autentico, colaboración, prototipado, retroalimentacion y reflexión (Lavado-Anguera et al., 2024; Galdames-Calderon et al., 2024; Santos-Diaz et al., 2024).

### Diseño centrado en las personas

La indagacion con estudiantes, docentes y personal tecnico es parte del diseño, no una validacion decorativa. ISO 9241-210, IEC 62366-1 y la guia de factores humanos de FDA recomiendan identificar usuarios, tareas, errores previsibles y condiciones de uso antes de definir una interfaz (ISO, 2019b; IEC, 2020b; FDA, 2016). El Double Diamond organiza esta actividad en descubrir, definir, desarrollar y entregar; en cada fase se deben conservar decisiones, evidencia y trazabilidad (Design Council, 2019).

## Estado del arte

Los analizadores comerciales son referentes de funcionalidad y seguridad, no competidores equivalentes del prototipo. Fluke Biomedical ESA615 y Rigel 288+ integran pruebas profesionales y automatizadas, documentación de resultados y accesorios diseñados para contextos de servicio. Pronk Safe-T Sim se usa como referente de simulacion de seguridad electrica. Sus manuales y fichas tecnicas se consultaran para construir el benchmark de pruebas disponibles, interfaces, protecciones, accesorios, uso previsto, exactitud declarada y costo cotizado; ningún dato publicitario se usara como requisito normativo (Fluke Biomedical, s. f.; Rigel Medical, s. f.; Pronk Technologies, s. f.).

| Referente | Tipo | Aporte al benchmark | Limite frente al proyecto |
|---|---|---|---|
| Fluke Biomedical ESA615 | Analizador profesional | Secuencia de prueba, automatizacion, registro y accesorios. | Arquitectura cerrada y costo de instrumento profesional. |
| Rigel 288+ | Analizador profesional | Funciones de prueba, interfaz y trazabilidad de resultados. | No esta concebido como plataforma de aprendizaje abierta. |
| Pronk Safe-T Sim | Simulador de seguridad electrica | Escenarios controlados y practicas con simulacion. | No hace visible por si solo la arquitectura de medicion. |
| Kit didactico de bioinstrumentacion | Producto disimil | Diseño de practicas, modularidad, guia y evaluacion. | No aborda necesariamente seguridad electrica segun IEC. |

La oportunidad de diseño esta entre un simulador sin medicion explicable y un analizador profesional cerrado: un banco modular que guie la secuencia de ensayo, exponga los bloques seguros de su arquitectura, permita fallas simuladas y registre evidencias de aprendizaje. La revision de kits de enseñanza en ingenieria biomedica respalda evaluar accesibilidad, curricularidad, seguridad, costo y posibilidad de replicación, en vez de adoptar una plataforma solo por sus funciones tecnicas (Nandram & Foster, 2025).

## Implicaciones para requisitos iniciales

| Hallazgo documental | Necesidad a confirmar con usuarios | Requisito preliminar verificable |
|---|---|---|
| La medicion depende de la configuracion y la red de ensayo. | Comprender la secuencia y el significado de cada lectura. | La interfaz mostrara conexion, escenario, rango y advertencia antes de ejecutar una practica. |
| El aprendizaje activo requiere desempeño y retroalimentacion. | Recibir orientacion inmediata ante conexiones o decisiones inseguras. | El sistema presentara una lista de verificacion y actividades de prediccion-explicacion. |
| La arquitectura abierta necesita documentacion y control de cambios. | Inspeccionar y comprender los bloques sin acceder a energia peligrosa. | Se publicaran esquematicos de baja tension, firmware, BOM y guia segura de modificaciones. |
| Una lectura educativa no equivale a una medicion de conformidad. | Practicar responsablemente sin confundir el alcance del sistema. | La carcasa, interfaz y reporte incluiran la limitacion de uso didactico. |
| El diseño centrado en usuarios exige evidencia de contexto. | Ajustar el banco a tiempo, espacio, equipos y conocimientos disponibles. | Los objetivos de desempeño, costo y preparacion se fijaran tras encuesta, entrevistas e inventario. |

## Referencias

American Society for Engineering Education. (2025). *2025 ASEE annual conference and exposition proceedings*. https://peer.asee.org/

Bureau International des Poids et Mesures. (2022). *The International System of Units (SI brochure)* (9th ed., version 2.01). https://doi.org/10.59161/AUEZ1291

Chagas, A. M. (2018). Haves and have nots must find a better way: The case for open scientific hardware. *PLOS Biology, 16*(9), e3000014. https://doi.org/10.1371/journal.pbio.3000014

Design Council. (2019). *The framework for innovation: Design Council's evolved Double Diamond*. https://www.designcouncil.org.uk/our-resources/framework-for-innovation/

Deslauriers, L., McCarty, L. S., Miller, K., Callaghan, K., & Kestin, G. (2019). Measuring actual learning versus feeling of learning in response to being actively engaged in the classroom. *Proceedings of the National Academy of Sciences, 116*(39), 19251-19257. https://doi.org/10.1073/pnas.1821936116

Fluke Biomedical. (s. f.). *ESA615 electrical safety analyzer*. https://www.flukebiomedical.com/products/electrical-safety-analyzers/esa615-electrical-safety-analyzer

Galdames-Calderon, M., Pedersen, A. S., & Rodriguez-Gomez, D. (2024). Systematic review: Revisiting challenge-based learning teaching practices in higher education. *Education Sciences, 14*(9), 1008. https://doi.org/10.3390/educsci14091008

International Electrotechnical Commission. (2014). *IEC 62353:2014: Medical electrical equipment—Recurrent test and test after repair of medical electrical equipment*. https://webstore.iec.ch/en/publication/6913

International Electrotechnical Commission. (2016). *IEC 60990:2016: Methods of measurement of touch current and protective conductor current*. https://webstore.iec.ch/en/publication/24992

International Electrotechnical Commission. (2017). *IEC 61010-1:2010+AMD1:2016 CSV: Safety requirements for electrical equipment for measurement, control, and laboratory use—Part 1: General requirements*. https://webstore.iec.ch/en/publication/59769

International Electrotechnical Commission. (2018). *IEC 60479-1:2018: Effects of current on human beings and livestock—Part 1: General aspects*. https://webstore.iec.ch/en/publication/62980

International Electrotechnical Commission. (2020a). *IEC 60601-1:2005+AMD1:2012+AMD2:2020 CSV: Medical electrical equipment—Part 1: General requirements for basic safety and essential performance*. https://webstore.iec.ch/en/publication/67497

International Electrotechnical Commission. (2020b). *IEC 62366-1:2015/AMD1:2020: Medical devices—Part 1: Application of usability engineering to medical devices*. https://webstore.iec.ch/en/publication/66794

International Electrotechnical Commission. (2020c). *IEC 60601-1-2:2020: Medical electrical equipment—Part 1-2: General requirements for basic safety and essential performance—Collateral standard: Electromagnetic disturbances—Requirements and tests*. https://webstore.iec.ch/en/publication/65529

International Laboratory Accreditation Cooperation. (2019). *ILAC G8:09/2019: Guidelines on decision rules and statements of conformity*. https://ilac.org/publications-and-resources/ilac-guidance-series/

International Laboratory Accreditation Cooperation. (2020a). *ILAC P10:07/2020: ILAC policy on metrological traceability of measurement results*. https://ilac.org/publications-and-resources/ilac-policy-series/

International Laboratory Accreditation Cooperation. (2020b). *ILAC P14:09/2020: ILAC policy for measurement uncertainty in calibration*. https://ilac.org/publications-and-resources/ilac-policy-series/

International Organization for Standardization. (2016). *ISO 13485:2016: Medical devices—Quality management systems—Requirements for regulatory purposes*. https://www.iso.org/standard/59752.html

International Organization for Standardization. (2017). *ISO/IEC 17025:2017: General requirements for the competence of testing and calibration laboratories*. https://www.iso.org/standard/66912.html

International Organization for Standardization. (2018a). *ISO 31000:2018: Risk management—Guidelines*. https://www.iso.org/standard/65694.html

International Organization for Standardization. (2018b). *ISO 31010:2019: Risk management—Risk assessment techniques*. https://www.iso.org/standard/72140.html

International Organization for Standardization. (2019a). *ISO 14971:2019: Medical devices—Application of risk management to medical devices*. https://www.iso.org/standard/72704.html

International Organization for Standardization. (2019b). *ISO 9241-210:2019: Ergonomics of human-system interaction—Part 210: Human-centred design for interactive systems*. https://www.iso.org/standard/77520.html

International Organization for Standardization. (2020). *ISO/TR 24971:2020: Medical devices—Guidance on the application of ISO 14971*. https://www.iso.org/standard/74437.html

International Organization for Standardization. (2021). *ISO 15223-1:2021: Medical devices—Symbols to be used with information to be supplied by the manufacturer—Part 1: General requirements*. https://www.iso.org/standard/77326.html

Joint Committee for Guides in Metrology. (2008). *Evaluation of measurement data—Guide to the expression of uncertainty in measurement* (JCGM 100:2008). https://doi.org/10.59161/JCGM100-2008E

Lavado-Anguera, S., Velasco-Quintana, P.-J., & Terron-Lopez, M.-J. (2024). Project-based learning as an experiential pedagogical methodology in engineering education: A review of the literature. *Education Sciences, 14*(6), 617. https://doi.org/10.3390/educsci14060617

Ministerio de la Proteccion Social. (2005). *Decreto 4725 de 2005*. https://www.funcionpublica.gov.co/eva/gestornormativo/norma.php?i=17622

Ministerio de la Proteccion Social. (2008). *Resolucion 4816 de 2008*. https://normograma.invima.gov.co/normograma/compilacion/docs/resolucion_minproteccion_4816_2008.htm

National Academies of Sciences, Engineering, and Medicine. (2018). *How people learn II: Learners, contexts, and cultures*. National Academies Press. https://doi.org/10.17226/24783

Nandram, A. P., & Foster, J. A. (2025). Systematic review of teaching kits in biomedical engineering education. In *2025 ASEE annual conference and exposition proceedings*. https://doi.org/10.18260/1-2--57180

Oellermann, M., Jolles, J. W., Ortiz, D., Seabra, R., Wenzel, T., Wilson, H., & Tanner, R. L. (2022). Open hardware in science: The benefits of open electronics. *Integrative and Comparative Biology, 62*(4), 1061-1075. https://doi.org/10.1093/icb/icac043

Pearce, J. M. (2017). Emerging business models for open source hardware. *Journal of Open Hardware, 1*(1), 2. https://doi.org/10.5334/joh.4

Pronk Technologies. (s. f.). *Safe-T Sim electrical safety analyzer simulator*. https://www.pronktech.com/

Rigel Medical. (s. f.). *Rigel 288+ electrical safety analyzer*. https://www.rigelmedical.com/product/406a910-288-plus/

Santos-Diaz, A., Montesinos, L., Barrera-Esparza, M., del Mar Perez-Desentis, M., & Salinas-Navarro, D. E. (2024). Implementing a challenge-based learning experience in a bioinstrumentation blended course. *BMC Medical Education, 24*, 528. https://doi.org/10.1186/s12909-024-05462-7

U.S. Food and Drug Administration. (2016). *Applying human factors and usability engineering to medical devices: Guidance for industry and Food and Drug Administration staff*. https://www.fda.gov/media/80481/download

Ulrich, K. T., Eppinger, S. D., & Yang, M. C. (2020). *Product design and development* (7th ed.). McGraw-Hill Education.
