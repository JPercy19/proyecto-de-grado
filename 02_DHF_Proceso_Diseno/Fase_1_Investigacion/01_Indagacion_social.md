# Indagacion social

## Contexto social y educativo

La seguridad electrica de los equipos electromedicos es un campo donde el conocimiento tecnico tiene una relacion directa con el bienestar de pacientes, operadores y personal de mantenimiento. Sin embargo, aprender los procedimientos de verificacion unicamente desde diapositivas, manuales o la interfaz cerrada de un analizador comercial dificulta relacionar el riesgo electrico con la configuracion de la prueba y la lectura obtenida. El problema no es la ausencia de equipos profesionales, sino que estos han sido desarrollados para ejecutar pruebas confiables en servicio y no necesariamente para explicar sus bloques internos a un estudiante.

En el contexto de formacion de ingenieria biomedica, los estudiantes requieren experiencias que integren fundamentos de electricidad, instrumentacion, gestion del riesgo, mantenimiento y normativa. La literatura sobre aprendizaje activo indica que la participacion práctica debe complementarse con prediccion, retroalimentacion y explicacion; de lo contrario, una actividad puede sentirse activa sin producir una comprension proporcional (Deslauriers et al., 2019). El aprendizaje basado en retos y proyectos permite que el estudiante enfrente una situacion realista, proponga una configuracion, pruebe de forma segura y argumente el resultado (Lavado-Anguera et al., 2024; Santos-Diaz et al., 2024).

El proyecto se dirige inicialmente a estudiantes de ingenieria biomedica que cursen asignaturas de bioinstrumentacion, mantenimiento, gestion de tecnologia hospitalaria o seguridad electrica; docentes responsables de dichas asignaturas; y personal tecnico con experiencia en el entorno de practica. Estos grupos no tienen la misma necesidad: el estudiante requiere comprension y retroalimentacion; el docente requiere una practica segura, repetible y evaluable; el personal tecnico requiere que se comunique con claridad que el prototipo no sustituye un analizador profesional ni autoriza decisiones sobre equipos clinicos.

## Problema social identificado

La necesidad social preliminar es ampliar el acceso a una práctica de seguridad electrica que sea segura, explicable y reproducible. El acceso no se refiere solamente a comprar un instrumento: comprende el número de estudiantes por práctica, el tiempo de uso, la disponibilidad de simuladores, el acompañamiento docente, la posibilidad de observar la arquitectura y la existencia de guias que conecten una acción con el fenómeno electrico que representa.

La falta de esta experiencia puede favorecer aprendizajes procedimentales: el estudiante sigue una secuencia de botones sin reconocer por qué se verifica una ruta de tierra, cómo cambia una lectura al modificar una condición de ensayo o por qué una lectura educativa no basta para declarar conformidad. Esta afirmacion es una hipótesis de diseño y debe contrastarse con evidencia local; no se deben atribuir porcentajes, incidentes ni dificultades a la población objetivo hasta aplicar los instrumentos definidos en este documento.

## Poblacion, actores y relacion con el proyecto

| Actor | Interes o necesidad | Riesgo si no se considera | Participacion en el diseño |
|---|---|---|---|
| Estudiantes | Practicar, comprender y recibir retroalimentacion. | Aprendizaje memoristico o conexiones inseguras. | Encuesta, prueba de tareas y evaluación de usabilidad. |
| Docentes | Guiar y evaluar una practica segura en tiempo limitado. | Actividad dificil de supervisar o evaluar. | Entrevista, validacion de guia y definición de resultados de aprendizaje. |
| Personal tecnico | Reconocer procedimientos y limites de uso. | Confusión entre plataforma didactica e instrumento de servicio. | Entrevista y revisión de escenarios de práctica. |
| Institucion/laboratorio | Uso seguro y sostenible de recursos. | Daño de equipos, prácticas no autorizadas o baja disponibilidad. | Inventario, reglamento y aprobación del protocolo. |

## Dimensiones que orientan la indagacion

**Social.** Se debe conocer el nivel de experiencia previa, la confianza para realizar conexiones, las barreras de acceso a prácticas y las expectativas sobre una herramienta abierta. La plataforma no debe exigir conocimientos que la población no ha adquirido ni excluir a quienes tengan menor experiencia instrumental.

