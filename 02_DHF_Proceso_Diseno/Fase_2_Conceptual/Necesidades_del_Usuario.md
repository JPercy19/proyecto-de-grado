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

El benchmarking técnico permite comparar las necesidades y características de interacción identificadas para el proyecto con diferentes analizadores comerciales de seguridad eléctrica utilizados como referentes.

Los productos seleccionados son:

- **Fluke Biomedical ESA615**
- **Rigel Medical 288+**
- **Metrel MI 6601 MediTest**

Estos equipos fueron seleccionados debido a que incorporan diferentes pruebas de seguridad eléctrica para equipos electromédicos y cuentan con funciones relacionadas con IEC 60601-1 e IEC 62353.

> **Nota:** Cuando una característica relacionada con la experiencia de usuario no se encuentra publicada por el fabricante, se indica como **No publicado**. No se realizan estimaciones de variables de usabilidad sin evidencia disponible.

## Tabla de Benchmarking

| N.º | Métrica técnica | Unidad | Fluke ESA615 | Rigel 288+ | Metrel MI 6601 |
|---:|---|---|---|---|---|
| 1 | Tensión máxima accesible durante la operación | V | No publicado | No publicado | No publicado |
| 2 | Corriente máxima accesible durante la operación | mA | No publicado | No publicado | No publicado |
| 3 | Conexiones correctamente identificadas | % | No publicado | No publicado | No publicado |
| 4 | Montajes correctos en el primer intento | % | No publicado | No publicado | No publicado |
| 5 | Tiempo de configuración del sistema | min | No publicado | No publicado | No publicado |
| 6 | Estados del sistema identificables | unid. | Sí | Sí | Sí |
| 7 | Tiempo de respuesta de la indicación de alerta | s | No publicado | No publicado | No publicado |
| 8 | Errores con orientación de respuesta | % | No publicado | Sí | Sí |
| 9 | Variables visibles durante la operación | unid. | No publicado | No publicado | No publicado |
| 10 | Criterios de verificación disponibles | unid. | Sí | Sí | Sí |
| 11 | Resultados verificables | % | Sí | Sí | Sí |
| 12 | Prácticas con información registrada | % | Sí | Sí | Sí |
| 13 | Tiempo de recuperación de un registro | s | No publicado | No publicado | No publicado |
| 14 | Pasos que requieren asistencia externa | pasos | No publicado | No publicado | No publicado |
| 15 | Número total de pasos del procedimiento | pasos | No publicado | No publicado | No publicado |
| 16 | Eventos inesperados por práctica | eventos/práctica | No publicado | No publicado | No publicado |

## Funciones observadas en los referentes

Aunque los fabricantes no publican todas las métricas de experiencia de usuario, sí es posible identificar características relevantes que permiten interpretar el benchmarking.

| Característica | Fluke ESA615 | Rigel 288+ | Metrel MI 6601 |
|---|:---:|:---:|:---:|
| Pruebas de seguridad eléctrica | Sí | Sí | Sí |
| IEC 60601-1 | Sí | Sí | Sí |
| IEC 62353 | Sí | Sí | Sí |
| Continuidad de tierra | Sí | Sí | Sí |
| Resistencia de aislamiento | Sí | Sí | Sí |
| Corrientes de fuga | Sí | Sí | Sí |
| Secuencias de prueba | Sí | Sí | Sí |
| Secuencias configurables | Sí | Sí | Sí |
| Registro de resultados | Sí | Sí | Sí |
| Comunicación con computador | Sí | Sí | Sí |
| Guía durante la prueba | Sí | Sí | Sí |
| Conexiones configurables | No publicado | No publicado | Sí |
| Arquitectura abierta | No evidenciada | No evidenciada | No evidenciada |

## Interpretación

El benchmarking muestra que los equipos comerciales cuentan con un conjunto importante de funciones destinadas a facilitar la ejecución de pruebas de seguridad eléctrica.

Entre las características comunes se encuentran:

- Ejecución de diferentes pruebas de seguridad eléctrica.
- Pruebas asociadas a IEC 60601-1 e IEC 62353.
- Secuencias de prueba.
- Registro de resultados.
- Orientación durante la ejecución.
- Configuración de diferentes pruebas.

Sin embargo, los fabricantes no publican normalmente métricas de usabilidad como el porcentaje de montajes correctos en el primer intento, el tiempo de configuración o el número de pasos que requieren asistencia.

Estas variables representan una oportunidad para el proyecto, ya que el prototipo tiene como propósito adicional facilitar el **aprendizaje práctico** y no únicamente realizar las mediciones.

El benchmarking permite, por tanto, tomar las capacidades de los equipos comerciales como referencia funcional y evaluar posteriormente si el prototipo puede ofrecer una interacción más adecuada para un contexto educativo.

### Referencias

[1] Fluke Biomedical. *ESA615 Electrical Safety Analyzer*.  
https://www.flukebiomedical.com/products/electrical-safety-analyzers/esa615-electrical-safety-analyzer

[2] Rigel Medical. *Rigel 288+ Electrical Safety Analyzer*.  
https://www.rigelmedical.com/product/406a910-288-plus/

[3] Metrel. *MI 6601 MediTest – Medical Electrical Safety Tester*.  
https://www.metrel.si/en/shop/PAT/medical-testers/mi-6601-meditest.html

