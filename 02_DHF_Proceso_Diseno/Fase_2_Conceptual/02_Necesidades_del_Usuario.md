# Lista de métricas técnicas

Las métricas técnicas permiten evaluar de forma objetiva si la solución de diseño responde a las necesidades identificadas durante el análisis de la experiencia de uso del equipo.

## Métricas

| # | Necesidad del usuario | Métrica | Unidad |
|---|---|---|---|
| 1 | Operar el equipo de manera segura | Tensión máxima accesible | V |
| 2 | Reducir el riesgo eléctrico | Corriente máxima accesible | mA |
| 3 | Identificar fácilmente las conexiones | Conexiones correctamente identificadas | % |
| 4 | Realizar correctamente el montaje | Montajes correctos en el primer intento | % |
| 5 | Configurar el equipo con facilidad | Tiempo de configuración | min |
| 6 | Comprender el estado del equipo | Estados del sistema identificables | unid. |
| 7 | Reconocer situaciones anormales | Tiempo de respuesta de la alerta | s |
| 8 | Saber cómo actuar ante un error | Errores con orientación de respuesta | % |
| 9 | Recibir información durante la práctica | Variables visibles durante la operación | unid. |
| 10 | Verificar el procedimiento realizado | Criterios de verificación disponibles | unid. |
| 11 | Comprobar los resultados obtenidos | Resultados verificables | % |
| 12 | Revisar posteriormente la práctica | Prácticas con información registrada | % |
| 13 | Acceder a registros anteriores | Tiempo de recuperación del registro | s |
| 14 | Desarrollar autonomía durante la práctica | Pasos que requieren asistencia | pasos |
| 15 | Realizar la práctica de manera sencilla | Número total de pasos | pasos |
| 16 | Tener una interacción predecible | Eventos inesperados por práctica | eventos/práctica |

## Criterios de evaluación

Las métricas se utilizarán para comparar y evaluar las diferentes alternativas de diseño. Dependiendo del desarrollo del proyecto, algunas métricas podrán modificarse o eliminarse cuando se definan con mayor precisión las funciones y características del prototipo.

### Tipos de evaluación

- **Seguridad:** mediciones y pruebas técnicas.
- **Funcionamiento:** pruebas controladas del sistema.
- **Usabilidad:** pruebas con usuarios.
- **Interacción:** observación de errores, tiempos y pasos necesarios.
- **Retroalimentación:** evaluación de la comprensión de alertas e información presentada.
- **Registro:** comprobación de la disponibilidad y recuperación de la información.

# B. Benchmarking Técnico

El benchmarking técnico permite identificar cómo los productos comerciales existentes responden a las necesidades identificadas en la Tabla A. Para ello, se seleccionaron tres analizadores de seguridad eléctrica para equipos electromédicos como referentes:

- **Fluke Biomedical ESA615**
- **Rigel Medical 288+**
- **Metrel MI 6601 MediTest**

Las características comparadas se relacionan directamente con las necesidades identificadas para el proyecto. De esta manera, el benchmarking permite reconocer qué soluciones ya existen y cuáles pueden ser consideradas como referencia para el desarrollo del prototipo.

> **Nota:** Cuando el fabricante no publica información suficiente para establecer una comparación cuantitativa, se utiliza una valoración cualitativa o se indica `No especificado`.

## Tabla de Benchmarking

