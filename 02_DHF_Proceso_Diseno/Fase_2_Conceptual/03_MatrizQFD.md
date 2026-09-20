# MATRIZ QFD
<img width="7528" height="7640" alt="03_MATRIZ_QFD" src="https://github.com/user-attachments/assets/11ce29ad-4d85-4585-9760-8f35cc8d9bc6" />

## Análisis de la Matriz QFD

La matriz QFD permite establecer la relación entre las **necesidades del usuario** y las **características técnicas** requeridas para el desarrollo del prototipo de analizador de seguridad eléctrica. Además, incorpora los valores objetivo, la dificultad técnica y una evaluación competitiva frente a equipos de referencia.

## 1. Priorización de las características técnicas

De acuerdo con la fila de **Importancia Relativa (%)**, las características técnicas con mayor peso dentro del diseño son:

| Característica técnica | Importancia relativa |
|---|---:|
| Guía e indicación del procedimiento | **14,4 %** |
| Detección e indicación de condiciones anormales | **10,7 %** |
| Secuencias de prueba automáticas/configurables | **9,8 %** |
| Variables y resultados visibles durante la prueba | **9,5 %** |
| Registro de resultados de las prácticas | **7,2 %** |
| Métodos de corriente de fuga IEC 62353 | **7,0 %** |
| Implementación de pruebas de continuidad de PE | **6,3 %** |
| Medición de resistencia de aislamiento | **6,2 %** |
| Conexiones configurables para partes aplicadas | **6,1 %** |
| Corriente de prueba de continuidad PE | **5,9 %** |
| Tensiones de prueba de aislamiento | **5,2 %** |
| Resolución de medición de corriente de fuga | **5,0 %** |
| Tiempo de recuperación de registros | **4,3 %** |
| Documentación de arquitectura abierta | **2,5 %** |

Estos resultados muestran que las necesidades del proyecto no se concentran únicamente en la capacidad de realizar mediciones eléctricas. Las características relacionadas con la **orientación del usuario, la seguridad durante el procedimiento, la visualización de información y la automatización de las pruebas** presentan una importancia elevada.

---

## 2. Interpretación de las características prioritarias

### 2.1. Guía e indicación del procedimiento — 14,4 %

La característica con mayor importancia relativa corresponde a la **guía e indicación del procedimiento**.

Esto indica que el prototipo debe permitir al usuario comprender qué debe hacer durante cada etapa de la práctica. La guía debe estar relacionada con:

- Selección del tipo de prueba.
- Configuración de parámetros.
- Conexión del equipo bajo prueba.
- Verificación de las condiciones de prueba.
- Ejecución de la medición.
- Interpretación del resultado.
- Orientación ante errores o condiciones anormales.

Por lo tanto, esta característica debe reflejarse posteriormente en el diseño de la interfaz y en la secuencia de funcionamiento del prototipo.

---

### 2.2. Detección e indicación de condiciones anormales — 10,7 %

La segunda característica con mayor importancia corresponde a la **detección e indicación de condiciones anormales**.

El sistema debe contemplar mecanismos que permitan identificar situaciones que puedan afectar el procedimiento de prueba. Esto puede relacionarse con:

- Conexiones incorrectas.
- Parámetros de prueba inadecuados.
- Valores fuera de los límites establecidos.
- Condiciones anormales durante la medición.
- Situaciones que requieran detener o modificar el procedimiento.

La detección de estas condiciones debe estar relacionada con la presentación de alertas y mensajes de orientación para el usuario.

---

### 2.3. Secuencias de prueba automáticas/configurables — 9,8 %

Las **secuencias de prueba automáticas o configurables** presentan una importancia relativa elevada.

Esta característica permite estructurar el procedimiento de manera ordenada, por ejemplo:

```text
Seleccionar prueba
        ↓
Configurar parámetros
        ↓
Verificar conexiones
        ↓
Establecer condiciones de prueba
        ↓
Realizar medición
        ↓
Procesar y evaluar
        ↓
Mostrar resultado
        ↓
Registrar resultado
```
## 2.4. Variables y resultados visibles durante la prueba — 9,5 %

La visualización de las variables y resultados durante la práctica también presenta una importancia elevada.

Dependiendo del tipo de prueba, el sistema debe permitir visualizar información relacionada con:

- Tensión.
- Corriente.
- Resistencia.
- Corriente de fuga.
- Parámetros configurados.
- Estado de la prueba.
- Resultado de la evaluación.
- Alertas.

Esta característica es especialmente relevante para el carácter educativo del prototipo, debido a que permite que el estudiante observe el comportamiento del sistema durante la ejecución de la práctica.

---

## 3. Características relacionadas con las mediciones eléctricas

Las características directamente relacionadas con la medición también presentan una importancia significativa dentro del QFD.

| Característica | Importancia relativa |
|---|---:|
| Implementación de pruebas de continuidad de PE | 6,3 % |
| Medición de resistencia de aislamiento | 6,2 % |
| Métodos de corriente de fuga IEC 62353 | 7,0 % |
| Corriente de prueba de continuidad PE | 5,9 % |
| Tensiones de prueba de aislamiento | 5,2 % |
| Resolución de medición de corriente de fuga | 5,0 % |

Estos resultados muestran que las funciones de medición constituyen una parte fundamental del sistema. Sin embargo, el resultado global de la matriz indica que estas funciones deben complementarse con mecanismos de orientación, evaluación y seguridad.

Por lo tanto, el prototipo debe buscar un equilibrio entre:

> **Medición eléctrica + seguridad + orientación + evaluación + registro.**

---

## 4. Registro de resultados

