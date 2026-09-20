# Generación de conceptos
https://lucid.app/lucidchart/cb61810b-8ae5-40ed-985f-0dadce6ae343/edit?viewport_loc=-35590%2C-17243%2C55211%2C28983%2C0_0&invitationId=inv_2041b838-1430-4e6f-a36f-7ccb0cae507e


## A. Sobre la descomposición

La estrategia utilizada para el proyecto fue una **descomposición funcional**. Cada fila de la matriz morfológica representa una función que el analizador de seguridad eléctrica debe cumplir y no necesariamente una actividad que el usuario deba ejecutar de manera estrictamente secuencial.

El sistema recibe un equipo electromédico bajo prueba, sus conexiones, el tipo y los parámetros de la prueba y la interacción del usuario. A partir de estas entradas, el prototipo debe establecer las condiciones necesarias para el ensayo, adquirir las variables eléctricas, procesarlas, evaluarlas y presentar los resultados. Paralelamente, debe permitir registrar la información obtenida durante la práctica.

La descomposición funcional se seleccionó porque el problema de diseño involucra diferentes funciones técnicas que pueden desarrollarse de manera independiente y posteriormente integrarse. Esto resulta especialmente importante debido a que el proyecto propone una **arquitectura abierta**, en la cual los módulos de medición, conexión, adquisición y procesamiento pueden modificarse o ampliarse sin tener que rediseñar completamente el sistema.

Se descartó una descomposición basada únicamente en la secuencia de uso, ya que esta habría organizado el proyecto principalmente alrededor de acciones como encender, conectar, medir y guardar, sin mostrar claramente los subsistemas técnicos que permiten realizar las pruebas. También se descartó una organización únicamente basada en necesidades del usuario, porque habría llevado a describir aspectos como facilidad de uso o aprendizaje sin explicar qué mecanismos electrónicos y de software permiten satisfacerlos.

Por esta razón, la descomposición funcional permite conectar directamente las necesidades identificadas con la ingeniería del producto y con la generación posterior de alternativas de diseño.

Las funciones principales consideradas son:

1. **Medición de seguridad eléctrica**
2. **Conexión del equipo bajo prueba**
3. **Conmutación y establecimiento de condiciones de prueba**
4. **Procesamiento y adquisición de variables**
5. **Interfaz y guía de aprendizaje**
6. **Registro de resultados**

---

## B. Sobre la búsqueda

Durante la generación de medios se analizaron diferentes alternativas para resolver cada una de las funciones del analizador. La búsqueda se orientó principalmente hacia soluciones que pudieran construirse con componentes disponibles comercialmente y que, además, permitieran mantener la arquitectura abierta del prototipo.

Una de las alternativas que inicialmente parecía más compleja fue la implementación de **módulos independientes para cada prueba de seguridad eléctrica**. A primera vista, separar continuidad del conductor de protección, resistencia de aislamiento y corriente de fuga en diferentes módulos podía parecer innecesario frente a un sistema completamente integrado.

Sin embargo, al analizar el objetivo de arquitectura abierta, esta alternativa permitió identificar una ventaja importante: cada módulo puede contener el circuito específico de medición y acondicionamiento necesario para una prueba, mientras que una unidad principal puede encargarse de la alimentación, comunicación, interfaz y procesamiento. De esta manera, una nueva prueba podría incorporarse posteriormente sin modificar completamente el sistema existente.

También se analizaron diferentes alternativas de interacción. Una pantalla integrada permite desarrollar un equipo autónomo, pero aumenta la complejidad del hardware y del software embebido. Por otro lado, utilizar una aplicación en un computador mediante USB permite concentrar la visualización, procesamiento, guía del estudiante y almacenamiento en software, reduciendo la complejidad del prototipo electrónico.

A partir de esta comparación se consideró especialmente viable la combinación entre **módulos de medición independientes, conexiones estandarizadas y una interfaz en PC**, ya que permite demostrar la arquitectura abierta y mantener el alcance del proyecto controlado.

---

## C. Sobre la exploración

Al realizar la matriz de combinación, el espacio de soluciones no se exploró en su totalidad. Se plantearon seis funciones principales y cuatro o cinco medios para cada una, generando un número elevado de combinaciones posibles.

A partir de esta base se generaron y desarrollaron completamente **nueve conceptos integrados**. Estos conceptos representan solamente una parte del espacio total de soluciones, pero permiten comparar diferentes niveles de integración, complejidad, costo y facilidad de implementación.

Además, algunas combinaciones que no resultaban evidentes al analizar cada función de manera individual aparecieron al cruzar las diferentes columnas. Por ejemplo, la combinación de módulos de medición independientes con una interfaz de PC y conectores modulares permite que el sistema pueda crecer posteriormente sin modificar completamente la unidad principal.

La matriz morfológica no solo permitió organizar las ideas disponibles, sino también identificar relaciones entre soluciones que inicialmente podían parecer independientes. Esto es especialmente relevante para este proyecto porque la arquitectura abierta depende de que los diferentes subsistemas puedan comunicarse y reemplazarse sin perder la funcionalidad general del analizador.

Los nueve conceptos se organizaron posteriormente de acuerdo con tres criterios principales:

