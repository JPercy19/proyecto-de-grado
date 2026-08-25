# Arbol de objetivos

## Proposito

El arbol de objetivos transforma el problema preliminar en una situacion deseada. No representa resultados ya obtenidos: las relaciones entre medios, objetivo central y fines se deben validar mediante la indagacion social, el inventario del laboratorio y la revision con docentes.

## Objetivo central

Fortalecer el aprendizaje practico, seguro y comprensible de pruebas seleccionadas de seguridad electrica en equipos electromedicos mediante una plataforma didactica de arquitectura abierta.

## Medios, objetivo y fines

```mermaid
flowchart TB
    M1[Ampliar el acceso a escenarios de practica seguros y supervisados] --> O[Fortalecer el aprendizaje practico de pruebas de seguridad electrica]
    M2[Hacer visible la relacion entre conexion, medicion y resultado] --> O
    M3[Integrar guias de practica con retroalimentacion y registro] --> O
    M4[Documentar una arquitectura abierta de baja energia y sus limites] --> O

    O --> F1[Mejorar la capacidad para configurar e interpretar escenarios de prueba]
    O --> F2[Reducir errores de conexion durante actividades academicas]
    O --> F3[Favorecer la preparacion para mantenimiento y gestion de tecnologia biomedica]
    O --> F4[Promover el uso responsable de normas, procedimientos y resultados de medicion]
```

## Relacion con las necesidades

| Medio | Necesidad asociada | Evidencia por obtener | Resultado de diseno esperado |
|---|---|---|---|
| Escenarios seguros y supervisados | N-01: practicar sin exposicion a energia peligrosa. | Riesgos identificados por docentes, personal tecnico e inventario. | Simuladores o cargas protegidas, controles y protocolo de uso. |
| Relacion visible entre conexion y resultado | N-02: comprender secuencia y fundamento. | Dificultades conceptuales y operativas de estudiantes. | Interfaz que muestre escenario, conexion, pasos y explicacion. |
| Guias, retroalimentacion y registro | N-03 y N-05: identificar errores y registrar practicas. | Errores frecuentes y criterios de evaluacion docente. | Lista de verificacion, retroalimentacion y reporte de practica. |
| Arquitectura abierta segura | N-04 y N-08: inspeccionar modulos y comprender limites. | Nivel de conocimientos, documentacion requerida y controles necesarios. | Esquematicos de baja tension, BOM, firmware y advertencias de alcance. |

## Indicadores de logro de la fase de diseno

El arbol se considerara util cuando cada medio se traduzca en uno o mas atributos verificables y cada fin pueda evaluarse sin atribuirle al prototipo una certificacion clinica. Los indicadores preliminares incluyen desempeno en la secuencia de practica, identificacion de configuraciones inseguras, explicacion del resultado, tiempo de preparacion y completitud del registro.