El **registro de resultados de las prácticas** presenta una importancia relativa de **7,2 %**, mientras que el **tiempo de recuperación de registros** presenta un valor de **4,3 %**.

Esto respalda la incorporación de una función que permita almacenar información relacionada con cada práctica, incluyendo:

- Equipo bajo prueba.
- Tipo de prueba.
- Parámetros utilizados.
- Resultados obtenidos.
- Fecha y hora.
- Información necesaria para su posterior consulta o exportación.

El registro permite que los resultados obtenidos durante las prácticas puedan ser revisados posteriormente.

---

## 5. Arquitectura abierta

La **documentación de arquitectura abierta** presenta una importancia relativa de **2,5 %**, siendo la característica con menor peso dentro de la matriz.

Este resultado no significa que la arquitectura abierta deba eliminarse del proyecto. Su importancia dentro del QFD está relacionada principalmente con las necesidades directas del usuario, mientras que la arquitectura abierta corresponde también a una característica estructural del proyecto.

La arquitectura abierta permite plantear un sistema en el que puedan documentarse y estudiarse:

- Hardware.
- Circuitos de medición.
- Módulos de control.
- Firmware.
- Software.
- Conexiones.
- Módulos intercambiables.

Por lo tanto, puede mantenerse como una característica de diseño aunque tenga una menor importancia relativa en la matriz.

---

## 6. Dificultad técnica

La matriz también incorpora una valoración de **Dificultad Técnica**, con valores entre 3 y 5.

Las características relacionadas directamente con las mediciones de seguridad eléctrica presentan niveles de dificultad técnica elevados. Entre ellas se encuentran:

- Implementación de pruebas de continuidad de PE.
- Medición de resistencia de aislamiento.
- Métodos de corriente de fuga.
- Tensiones de prueba de aislamiento.

Esto indica que la selección del concepto no debe realizarse únicamente considerando la interfaz o la apariencia física del prototipo.

El concepto seleccionado debe proporcionar una arquitectura que permita integrar los circuitos de medición y protección necesarios sin aumentar innecesariamente la complejidad del sistema.

---

## 7. Evaluación competitiva

La matriz incorpora una comparación con tres equipos de referencia:

- **Fluke ESA615**
- **Rigel 288+**
- **Metrel MI 6601**

El benchmarking permite comparar el prototipo propuesto frente a equipos existentes en diferentes características técnicas.

La comparación muestra que los equipos de referencia cuentan con capacidades consolidadas relacionadas con las pruebas de seguridad eléctrica. Por esta razón, el prototipo no debe plantearse únicamente como una reproducción de un analizador comercial.

La matriz orienta el desarrollo hacia la integración de:

- Medición de seguridad eléctrica.
- Guía del procedimiento.
- Detección de condiciones anormales.
- Visualización de variables.
- Evaluación de resultados.
- Registro de prácticas.
- Arquitectura abierta.

---

## 8. Relación entre las características técnicas

El techo de la matriz QFD permite identificar relaciones entre las diferentes características técnicas.

Estas relaciones muestran que las características no deben analizarse de manera independiente, debido a que una decisión de diseño puede afectar simultáneamente diferentes aspectos del sistema.

Por ejemplo:

```text
Mayor automatización
        ↓
Mayor necesidad de control
        ↓
Mayor complejidad del sistema
```
Por esta razón, la selección de alternativas debe considerar el conjunto de características técnicas y no solamente una característica individual.

## 9. Implicaciones para la selección del concepto

Los resultados obtenidos mediante el QFD permiten establecer criterios para la siguiente etapa de diseño conceptual.

El concepto seleccionado debe favorecer principalmente:

Guía paso a paso del procedimiento.
Detección e indicación de condiciones anormales.
Secuencias de prueba automáticas o configurables.
Visualización de variables y resultados.
Registro de las prácticas realizadas.
Implementación de las pruebas eléctricas definidas en el alcance.
Arquitectura modular y documentada.

Estos criterios pueden utilizarse posteriormente para comparar los diferentes conceptos generados mediante la matriz morfológica.

## 10. Conclusión del análisis QFD

La matriz QFD permitió establecer la relación entre las necesidades identificadas del usuario y las características técnicas necesarias para el desarrollo del prototipo de analizador de seguridad eléctrica.

Los resultados muestran que las características con mayor importancia relativa son la guía e indicación del procedimiento (14,4 %), la detección e indicación de condiciones anormales (10,7 %), las secuencias de prueba automáticas o configurables (9,8 %) y la visualización de variables y resultados durante la prueba (9,5 %).

Esto evidencia que el proyecto requiere no solamente capacidades de medición eléctrica, sino también mecanismos que permitan orientar al usuario, controlar el procedimiento y facilitar la interpretación de los resultados.

Las características relacionadas directamente con las mediciones, como la continuidad del conductor de protección, la resistencia de aislamiento y los métodos de corriente de fuga, también presentan una importancia significativa y constituyen la base funcional del analizador.

Por otra parte, el registro de resultados (7,2 %) respalda la incorporación de mecanismos para almacenar y consultar la información obtenida durante las prácticas. La documentación de arquitectura abierta (2,5 %) presenta una importancia relativa menor dentro del QFD, pero permanece como una característica estratégica debido al carácter educativo y modular del proyecto.

Finalmente, el benchmarking permite establecer que el prototipo no debe plantearse únicamente como una réplica de un analizador comercial. Los resultados del QFD orientan el diseño hacia una solución que integre:

Medición de seguridad eléctrica + orientación del procedimiento + detección de condiciones anormales + visualización + evaluación + registro + arquitectura abierta.

Estos resultados servirán como base para la selección y evaluación de los conceptos generados mediante la matriz morfológica.