| Necesidad A | Característica evaluada | Unidad / tipo | Fluke ESA615 | Rigel 288+ | Metrel MI 6601 |
|---|---|---|---|---|---|
| **N1. Operar el equipo de manera segura** | Prueba de continuidad de tierra de protección (PE) | Sí / No | Sí | Sí | Sí |
| **N2. Reducir el riesgo eléctrico** | Prueba de resistencia de aislamiento | Sí / No | Sí | Sí | Sí |
| **N2. Reducir el riesgo eléctrico** | Pruebas de corriente de fuga | Sí / No | Sí | Sí | Sí |
| **N2. Reducir el riesgo eléctrico** | Corriente de prueba de PE | mA / A | >200 mA* | >200 mA | 200 mA / 25 A |
| **N3. Identificar fácilmente las conexiones** | Identificación/configuración de conexiones para partes aplicadas | Sí / No | No especificado | No especificado | Sí |
| **N4. Realizar correctamente el montaje** | Verificación de conexiones durante la prueba | Sí / No | Sí | Sí | Sí |
| **N5. Configurar el equipo con facilidad** | Secuencias de prueba configurables | Sí / No | Sí | Sí | Sí |
| **N6. Comprender el estado del equipo** | Visualización del estado de la prueba | Sí / No | Sí | Sí | Sí |
| **N7. Reconocer situaciones anormales** | Indicación de condiciones de error | Sí / No | Sí | Sí | Sí |
| **N8. Saber cómo actuar ante un error** | Orientación durante la ejecución de la prueba | Sí / No | Sí | Sí | Sí |
| **N9. Recibir información durante la práctica** | Visualización de parámetros de medición | Sí / No | Sí | Sí | Sí |
| **N10. Verificar el procedimiento realizado** | Secuencias de prueba guiadas | Sí / No | Sí | Sí | Sí |
| **N11. Comprobar los resultados** | Visualización de resultados de prueba | Sí / No | Sí | Sí | Sí |
| **N12. Revisar posteriormente la práctica** | Almacenamiento de resultados | Sí / No | Sí | Sí | Sí |
| **N13. Acceder fácilmente a registros anteriores** | Recuperación de resultados almacenados | Sí / No | Sí | Sí | Sí |
| **N14. Desarrollar autonomía durante la práctica** | Automatización de secuencias | Sí / No | Sí | Sí | Sí |
| **N15. Realizar la práctica de manera sencilla** | Procedimientos/secuencias predefinidas | Sí / No | Sí | Sí | Sí |
| **N16. Tener una interacción predecible** | Ejecución estructurada de las pruebas | Sí / No | Sí | Sí | Sí |

\* El valor exacto depende de la configuración y método de prueba especificado por el fabricante.

## Características técnicas adicionales de referencia

Además de las características relacionadas directamente con las necesidades del usuario, se identificaron variables técnicas que permiten establecer el nivel de desempeño de los equipos existentes.

| Característica | Unidad | Fluke ESA615 | Rigel 288+ | Metrel MI 6601 |
|---|---|---|---|---|
| Tensión de prueba de aislamiento | VDC | 250 / 500 | 50 / 100 / 250 / 500 | 250 / 500 |
| Rango de resistencia de aislamiento | MΩ | 0,5–100 | 0,01–100 | No especificado |
| Fuga directa | Sí / No | Sí | Sí | Sí |
| Fuga diferencial | Sí / No | Sí | Sí | Sí |
| Fuga alternativa | Sí / No | Sí | Sí | Sí |
| Resolución de fuga | µA | No especificado | 1 | 1 |
| Secuencias automáticas | Sí / No | Sí | Sí | Sí |
| Registro de resultados | Sí / No | Sí | Sí | Sí |
| Comunicación con computador | Sí / No | Sí | Sí | Sí |
| Prueba de partes aplicadas | Sí / No | Sí | Sí | Sí |
| Arquitectura abierta documentada | Sí / No | No evidenciada | No evidenciada | No evidenciada |

## Interpretación del Benchmarking

El benchmarking permite observar que las necesidades identificadas en la Tabla A ya cuentan con diferentes soluciones implementadas en analizadores comerciales.

Las necesidades relacionadas con **seguridad** se abordan principalmente mediante pruebas de continuidad de tierra, aislamiento y corrientes de fuga.

Las necesidades relacionadas con **conexión y configuración** se abordan mediante diferentes configuraciones de prueba, conexiones para partes aplicadas y secuencias configurables.

Las necesidades relacionadas con **información y retroalimentación** se abordan mediante interfaces que muestran el estado de la prueba, las mediciones y los resultados.

Las necesidades relacionadas con **autonomía y facilidad de uso** se abordan mediante secuencias predefinidas y automatización de procedimientos.

Finalmente, las necesidades relacionadas con **registro y seguimiento** se abordan mediante almacenamiento de resultados y comunicación con sistemas externos.

Sin embargo, las características comerciales están principalmente orientadas a la ejecución profesional de pruebas. El proyecto propone incorporar estas capacidades dentro de un contexto de **aprendizaje práctico**, además de mantener una **arquitectura abierta y documentada**.

## Referencias

[1] Fluke Biomedical. *ESA615 Electrical Safety Analyzer*.  
https://www.flukebiomedical.com/products/electrical-safety-analyzers/esa615-electrical-safety-analyzer

[2] Rigel Medical. *Rigel 288+ Electrical Safety Analyzer*.  
https://www.rigelmedical.com/product/406a910-288-plus/

