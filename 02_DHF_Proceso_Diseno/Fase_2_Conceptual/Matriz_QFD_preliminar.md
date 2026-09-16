# Casa de la Calidad (QFD) preliminar

## Propósito y alcance

Esta matriz traduce las necesidades documentadas para el prototipo didáctico de
analizador de seguridad eléctrica en características técnicas de diseño. El
prototipo es una plataforma de aprendizaje de arquitectura abierta; no es un
analizador certificado, no se conecta a pacientes y no se usa para liberar,
diagnosticar ni declarar la conformidad de equipos clínicos.

El archivo [`matriz_qfd_preliminar.json`](matriz_qfd_preliminar.json) se puede
cargar directamente en la aplicación [Matriz QFD](https://oscampo.github.io/Matriz-QFD/):
**Archivo > Importar JSON**. Después se puede exportar como imagen o SVG para
el informe.

## Estado de la priorización

La evidencia de campo todavía está pendiente: el repositorio no contiene
resultados de encuesta, entrevistas ni inventario del laboratorio. Por tanto,
los valores de importancia son una propuesta inicial de diseño, no resultados
atribuidos a usuarios. N-01 y N-08 se mantienen con importancia 5 por ser
restricciones de seguridad y de uso previsto; no pueden compensarse con costo
o conveniencia. Las demás prioridades y todos los objetivos cuantitativos
deben actualizarse tras triangular la evidencia indicada en los instrumentos
de indagación.

Las relaciones emplean la escala de la aplicación: **9** fuerte, **3** media y
**1** débil. El techo utiliza relaciones positivas y negativas entre
características técnicas.

## Requerimientos de usuario (QUÉ)

| Código | Requerimiento | Importancia inicial |
|---|---|---:|
| N-01 | Practicar sin exposición a energía peligrosa. | 5 |
| N-02 | Comprender la secuencia y el fundamento de cada prueba. | 5 |
| N-03 | Identificar configuraciones incorrectas antes de ejecutar una práctica. | 4 |
| N-04 | Observar una arquitectura documentada y modificable de forma segura. | 4 |
| N-05 | Registrar el escenario, procedimiento y resultado de una práctica. | 4 |
| N-06 | Preparar, supervisar y evaluar la práctica en el tiempo disponible. | 4 |
| N-07 | Contar con una solución mantenible, reparable y compatible con los recursos del laboratorio. | 3 |
| N-08 | Distinguir el alcance educativo de una evaluación profesional. | 5 |

## Características técnicas (CÓMO)

| Código | Característica técnica | Unidad | Objetivo |
|---|---|---|---|
| C-01 | Cobertura de controles para escenarios de baja energía. | % de escenarios | Por definir con análisis de riesgo. |
| C-02 | Cobertura de detección o confirmación de configuraciones incorrectas. | % de errores definidos | Por definir con pruebas de tareas. |
| C-03 | Cobertura de pasos guiados por escenario. | % de pasos | Por definir con revisión docente. |
| C-04 | Cobertura de explicaciones de principio, resultado y límite. | % de elementos didácticos | Por definir con rúbrica conceptual. |
| C-05 | Completitud y versionado de la documentación de módulos permitidos. | % de documentos requeridos | Por definir con lista documental. |
| C-06 | Completitud del registro exportable por práctica. | Campos obligatorios | Por definir con docentes. |
| C-07 | Tiempo de preparación, cierre y evaluación de la práctica. | Minutos | Por definir con inventario y cronometraje. |
| C-08 | Modularidad y reemplazabilidad de componentes de baja energía. | Módulos reemplazables | Por definir con BOM y presupuesto. |
| C-09 | Cobertura de advertencias sobre el alcance educativo. | Puntos de contacto | Carcasa, interfaz y reporte. |

## Prioridad técnica calculada

La herramienta calcula la importancia absoluta como la suma de
`importancia del QUÉ × relación`. Con los datos preliminares, el orden de
atención es:

| Orden | Característica | Importancia absoluta | Importancia relativa |
|---:|---|---:|---:|
| 1 | C-03: Pasos guiados por escenario | 101 | 15.0% |
| 2 | C-01: Controles para escenarios de baja energía | 90 | 13.4% |
| 3 | C-04: Explicaciones de principio, resultado y límite | 84 | 12.5% |
| 4 | C-09: Advertencias sobre alcance educativo | 84 | 12.5% |
| 5 | C-06: Registro exportable por práctica | 78 | 11.6% |
| 6 | C-05: Documentación de módulos permitidos | 75 | 11.1% |
| 7 | C-02: Detección o confirmación de configuraciones incorrectas | 63 | 9.3% |
| 8 | C-08: Modularidad y reemplazabilidad | 54 | 8.0% |
| 9 | C-07: Tiempo de preparación, cierre y evaluación | 45 | 6.7% |

## Correlaciones relevantes del techo

| Relación | Tipo | Implicación de diseño |
|---|---|---|
| C-03 y C-04 | Positiva fuerte | La guía paso a paso debe incluir la explicación conceptual del paso y del resultado. |
| C-05 y C-08 | Positiva fuerte | La modularidad necesita documentación y BOM versionados para permitir una reparación segura. |
| C-01 y C-07 | Negativa media | Los controles de seguridad pueden aumentar el tiempo de preparación; se debe simplificar el protocolo sin reducir barreras. |
| C-01 y C-08 | Negativa media | Barreras y acceso restringido pueden dificultar la sustitución de módulos; separar los módulos de baja energía. |
| C-06 y C-07 | Negativa media | Un registro más completo puede aumentar el tiempo de práctica; definir solo los campos necesarios para reconstruirla. |
| C-07 y C-08 | Negativa media | La facilidad de reemplazo puede exigir tiempo adicional de acceso o verificación; diseñar conectores y procedimientos claros. |

## Fuentes del repositorio

- `Fase_1_Investigacion/NECESIDADES DEL OBJETIVO/necesidades identificadas.md`
- `Fase_1_Investigacion/NECESIDADES DEL OBJETIVO/Arbol de objetivos.md`
- `Fase_1_Investigacion/INDAGACION SOCIAL/indagacion social.md`
- `Fase_1_Investigacion/INDAGACION SOCIAL/Instrumentos de indagacion.md`
- `Fase_1_Investigacion/Base_investigacion_y_proceso_diseno.md`