**Tecnologica.** Se debe documentar qué analizadores, simuladores, equipos no clínicos, computadores, conectividad, mesas y elementos de protección están disponibles. También se debe registrar si el laboratorio permite prácticas con red eléctrica o si la primera versión debe limitarse a señales y simulaciones de baja energía.

**Economica.** El presupuesto no se asumirá. Se recolectarán cotizaciones de componentes, manufactura, mantenimiento y repuestos, además del costo de oportunidad de las horas de laboratorio. La apertura documental puede facilitar mantenimiento y réplica, pero esta ventaja deberá demostrarse con el presupuesto, no declararse como un hecho.

**Ambiental.** El diseño deberá considerar consumo en espera, reparabilidad, modularidad, selección de materiales y manejo de residuos electrónicos. El prototipo debe permitir reemplazar módulos de bajo voltaje sin desechar el conjunto completo.

**Seguridad y bienestar.** Los escenarios educativos se diseñarán para evitar contacto con partes energizadas, energía residual, configuraciones ambiguas y uso clínico indebido. ISO 14971 orientará el análisis de peligros y sus controles; IEC 60601-1, IEC 62353 e IEC 60990 serán marcos de referencia, sin convertir el prototipo en un equipo certificado.

## Metodo de indagacion

Se utilizará un enfoque mixto y secuencial. La revisión documental permite construir conceptos y preguntas; las entrevistas profundizan en tareas y restricciones; la encuesta permite estimar tendencias de la cohorte; el inventario muestra las condiciones físicas; y la triangulación convierte resultados en requisitos.

1. Revisar normas, literatura, manuales técnicos y reglamentos de laboratorio.
2. Entrevistar a docentes y, si aplica, personal técnico.
3. Aplicar una encuesta anónima a estudiantes elegibles.
4. Realizar observación e inventario del laboratorio con autorización.
5. Codificar hallazgos y relacionarlos con necesidades y atributos verificables.

Las entrevistas se analizarán mediante categorías: seguridad, secuencia de práctica, comprensión conceptual, retroalimentación, recursos, tiempo, documentación y restricciones. En la encuesta se reportarán respuestas válidas, distribución por ítem y síntesis de preguntas abiertas. Los datos se anonimizan; no se incluirán nombres, códigos estudiantiles ni información clínica.

## Instrumentos

La encuesta y el guion de entrevista se encuentran desarrollados en [Indagacion_social_y_necesidades.md](Indagacion_social_y_necesidades.md). Antes de aplicarlos, deben ser revisados por el docente y por la instancia institucional que corresponda. El inventario debe incluir: espacio, tomas, protecciones, elementos disponibles, estado de los equipos, normas de uso, número de grupos, tiempo por sesión y condiciones de almacenamiento.

## Resultado esperado de la fase

El resultado de la indagacion no será un prototipo, sino una matriz de evidencia que muestre qué necesidades provienen de qué actor y qué restricción del contexto condiciona cada decisión. La siguiente fase solo podrá fijar prioridades, métricas y objetivos cuantitativos cuando esta evidencia esté disponible.

## Referencias

Deslauriers, L., McCarty, L. S., Miller, K., Callaghan, K., & Kestin, G. (2019). Measuring actual learning versus feeling of learning in response to being actively engaged in the classroom. *Proceedings of the National Academy of Sciences, 116*(39), 19251-19257. https://doi.org/10.1073/pnas.1821936116

International Organization for Standardization. (2019). *ISO 14971:2019: Medical devices—Application of risk management to medical devices*. https://www.iso.org/standard/72704.html

Lavado-Anguera, S., Velasco-Quintana, P.-J., & Terron-Lopez, M.-J. (2024). Project-based learning as an experiential pedagogical methodology in engineering education: A review of the literature. *Education Sciences, 14*(6), 617. https://doi.org/10.3390/educsci14060617

Santos-Diaz, A., Montesinos, L., Barrera-Esparza, M., del Mar Perez-Desentis, M., & Salinas-Navarro, D. E. (2024). Implementing a challenge-based learning experience in a bioinstrumentation blended course. *BMC Medical Education, 24*, 528. https://doi.org/10.1186/s12909-024-05462-7
