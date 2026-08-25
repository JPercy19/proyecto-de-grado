# Necesidades identificadas y objetivos de diseño

## Objetivo de diseño

Diseñar una plataforma didáctica de arquitectura abierta que permita a estudiantes practicar, de manera segura y supervisada, la preparación, configuración, ejecución e interpretación de pruebas seleccionadas de seguridad eléctrica en escenarios controlados, tomando como referencia IEC 60601-1 e IEC 62353.

El objetivo se limita a aprendizaje práctico. No busca sustituir un analizador calibrado, certificar dispositivos, liberar equipos para uso clínico ni conectar el sistema a pacientes. Esta delimitación orienta las decisiones de seguridad y evita presentar resultados educativos como evidencia de conformidad.

## Necesidades preliminares

Las necesidades están redactadas desde el punto de vista de los usuarios y no imponen todavía una solución. Se priorizarán después de aplicar la indagación social.

| Codigo | Necesidad | Justificacion |
|---|---|---|
| N-01 | El usuario necesita practicar sin exposición a energía peligrosa. | El aprendizaje no debe introducir riesgos inaceptables de contacto, conexión o energía residual. |
| N-02 | El usuario necesita comprender la secuencia y el fundamento de cada prueba. | Una lectura aislada no explica el fenómeno, el montaje ni su límite de interpretación. |
| N-03 | El usuario necesita identificar configuraciones incorrectas antes de ejecutar una práctica. | La retroalimentación temprana favorece una operación responsable. |
| N-04 | El usuario necesita observar una arquitectura documentada y modificable de forma segura. | La apertura permite relacionar bloques, señales y software sin acceso a partes peligrosas. |
| N-05 | El usuario necesita registrar el escenario, procedimiento y resultado de una práctica. | El registro permite discutir, repetir y evaluar la actividad. |
| N-06 | El docente necesita preparar, supervisar y evaluar la práctica en el tiempo disponible. | La herramienta debe funcionar dentro de las restricciones reales del laboratorio. |
| N-07 | El laboratorio necesita una solución mantenible, reparable y compatible con sus recursos. | La viabilidad incluye costo de materiales, repuestos, almacenamiento y mantenimiento. |
| N-08 | Todos los usuarios necesitan distinguir el alcance educativo de una evaluación profesional. | Una lectura sin trazabilidad ni incertidumbre no puede emplearse para declarar conformidad. |

## Objetivos específicos de diseño

1. Implementar escenarios de práctica con simuladores, cargas protegidas o equipos autorizados, sin paciente conectado.
2. Guiar al estudiante mediante una secuencia visible de preparación, conexión, ejecución, interpretación y cierre.
3. Hacer visibles los bloques de baja energía asociados a control, adquisición, visualización y registro, junto con su documentación técnica.
4. Incorporar controles de seguridad, advertencias y restricciones de acceso definidos por el análisis de riesgo.
5. Registrar información suficiente para reconstruir una práctica didáctica, incluyendo identificación del escenario, configuración, usuario codificado, fecha y resultado.
6. Diseñar módulos reparables y documentados, con una lista de materiales y procedimientos de mantenimiento.
7. Evaluar el desempeño pedagógico y la usabilidad del prototipo sin afirmar certificación normativa.

## Traducción a atributos y métodos de verificación

| Necesidad | Atributo técnico preliminar | Unidad o criterio | Verificación |
|---|---|---|---|
| N-01 | Barreras, aislamiento, enclavamientos y descarga de energía implementados. | Cumple/no cumple según análisis de riesgo. | Inspección, prueba segura y revisión documental. |
| N-02 | Cobertura de escenarios y pasos explicados. | Número de escenarios y porcentaje de pasos guiados. | Prueba de tareas y rúbrica conceptual. |
| N-03 | Detección o confirmación de configuración previa. | Porcentaje de errores detectados en escenarios definidos. | Prueba con fallas simuladas. |
| N-04 | Documentación de módulos seguros disponible. | Porcentaje de documentos publicados y versionados. | Revisión de esquemáticos, BOM, firmware y guía. |
| N-05 | Campos de registro por práctica. | Número de campos obligatorios. | Exportación y revisión de reporte. |
| N-06 | Tiempo de preparación y facilidad de evaluación. | Minutos y resultado de prueba de usabilidad. | Cronometraje y cuestionario docente. |
| N-07 | Costo, modularidad y disponibilidad de repuestos. | COP, número de módulos reemplazables y proveedores. | Presupuesto y BOM. |
| N-08 | Comunicación explícita del alcance educativo. | Presencia de advertencia en carcasa, interfaz y reporte. | Inspección de interfaz y documentación. |

## Restricciones no negociables

- El prototipo no se conectará a pacientes.
- No se usará para aprobar, liberar o diagnosticar equipos clínicos.
- La primera fase de pruebas se realizará con simuladores de baja energía o cargas expresamente diseñadas para docencia.
- Las zonas asociadas a red eléctrica, si se consideran en una fase posterior, requerirán análisis de riesgo, barreras físicas, control de acceso y supervisión docente.
- Las métricas de exactitud, incertidumbre y conformidad solo podrán definirse tras seleccionar la arquitectura y contar con medios de calibración adecuados.

## Priorizacion pendiente de campo

La importancia relativa de N-01 a N-08 se obtendrá de la encuesta, entrevistas e inventario. La seguridad será una restricción y no se compensará con puntajes de costo o conveniencia. Las necesidades restantes se priorizarán mediante importancia de usuarios, frecuencia de evidencia, impacto pedagógico, viabilidad y costo; el resultado alimentará la Casa de la Calidad.