[3] Metrel. *MI 6601 MediTest – Medical Electrical Safety Tester*.  
https://www.metrel.si/en/shop/PAT/medical-testers/mi-6601-meditest.html
# C. Tabla de especificaciones objetivo

Las especificaciones objetivo se establecen a partir de las necesidades identificadas en la Tabla A y de las características observadas en el benchmarking técnico de la Tabla B.

Cada especificación representa una característica que el prototipo deberá alcanzar para responder a una o más necesidades del usuario.

| N.º | Necesidad relacionada | Especificación objetivo | Métrica | Unidad | Dirección de mejora | Valor marginal | Valor ideal | Método de verificación |
|---:|---|---|---|---|---|---|---|---|
| 1 | N1. Operar el equipo de manera segura | El prototipo debe permitir realizar las pruebas de seguridad eléctrica definidas en el alcance | Pruebas implementadas | unid. | Aumentar | Pruebas básicas definidas | Todas las pruebas definidas | Verificación funcional |
| 2 | N2. Reducir el riesgo eléctrico | El prototipo debe incorporar mecanismos de protección durante la ejecución de las pruebas | Mecanismos de protección implementados | unid. | Aumentar | Protecciones básicas | Protección integral | Pruebas eléctricas |
| 3 | N3. Identificar fácilmente las conexiones | Las conexiones deben estar claramente identificadas | Conexiones correctamente identificadas | % | Aumentar | ≥ 90 % | ≥ 98 % | Prueba con usuarios |
| 4 | N4. Realizar correctamente el montaje | El sistema debe facilitar la realización correcta del montaje | Montajes correctos en el primer intento | % | Aumentar | ≥ 80 % | ≥ 95 % | Prueba con usuarios |
| 5 | N5. Configurar el equipo con facilidad | El sistema debe permitir seleccionar y configurar las pruebas | Tiempo de configuración | min | Disminuir | ≤ 10 min | ≤ 5 min | Prueba de usabilidad |
| 6 | N6. Comprender el estado del equipo | El sistema debe mostrar claramente su estado de operación | Estados identificables | % | Aumentar | ≥ 90 % | 100 % | Prueba con usuarios |
| 7 | N7. Reconocer situaciones anormales | El sistema debe detectar e indicar condiciones anormales | Tiempo de respuesta de alerta | s | Disminuir | ≤ 2 s | ≤ 1 s | Prueba funcional |
| 8 | N8. Saber cómo actuar ante un error | El sistema debe proporcionar información sobre el error y la acción requerida | Errores con orientación | % | Aumentar | ≥ 80 % | 100 % | Prueba de usabilidad |
| 9 | N9. Recibir información durante la práctica | El sistema debe mostrar las variables necesarias para interpretar la prueba | Variables visibles | unid. | Aumentar | Variables esenciales | Todas las variables relevantes | Inspección funcional |
| 10 | N10. Verificar el procedimiento realizado | El sistema debe proporcionar indicaciones para comprobar cada etapa | Criterios de verificación | unid. | Aumentar | ≥ 3 | Todos los definidos | Prueba funcional |
| 11 | N11. Comprobar los resultados | Los resultados obtenidos deben poder ser comparados con valores de referencia | Resultados verificables | % | Aumentar | ≥ 90 % | 100 % | Comparación con referencia |
| 12 | N12. Revisar posteriormente la práctica | El sistema debe almacenar la información generada durante la práctica | Prácticas registradas | % | Aumentar | ≥ 90 % | 100 % | Prueba de almacenamiento |
| 13 | N13. Acceder fácilmente a registros anteriores | Los registros deben poder localizarse y visualizarse rápidamente | Tiempo de recuperación | s | Disminuir | ≤ 30 s | ≤ 10 s | Prueba de usabilidad |
| 14 | N14. Desarrollar autonomía | El sistema debe permitir realizar la práctica sin asistencia constante | Pasos que requieren asistencia | pasos | Disminuir | ≤ 3 | 0 | Prueba con usuarios |
| 15 | N15. Realizar la práctica de manera sencilla | El procedimiento debe reducir pasos y acciones innecesarias | Número total de pasos | pasos | Disminuir | ≤ 15 | ≤ 10 | Análisis del procedimiento |
| 16 | N16. Tener una interacción predecible | El sistema debe mantener una secuencia de operación clara y consistente | Eventos inesperados por práctica | eventos/práctica | Disminuir | ≤ 2 | 0 | Pruebas repetidas |
