# Indagacion social, necesidades y objetivos de diseño

## Objetivo de la indagacion

Caracterizar las condiciones de aprendizaje, seguridad y uso que condicionan el diseño de una plataforma didactica para pruebas de seguridad electrica. La indagacion no busca demostrar que el prototipo es un analizador profesional ni recolectar información clínica. Sus resultados permitirán convertir voces, comportamientos y restricciones del contexto en necesidades y atributos de diseño.

## Participantes y consideraciones eticas

| Grupo | Criterio de inclusion | Aporte esperado | Datos a conservar |
|---|---|---|---|
| Estudiantes | Estar cursando o haber cursado una asignatura relacionada con instrumentacion, mantenimiento o seguridad electrica. | Dificultades, conocimientos previos, disponibilidad y expectativas de aprendizaje. | Encuesta anonima y consentimiento si la institucion lo solicita. |
| Docentes | Impartir o coordinar asignaturas relacionadas. | Resultados de aprendizaje, secuencias de practica, criterios de seguridad y restricciones academicas. | Entrevista autorizada, transcripcion anonima y matriz de codigos. |
| Personal tecnico | Tener experiencia pertinente en mantenimiento o ingenieria clinica. | Errores frecuentes, procedimientos, condiciones de uso y límites del prototipo. | Entrevista autorizada y notas anonimizadas. |
| Laboratorio | Espacio autorizado para las practicas. | Inventario, redes disponibles, normas, espacio, almacenamiento y supervision. | Lista de verificacion, fotografias autorizadas y acta de observacion. |

Antes de recolectar datos, se debe obtener autorización del docente o instancia institucional correspondiente. No se recopilarán nombres en la base de análisis, datos clínicos ni información sensible de equipos hospitalarios. Las respuestas se identificarán con códigos y se conservarán solo durante el periodo aprobado.

## Diseño metodologico

Se aplicará un enfoque mixto secuencial. Primero se revisan normas, literatura y manuales; después se recoge evidencia del contexto mediante entrevistas, encuesta e inventario; finalmente se triangulan hallazgos para formular requisitos. La combinación evita que una necesidad se defina únicamente desde la opinión del equipo de diseño.

| Actividad | Producto | Analisis | Salida de diseño |
|---|---|---|---|
| Revision documental | Fichas de fuentes y benchmark. | Comparacion de funciones, riesgos y enfoques pedagogicos. | Restricciones normativas y criterios de evaluación. |
| Entrevistas | Audios/notas autorizadas y transcripciones anonimas. | Codificacion temática: seguridad, aprendizaje, operación, recursos y apertura. | Necesidades expresadas y escenarios de uso. |
| Encuesta | Base anonima de respuestas. | Frecuencias, mediana por ítem y analisis de preguntas abiertas. | Priorizacion inicial de necesidades. |
| Observacion/inventario | Lista de verificación y evidencia autorizada. | Brechas entre tarea, recursos y seguridad del espacio. | Restricciones reales de tamaño, preparación y supervisión. |
| Triangulacion | Matriz evidencia-necesidad-requisito. | Confirmacion, contradiccion o ajuste de cada hallazgo. | Lista de necesidades y atributos técnicos. |

## Guion de entrevista semiestructurada

1. ¿Qué competencias debe demostrar un estudiante antes de utilizar un analizador profesional de seguridad eléctrica?
2. ¿Qué pruebas, configuraciones o conceptos generan más dificultades durante la práctica?
3. ¿Qué errores de conexión, operación o interpretación se presentan con mayor frecuencia?
4. ¿Qué restricciones de tiempo, equipos, presupuesto, espacio y supervisión condicionan las prácticas?
5. ¿Qué información debe mostrarse para que el estudiante comprenda el principio de una medición?
6. ¿Qué escenarios de baja energía o simuladores serían apropiados para una primera práctica?
7. ¿Qué controles harían inseguro o inaceptable el prototipo?
8. ¿Qué evidencia permitiría concluir que una práctica mejoró el aprendizaje?

## Encuesta para estudiantes

Escala: 1 = totalmente en desacuerdo; 2 = en desacuerdo; 3 = ni de acuerdo ni en desacuerdo; 4 = de acuerdo; 5 = totalmente de acuerdo.

