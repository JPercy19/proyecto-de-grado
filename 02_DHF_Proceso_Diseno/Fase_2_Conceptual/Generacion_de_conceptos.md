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

# Matriz morfológica — Generación de medios

| Función principal (subsistema) | Medio 1 (M1) | Medio 2 (M2) | Medio 3 (M3) | Medio 4 (M4) |
|---|---|---|---|---|
| **F1. Medición de seguridad eléctrica** | Módulos de medición independientes | Circuitos de medición integrados en una placa | Módulos intercambiables según la prueba | Módulos con acondicionamiento y protección de señales |
| **F2. Conexión del equipo bajo prueba** | Bornes banana de 4 mm identificados | Panel de conectores modulares | Borneras de conexión independientes | Cables con conectores específicos para cada prueba |
| **F3. Conmutación y condiciones de prueba** | Relés electromecánicos | Relés + circuitos de protección | Módulos de conmutación independientes | Conmutación controlada por microcontrolador |
| **F4. Procesamiento y adquisición** | Microcontrolador + ADC externo | Módulos de adquisición independientes | Microcontrolador + aplicación en PC mediante USB | Sistema de adquisición dedicado por prueba |
| **F5. Interfaz y guía de aprendizaje** | Pantalla TFT/LCD integrada | Pantalla LCD + botones físicos | Aplicación de escritorio mediante USB | Interfaz gráfica en PC con guía paso a paso |
| **F6. Registro de resultados** | Tarjeta microSD | Memoria interna | Almacenamiento en PC mediante USB | Archivo CSV generado por el software |

---

# Conceptos integrados

A partir de la tabla de combinación de conceptos se generaron nueve alternativas. Cada una combina una alternativa de las seis funciones principales.

---

## 1. Conceptos de mínimo costo

### Concepto 2 — "Analizador de laboratorio básico"

**Combinación:** F1-M2 + F2-M1 + F3-M1 + F4-M1 + F5-M3 + F6-M3

- **Medición de seguridad eléctrica:**  
  Circuitos de medición integrados en una sola placa.

- **Conexión del equipo bajo prueba:**  
  Bornes tipo banana de 4 mm identificados.

- **Conmutación y condiciones de prueba:**  
  Relés electromecánicos.

- **Procesamiento y adquisición:**  
  Microcontrolador + ADC externo.

- **Interfaz y guía de aprendizaje:**  
  Aplicación de escritorio mediante USB.

- **Registro de resultados:**  
  Almacenamiento en PC mediante USB.

### Concepto 5 — "Analizador de sobremesa modular"

**Combinación:** F1-M2 + F2-M3 + F3-M1 + F4-M1 + F5-M3 + F6-M3

- **Medición de seguridad eléctrica:**  
  Circuitos de medición integrados en una sola placa.

- **Conexión del equipo bajo prueba:**  
  Borneras de conexión independientes.

- **Conmutación y condiciones de prueba:**  
  Relés electromecánicos.

- **Procesamiento y adquisición:**  
  Microcontrolador + ADC externo.

- **Interfaz y guía de aprendizaje:**  
  Aplicación de escritorio mediante USB.

- **Registro de resultados:**  
  Almacenamiento en PC mediante USB.

### Concepto 6 — "Analizador básico con control físico"

**Combinación:** F1-M1 + F2-M1 + F3-M2 + F4-M1 + F5-M2 + F6-M1

- **Medición de seguridad eléctrica:**  
  Módulos de medición independientes.

- **Conexión del equipo bajo prueba:**  
  Bornes tipo banana de 4 mm identificados.

- **Conmutación y condiciones de prueba:**  
  Relés con circuitos de protección.

- **Procesamiento y adquisición:**  
  Microcontrolador + ADC externo.

- **Interfaz y guía de aprendizaje:**  
  Pantalla LCD + botones físicos.

- **Registro de resultados:**  
  Tarjeta microSD.

### Justificación del criterio