- **Costo de implementación**
- **Facilidad de implementación**
- **Complejidad técnica**

---

Teniendo en cuenta los **Requerimientos Funcionales y no Funcionales** tomados en cuenta de las necesidades identificadas se realiza la siguiente:

## 1. Matriz Morfológica (Generación de Medios)

Esta tabla descompone el **Nexus 601** en sus subsistemas principales (las Funciones) y propone diferentes formas técnicas de lograrlo (los Medios).

| Función Principal (Subsistema) | Medio 1 (M1) | Medio 2 (M2) | Medio 3 (M3) | Medio 4 (M4) |
|---|---|---|---|---|
| **F1. Visualizar ruta de corriente y Red MD** (Req 1, 11) | Carcasa superior en acrílico transparente + Pistas de LEDs físicos en placa. | Pantalla táctil a color con animación interactiva del flujo. | Panel de aluminio serigrafiado con recortes y retroiluminación. | App móvil/Tablet con Realidad Aumentada escaneando el equipo. |
| **F2. Procesamiento de datos y Gráficas** (Req 4, 8, 12) | Microcontrolador (ESP32/Arduino) + Software en PC externo. | Computadora de placa única (Raspberry Pi) todo integrado. | Envío de datos vía WiFi/Bluetooth a Servidor/Nube (IoT). | Microcontrolador básico + Pantalla inteligente (Nextion). |
| **F3. Interacción y Modo Guiado** (Req 2, 5) | Botones físicos, perilla (encoder rotativo) y display LCD 20x4. | Pantalla táctil capacitiva integrada en el chasis. | Interfaz 100% controlada desde un software de escritorio (USB). | Aplicación en Tablet anclada al equipo. |
| **F4. Inyección de Fallas y Seguridad** (Req 6, 10) | Relés mecánicos visibles + Botón físico de Parada de Emergencia (E-Stop). | Contactores de estado sólido (SSR) + E-Stop digital en pantalla. | Interruptores manuales físicos (switches) + Portafusibles expuestos. | Módulo externo acoplable solo para el profesor (Llave física). |
| **F5. Conexión de Partes Aplicadas** (Req 9) | Bornes tipo banana de 4mm agrupados por colores y símbolos IEC. | Conectores industriales modulares multipin (tipo DB9/VGA). | Placa de conexión con pines magnéticos (tipo Pogo-pin). | Cables fijos retráctiles integrados en la carcasa. |
| **F6. Arquitectura Estructural (Chasis)** (Req 3) | Impresión 3D combinada (Cuerpo en PLA / Bases en TPU antivibración). | Maletín rígido tipo Pelican (Portátil, equipo integrado en la base). | Diseño híbrido (Paneles de MDF cortados a láser + tapa acrílica). | Gabinete estándar metálico comercial modificado. |

---

## 2. Conceptos generados
<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/1149de9b-fc2b-4e3c-b571-9675b81a7fb6" />


## Concepto 1: El "Híbrido de Laboratorio"

**Combinación:**  
`F1-M1 + F2-M1 + F3-M3 + F4-M1 + F5-M1 + F6-M3`

**Descripción:**  
Un equipo de sobremesa con laterales en corte láser y una tapa de acrílico transparente. Se ven los relés y los LEDs iluminarse. Tiene bornes banana estándar. No tiene pantalla propia, se conecta por USB a un PC del laboratorio donde un software guía al estudiante y grafica todo.

---

## Concepto 2: La "Consola Todo-en-Uno" (Stand-alone)

**Combinación:**  
`F1-M2 + F2-M2 + F3-M2 + F4-M1 + F5-M1 + F6-M1`

**Descripción:**  
Un diseño moderno e integrado, impreso totalmente en 3D (PLA). Cuenta con una pantalla táctil grande embebida en ángulo que muestra las animaciones, las gráficas y la separación normativa. No necesita PC externo.

---

## Concepto 3: El "Maletín de Campo"

**Combinación:**  
`F1-M4 + F2-M4 + F3-M1 + F4-M3 + F5-M1 + F6-M2`

**Descripción:**  
Integrado dentro de una maleta rígida tipo Pelican. Es ideal para llevarlo entre salones. El panel es de aluminio negro con los diagramas grabados (serigrafía retroiluminada). Usa interruptores de palanca gruesos ("switches" físicos) para que el profesor induzca las fallas manualmente.

---

## Concepto 4: El "Minimalista IoT"

**Combinación:**  
`F1-M1 + F2-M3 + F3-M4 + F4-M2 + F5-M3 + F6-M1`

**Descripción:**  
Una caja transparente impresa en resina o ensamblada en acrílico, extremadamente limpia. Funciona como un módulo de adquisición "tonto" basado en ESP32 que envía todo de forma inalámbrica a una Tablet. Las partes aplicadas se conectan magnéticamente.

---

## Concepto 5: La "Estación Modular Encastrable"

**Combinación:**  
`F1-M3 + F2-M1 + F3-M3 + F4-M4 + F5-M2 + F6-M1`

**Descripción:**  
Una base principal a la que se le pueden apilar módulos (como bloques) dependiendo de si se va a medir partes aplicadas tipo B, BF o CF, o si se añade el módulo de fallas del profesor.

---