# C. Tabla de especificaciones objetivo

Las especificaciones objetivo establecen las metas que deberá alcanzar el prototipo a partir de las necesidades identificadas y del benchmarking realizado.

Los valores definidos corresponden a **objetivos de diseño del prototipo**. No deben interpretarse como valores de certificación o como sustitutos de los límites establecidos por IEC 60601-1 o IEC 62353.

## Tabla de especificaciones objetivo

| N.º | Métrica técnica | Unidad | Dirección de mejora | Valor marginal | Valor ideal | Método de verificación |
|---:|---|---|---|---|---|---|
| 1 | Tensión máxima accesible durante la operación | V | Disminuir | ≤ 50 V en partes accesibles | Minimizar exposición a tensión peligrosa | Medición de tensión en partes accesibles durante diferentes condiciones de operación. |
| 2 | Corriente máxima accesible durante la operación | mA | Disminuir | ≤ 1 mA | Minimizar corriente accesible | Medición de corriente en puntos accesibles bajo condiciones de prueba controladas. |
| 3 | Conexiones correctamente identificadas | % | Aumentar | ≥ 90 % | ≥ 98 % | Prueba con usuarios realizando conexiones y registro de conexiones correctas. |
| 4 | Montajes correctos en el primer intento | % | Aumentar | ≥ 80 % | ≥ 95 % | Evaluación con usuarios realizando el montaje sin asistencia. |
| 5 | Tiempo de configuración del sistema | min | Disminuir | ≤ 10 min | ≤ 5 min | Medir el tiempo desde el inicio del montaje hasta que el sistema esté listo para ejecutar la prueba. |
| 6 | Estados del sistema identificables | unid. | Aumentar | Todos los estados principales | Todos los estados relevantes | Evaluar mediante prueba de reconocimiento de estados por parte de los usuarios. |
| 7 | Tiempo de respuesta de la indicación de alerta | s | Disminuir | ≤ 2 s | ≤ 1 s | Medir el tiempo entre la aparición de la condición anormal y la generación de la alerta. |
| 8 | Errores con orientación de respuesta | % | Aumentar | ≥ 80 % | 100 % | Provocar errores controlados y verificar que el sistema indique una acción de respuesta. |
| 9 | Variables visibles durante la operación | unid. | Aumentar | Variables necesarias para la prueba | Todas las variables relevantes | Verificar que las variables necesarias para interpretar la prueba estén disponibles durante su ejecución. |
| 10 | Criterios de verificación disponibles | unid. | Aumentar | ≥ 3 criterios | Todos los criterios definidos para cada prueba | Revisar las indicaciones disponibles para comprobar la correcta ejecución de cada procedimiento. |
| 11 | Resultados verificables | % | Aumentar | ≥ 90 % | 100 % | Comparar los resultados obtenidos con valores de referencia conocidos. |
| 12 | Prácticas con información registrada | % | Aumentar | ≥ 90 % | 100 % | Ejecutar prácticas y comprobar que los resultados queden almacenados correctamente. |
| 13 | Tiempo de recuperación de un registro | s | Disminuir | ≤ 30 s | ≤ 10 s | Medir el tiempo necesario para localizar y visualizar una práctica almacenada. |
| 14 | Pasos que requieren asistencia externa | pasos | Disminuir | ≤ 3 pasos | 0 pasos | Observar una práctica realizada por un usuario sin asistencia directa. |
| 15 | Número total de pasos del procedimiento | pasos | Disminuir | ≤ 15 pasos | ≤ 10 pasos | Contabilizar los pasos necesarios para completar una práctica representativa. |
| 16 | Eventos inesperados por práctica | eventos/práctica | Disminuir | ≤ 2 | 0 | Registrar comportamientos inesperados durante pruebas repetidas del sistema. |

## Criterios de interpretación

### Valor marginal

El valor marginal representa el nivel mínimo de desempeño que debería alcanzar el prototipo para considerar que la característica cumple de manera aceptable con el objetivo de diseño.

### Valor ideal

El valor ideal representa el desempeño deseado para obtener una experiencia de uso más segura, clara y autónoma.

### Dirección de mejora

- **Aumentar:** un valor mayor representa una mejora.
- **Disminuir:** un valor menor representa una mejora.

## Consideraciones

Los valores objetivo relacionados con seguridad eléctrica deberán revisarse y validarse durante el diseño electrónico y las pruebas experimentales. Los límites definitivos de seguridad no deben establecerse únicamente a partir del benchmarking comercial.

Las métricas de interacción y usabilidad deberán validarse mediante pruebas con usuarios, mientras que las métricas eléctricas deberán verificarse mediante mediciones instrumentales y procedimientos de prueba controlados.

El objetivo del proyecto es desarrollar un **prototipo de analizador de seguridad eléctrica de arquitectura abierta para el aprendizaje práctico**, por lo que el desempeño técnico debe evaluarse junto con la facilidad de comprensión, configuración, ejecución y revisión de las pruebas.

> **Importante:** alcanzar los valores objetivo definidos en esta tabla no implica que el prototipo esté certificado ni que pueda utilizarse como sustituto de un analizador comercial certificado.