Los conceptos 2, 5 y 6 se agrupan en **mínimo costo** porque utilizan principalmente componentes electrónicos comerciales y una arquitectura relativamente sencilla. Los conceptos 2 y 5 aprovechan un computador externo para realizar la visualización y el almacenamiento, reduciendo la cantidad de hardware que debe integrarse en el prototipo. El concepto 6 incorpora una interfaz y almacenamiento locales, pero mantiene componentes convencionales como relés, microcontrolador, ADC y tarjeta microSD.

---

## 2. Conceptos más fáciles de implementar

### Concepto 1 — "Analizador de laboratorio"

**Combinación:** F1-M1 + F2-M1 + F3-M1 + F4-M1 + F5-M2 + F6-M1

- **Medición de seguridad eléctrica:**  
  Módulos de medición independientes.

- **Conexión del equipo bajo prueba:**  
  Bornes tipo banana de 4 mm identificados.

- **Conmutación y condiciones de prueba:**  
  Relés electromecánicos.

- **Procesamiento y adquisición:**  
  Microcontrolador + ADC externo.

- **Interfaz y guía de aprendizaje:**  
  Pantalla LCD + botones físicos.

- **Registro de resultados:**  
  Tarjeta microSD.

### Concepto 9 — "Analizador modular conectado a PC"

**Combinación:** F1-M3 + F2-M2 + F3-M3 + F4-M3 + F5-M3 + F6-M3

- **Medición de seguridad eléctrica:**  
  Módulos intercambiables según la prueba.

- **Conexión del equipo bajo prueba:**  
  Panel de conectores modulares.

- **Conmutación y condiciones de prueba:**  
  Módulos de conmutación independientes.

- **Procesamiento y adquisición:**  
  Microcontrolador + aplicación en PC mediante USB.

- **Interfaz y guía de aprendizaje:**  
  Aplicación de escritorio mediante USB.

- **Registro de resultados:**  
  Almacenamiento en PC mediante USB.

### Justificación del criterio

Los conceptos 1 y 9 se consideran **más fáciles de implementar** porque pueden construirse a partir de módulos electrónicos y componentes comerciales disponibles. Además, permiten separar las funciones de medición y procesamiento sin requerir un sistema embebido excesivamente complejo.

El concepto 9 resulta particularmente favorable para el desarrollo de arquitectura abierta, ya que los módulos de medición pueden probarse individualmente y posteriormente integrarse a una unidad principal.

---

## 3. Conceptos complejos

### Concepto 7 — "Estación modular autónoma"

**Combinación:** F1-M3 + F2-M2 + F3-M4 + F4-M2 + F5-M1 + F6-M1

- **Medición de seguridad eléctrica:**  
  Módulos intercambiables según la prueba.

- **Conexión del equipo bajo prueba:**  
  Panel de conectores modulares.

- **Conmutación y condiciones de prueba:**  
  Conmutación controlada por microcontrolador.

- **Procesamiento y adquisición:**  
  Módulos de adquisición independientes.

- **Interfaz y guía de aprendizaje:**  
  Pantalla TFT/LCD integrada.

- **Registro de resultados:**  
  Tarjeta microSD.

### Concepto 8 — "Analizador didáctico integrado"

**Combinación:** F1-M4 + F2-M4 + F3-M4 + F4-M4 + F5-M4 + F6-M3

- **Medición de seguridad eléctrica:**  
  Módulos con acondicionamiento y protección de señales.

- **Conexión del equipo bajo prueba:**  
  Cables con conectores específicos para cada prueba.

- **Conmutación y condiciones de prueba:**  
  Conmutación controlada por microcontrolador.

- **Procesamiento y adquisición:**  
  Sistema de adquisición dedicado por prueba.

- **Interfaz y guía de aprendizaje:**  
  Interfaz gráfica en PC con guía paso a paso.

- **Registro de resultados:**  
  Almacenamiento en PC mediante USB.

### Justificación del criterio

