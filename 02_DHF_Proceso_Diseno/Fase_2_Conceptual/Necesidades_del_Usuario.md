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

El benchmarking técnico permite comparar las características y capacidades de diferentes analizadores comerciales de seguridad eléctrica para equipos electromédicos. Los referentes seleccionados se utilizan como punto de comparación para identificar funciones relevantes para el desarrollo del prototipo.

Los productos seleccionados corresponden a:

- **Fluke Biomedical ESA615**
- **Rigel Medical 288+**
- **Metrel MI 6601 MediTest**

Las características comparadas se relacionan principalmente con las pruebas contempladas en **IEC 60601-1** e **IEC 62353**, además de funciones de automatización, registro de resultados, comunicación y configuración.

> **Nota:** Los valores del benchmarking corresponden a las especificaciones publicadas por los fabricantes. Cuando una característica no se encuentra claramente especificada en la documentación consultada, se indica como `No especificado`.

### Tabla de Benchmarking Técnico

| N.º | Métrica técnica | Unidad | Fluke ESA615 | Rigel 288+ | Metrel MI 6601 | Fuente |
|---:|---|---|---|---|---|---|
| 1 | Soporte de IEC 60601-1 | Sí / No | Sí | Sí | Sí | [1][2][3] |
| 2 | Soporte de IEC 62353 | Sí / No | Sí | Sí | Sí | [1][2][3] |
| 3 | Prueba de continuidad de tierra de protección (PE) | Sí / No | Sí | Sí | Sí | [1][2][3] |
| 4 | Corriente de prueba de PE | mA / A | >200 mA | >200 mA | 200 mA / 25 A | [1][2][3] |
| 5 | Prueba de resistencia de aislamiento | Sí / No | Sí | Sí | Sí | [1][2][3] |
| 6 | Tensiones de prueba de aislamiento | VDC | 250 / 500 | 50 / 100 / 250 / 500 | 250 / 500 | [1][2][3] |
| 7 | Medición de corriente de fuga directa | Sí / No | Sí | Sí | Sí | [1][2][3] |
| 8 | Medición de corriente de fuga diferencial | Sí / No | Sí | Sí | Sí | [1][2][3] |
| 9 | Medición de corriente de fuga alternativa | Sí / No | Sí | Sí | Sí | [1][2][3] |
| 10 | Resolución de medición de fuga | µA | 0,1 µA* | 1 µA | 1 µA | [1][2][3] |
| 11 | Rango de medición de fuga | µA | Hasta 10.000 | Hasta 9.999* | No especificado | [1][2][3] |
| 12 | Medición de tensión de red | VAC | 90–264 | 0–300 | Sí | [1][2][3] |
| 13 | Medición de corriente del equipo | A | 0–20 | 0–16 | Sí | [1][2][3] |
| 14 | Secuencias de prueba automatizadas | Sí / No | Sí | Sí | Sí | [1][2][3] |
| 15 | Secuencias de prueba configurables | Sí / No | Sí | Sí | Sí | [1][2][3] |
| 16 | Almacenamiento de resultados | Sí / No | Sí | Sí | Sí | [1][2][3] |
| 17 | Comunicación con computador | Sí / No | Sí | Sí | Sí | [1][2][3] |
| 18 | Configuración para diferentes partes aplicadas | Sí / No | No especificado | No especificado | Sí | [3] |
| 19 | Interfaz para guiar la ejecución de pruebas | Sí / No | Sí | Sí | Sí | [1][2][3] |
| 20 | Arquitectura abierta documentada | Sí / No | No evidenciada | No evidenciada | No evidenciada | [1][2][3] |

\* Los valores pueden depender del método de prueba o de las condiciones especificadas por el fabricante.

### Referentes

**Fluke Biomedical ESA615**  
Analizador portátil de seguridad eléctrica para equipos médicos que incorpora pruebas de tierra de protección, aislamiento, corrientes de fuga y otras pruebas relacionadas con seguridad eléctrica.

**Rigel Medical 288+**  
Analizador orientado a pruebas de seguridad eléctrica de equipos médicos, con diferentes métodos de medición de fuga y posibilidad de utilizar secuencias de prueba.

**Metrel MI 6601 MediTest**  
Analizador de seguridad eléctrica para equipos médicos con funciones de prueba, secuencias automáticas, almacenamiento y comunicación.

### Interpretación del benchmarking

Los tres referentes presentan funciones destinadas a evaluar diferentes aspectos de la seguridad eléctrica de equipos electromédicos. Entre las funciones comunes se encuentran:

- Continuidad de tierra de protección.
- Resistencia de aislamiento.
- Corrientes de fuga.
- Medición de tensión.
- Secuencias de prueba.
- Registro de resultados.
- Comunicación con sistemas externos.

El proyecto de grado toma estas funciones como referencia, pero incorpora un enfoque diferente orientado al **aprendizaje práctico**. Por esta razón, además de las capacidades de medición, se considera importante evaluar la facilidad de comprensión, la interacción con el usuario, la posibilidad de modificar las pruebas y la documentación de la arquitectura.

### Referencias

[1] Fluke Biomedical. *ESA615 Electrical Safety Analyzer*.  
https://www.flukebiomedical.com/products/electrical-safety-analyzers/esa615-electrical-safety-analyzer

[2] Seaward / Rigel Medical. *Rigel 288+ Electrical Safety Analyzer*.  
https://www.seaward.com/us/support/medical/288-plus/

[3] Metrel. *MI 6601 MediTest – Medical Electrical Safety Tester*.  
https://www.metrel.si/en/shop/PAT/medical-testers/mi-6601-meditest.html

[4] International Electrotechnical Commission. *IEC 62353:2014 – Medical electrical equipment – Recurrent test and test after repair of medical electrical equipment*.  
https://webstore.iec.ch/en/publication/6913

[5] International Electrotechnical Commission. *IEC 60601-1 – Medical electrical equipment – Part 1: General requirements for basic safety and essential performance*.  
https://webstore.iec.ch/en/publication/67497