| Codigo | Enunciado | Dimension |
|---|---|---|
| E-01 | Comprendo la diferencia entre continuidad de tierra y corriente de fuga. | Conocimiento conceptual |
| E-02 | Puedo identificar riesgos antes de conectar un equipo a un analizador. | Seguridad |
| E-03 | He tenido suficiente tiempo de práctica con instrumentos de seguridad eléctrica. | Acceso |
| E-04 | La interfaz disponible me ayuda a comprender cómo se obtiene cada medición. | Comprensibilidad |
| E-05 | Me sería útil observar los bloques funcionales y la secuencia de una prueba. | Arquitectura abierta |
| E-06 | Necesito retroalimentación inmediata sobre conexiones o configuraciones incorrectas. | Retroalimentación |
| E-07 | Considero importante registrar procedimiento, configuración y resultado de cada práctica. | Trazabilidad didáctica |
| E-08 | Me sentiría capaz de explicar por qué un resultado cambia al modificar un escenario de falla simulado. | Transferencia |

Preguntas abiertas: “¿Qué aspecto le resulta más difícil al realizar o interpretar una prueba?” y “¿Qué característica haría más útil y segura una plataforma de práctica?”. Se reportará el número de respuestas válidas, periodo de aplicación, perfil agregado de participantes y resultados sin identificar personas. No se fabricarán porcentajes, citas ni conclusiones antes de recolectar los datos.

## Lista inicial de necesidades

Estas necesidades son hipótesis de diseño documentadas. La fuente definitiva, importancia y evidencia se completarán con los resultados de indagación.

| Codigo | Necesidad expresada sin imponer solución | Evidencia documental inicial | Evidencia de campo requerida |
|---|---|---|---|
| N-01 | Practicar sin exposición a partes peligrosas ni ambigüedad sobre el uso permitido. | IEC 60601-1, ISO 14971. | Riesgos y controles señalados por docentes y técnicos. |
| N-02 | Comprender la secuencia, el principio y las limitaciones de cada prueba. | IEC 60990; aprendizaje activo. | Dificultades reportadas por estudiantes. |
| N-03 | Recibir retroalimentación ante una conexión, selección o interpretación incorrecta. | Diseño centrado en usuarios y aprendizaje por retos. | Errores frecuentes observados. |
| N-04 | Visualizar una arquitectura documentada que pueda inspeccionarse de forma segura. | Hardware abierto. | Interés y nivel de conocimiento previo. |
| N-05 | Registrar una práctica reproducible con contexto suficiente para discutir el resultado. | Trazabilidad metrológica y aprendizaje reflexivo. | Campos que docentes requieren evaluar. |
| N-06 | Preparar y guardar el sistema dentro del tiempo, espacio y recursos del laboratorio. | Indagación contextual. | Inventario, tiempos y restricciones reales. |
| N-07 | Distinguir una demostración educativa de una prueba de conformidad profesional. | ISO/IEC 17025 e ILAC G8. | Comprensión de alcance y señales necesarias. |

## Criterios de priorizacion y trazabilidad

Cada necesidad se calificará por importancia para los usuarios (1-5), frecuencia de evidencia, impacto sobre seguridad y viabilidad técnica. No se promediarán respuestas de grupos distintos sin informar su composición. Un requisito solo será “priorizado” cuando la matriz conserve la fuente, fecha, código de evidencia, decisión y responsable.

| Hallazgo verificable | Fuente y codigo | Necesidad | Atributo o requisito posterior | Estado |
|---|---|---|---|---|
| [Completar después de campo] | [E-xx / D-xx / I-xx] | [N-xx] | [Métrica, unidad y método de verificación] | Pendiente |

## Plan de evaluacion didactica

La validación no medirá conformidad clínica. Se comparará el desempeño antes y después de una práctica autorizada mediante: prueba corta de conceptos, rúbrica de conexión segura, observación de secuencia, registro de errores, tiempo de preparación, cuestionario de usabilidad y una pregunta de explicación del resultado. La evidencia debe mostrar tanto aprendizaje como comprensión de los límites del prototipo.