Los conceptos 7 y 8 se clasifican como **complejos** debido a la integración de diferentes subsistemas y al nivel de control requerido. El concepto 7 requiere módulos intercambiables, adquisición independiente, conmutación controlada y una interfaz integrada. El concepto 8 incorpora además circuitos de acondicionamiento y protección específicos, conectores particulares para cada prueba y sistemas de adquisición dedicados.

Estos elementos aumentan la cantidad de hardware que debe diseñarse, integrarse y validarse, así como la complejidad del firmware y del software de control.

---

## 4. Conceptos de mayor costo

### Concepto 3 — "Estación modular autónoma avanzada"

**Combinación:** F1-M3 + F2-M2 + F3-M3 + F4-M2 + F5-M1 + F6-M1

- **Medición de seguridad eléctrica:**  
  Módulos intercambiables según la prueba.

- **Conexión del equipo bajo prueba:**  
  Panel de conectores modulares.

- **Conmutación y condiciones de prueba:**  
  Módulos de conmutación independientes.

- **Procesamiento y adquisición:**  
  Módulos de adquisición independientes.

- **Interfaz y guía de aprendizaje:**  
  Pantalla TFT/LCD integrada.

- **Registro de resultados:**  
  Tarjeta microSD.

### Concepto 4 — "Plataforma didáctica completa"

**Combinación:** F1-M4 + F2-M4 + F3-M4 + F4-M4 + F5-M4 + F6-M3

- **Medición de seguridad eléctrica:**  
  Módulos con acondicionamiento y protección de señales.

- **Conexión del equipo bajo prueba:**  
  Cables con conectores específicos para cada prueba.

- **Conmutación y condiciones de prueba:**  
  Conmutación controlada por microcontrolador.

- **Procesamiento y adquisición:**  
  Sistema de adquisición dedicado por prueba.

- **Interfaz y guía de aprendizaje:**  
  Interfaz gráfica en PC con guía paso a paso.

- **Registro de resultados:**  
  Almacenamiento en PC mediante USB.

### Justificación del criterio

Los conceptos 3 y 4 se clasifican como de **mayor costo** debido a que requieren un mayor número de módulos, circuitos de adquisición y elementos de conexión especializados. El concepto 3 incorpora módulos independientes de medición y adquisición junto con una interfaz integrada. El concepto 4 requiere sistemas de acondicionamiento y protección específicos, adquisición dedicada y conectores particulares para cada prueba.

Estos elementos pueden incrementar tanto el costo de los componentes como el tiempo requerido para fabricación, integración y validación.

---

# 5. Concepto seleccionado para desarrollo posterior

A partir de la comparación entre costo, facilidad de implementación, complejidad y coherencia con el objetivo de arquitectura abierta, se propone continuar el desarrollo conceptual tomando como base el:

## "Analizador modular conectado a PC"

Este concepto combina:

- Módulos de medición intercambiables.
- Conectores modulares y claramente identificados.
- Módulos de conmutación independientes.
- Microcontrolador para adquisición y control.
- Comunicación USB con un computador.
- Interfaz gráfica orientada al aprendizaje.
- Registro de resultados en formato abierto.

La selección no implica que las demás alternativas sean descartadas desde el punto de vista técnico. Los demás conceptos sirven como alternativas de diseño y permiten identificar diferentes maneras de resolver las funciones del producto.

La arquitectura seleccionada permite además mantener una separación clara entre **hardware de medición, control, software e interfaz**, facilitando futuras modificaciones y la incorporación de nuevas pruebas de seguridad eléctrica.

---

# Relación con el objetivo del proyecto

El concepto generado busca responder al objetivo general de diseñar un **prototipo de analizador de seguridad eléctrica de arquitectura abierta para el aprendizaje práctico de pruebas de seguridad eléctrica en equipos electromédicos**, tomando como referencia los procedimientos y criterios aplicables de **IEC 60601-1 e IEC 62353**.

La generación de conceptos permite pasar de las necesidades identificadas y las funciones del sistema a una configuración física y funcional que posteriormente puede ser evaluada mediante los criterios de selección de conceptos, la matriz QFD y las especificaciones objetivo del producto.
