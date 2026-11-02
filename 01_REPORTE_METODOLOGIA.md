# Reporte técnico de selección y justificación metodológica.
**Asignatura:** Ingeniería de Software.
**Unidad 1:** Cierre Sumativo.
**Proyecto Final:** DataDoc: Plataforma de Procesamiento, Estandarización y Análisis de Datos.
**Fecha:** 21/10/2026



## 1. Caracterización del sistema y entorno de proyecto.
- **Ámbito de dominio:** Procesamiento de datos, inteligencia artificial y visualización analítica.
- **Problema principal a resolver:** Facilitar el analisis de datos, poder eficientar la manera de analizar los datos y que sea más sencillo encontrar patrones.
- **Complejidad técnica y criticidad:**
  - *Complejidad:* Moderada o alta por el procesamiento de archivos e ingeniería de pipelines de preparación.
  - *Criticidad:* Moderada. Errores en la limpieza pueden corromper la integridad del dataset original. Se mitiga preservando el dataset original e implementando de una confirmación humana    antes del guardadar o exportar.
  - *Atributos de calidad:* Rendimiento, usabilidad e integridad de Datos (ISO/IEC 25010).
- **Perfil de integrantes y cliente:**
  - *Equipo de desarrollo:* Estudiantes de Ingeniería en Datos e Inteligencia Artificial (7° cuatrimestre) con competencias intermedias en Python y análisis de datos.
  - *Cliente / Product Owner:* Docente/Evaluado.


## 2. Evaluación multicriterio de alternativas metodológicas.
Para seleccionar la metodología de desarrollo más adecuada para DataDoc, se compararon tres enfoques: el tradicional, el ágil y el híbrido.

| Criterio | Enfoque clásico (Cascada) | Enfoque ágil | Enfoque híbrido propuesto |
|---|---|---|---|
| Gestión de cambios | Los cambios son difíciles de realizar porque las etapas siguen un orden establecido. | Permite realizar cambios durante el desarrollo según las necesidades del proyecto. | Combina la flexibilidad del enfoque ágil con una planificación y seguimiento organizados. |
| Documentación | Requiere documentación detallada antes de avanzar a la siguiente etapa. | Utiliza documentación sencilla y enfocada en lo necesario. | Mantiene documentación organizada sin generar trabajo innecesario. |
| Participación del usuario | El usuario participa principalmente al inicio y al final del proyecto. | El usuario puede dar opiniones y sugerencias durante el desarrollo. | Se revisan los avances al finalizar cada Sprint para realizar mejoras. |
| Entrega del software | El producto se entrega generalmente al finalizar el desarrollo. | Se entregan partes funcionales del sistema en periodos cortos. | Se desarrolla y entrega el sistema por etapas, comenzando por las funciones más importantes. |

## 3. Justificación de la metodología seleccionada.
- **Metodología seleccionada:** Enfoque híbrido basado en Scrum y prácticas de Extreme Programming (XP).

La elección de esta metodología se debe a que DataDoc necesita desarrollarse de manera organizada, pero también requiere flexibilidad para realizar cambios y mejoras durante el proceso.
Se tomaron como referencia los principios de los procesos de software de Ian Sommerville, adaptándolos a las necesidades del proyecto.

Las principales razones de esta elección son:

1. **Facilidad para realizar cambios:**
   Durante el desarrollo de DataDoc pueden surgir nuevas necesidades o modificaciones en la forma de procesar los datasets. Scrum permite organizar el trabajo en periodos cortos llamados Sprints, lo que facilita revisar los avances y realizar ajustes sin tener que reorganizar todo el proyecto.

2. **Mejora de la calidad del software:**
   Se incorporarán algunas prácticas de XP, como la revisión del código entre los integrantes, la corrección de errores y la mejora continua. Esto ayudará a mantener un código organizado y facilitará el mantenimiento del sistema.

3. **Mejor organización del equipo:**
   Al estar integrado por tres personas, el equipo necesita distribuir las actividades y responsabilidades de manera clara. Scrum permite organizar las tareas, establecer prioridades y revisar periódicamente el avance del proyecto.

4. **Entregas progresivas:**
   En lugar de desarrollar todas las funciones al mismo tiempo, DataDoc se construirá por etapas. Primero se trabajará en la carga y procesamiento de archivos, después en el análisis y finalmente en la limpieza opcional y presentación de resultados.


## 4. Definición del proceso adaptado y artefactos.
### Fases o ciclos del proceso.
El desarrollo de DataDoc se organizará mediante Sprints, en los cuales se trabajarán diferentes funcionalidades del sistema.

- **Sprint 1 (Duración: 1 semana): Carga y procesamiento de datos:**
  Se desarrollará la carga de archivos CSV y Excel, así como la lectura y procesamiento de su contenido. También se identificarán las filas, columnas y tipos de datos.

- **Sprint 2 (Duración: 1-2 semanas): Análisis de datos:**
  Se implementará la generación de estadísticas, la detección de valores faltantes y registros duplicados, además de la generación de resúmenes con información relevante.

- **Sprint 3 (Duración: 1-2 semanas): Limpieza y visualización:**
  Se desarrollarán las funciones de limpieza y estandarización opcional. También se trabajará en la presentación de resultados y, si el tiempo lo permite, en la exportación de reportes.

### Artefactos del proyecto.
Durante el desarrollo se generarán los siguientes elementos:

- **Documentación:** reporte de metodología, factibilidad y planificación, historias de usuario, Sprint Planning, requisitos del software, diagramas UML, diseño de base de datos y plan de pruebas.
- **Gestión del proyecto:** tablero Kanban, organización de tareas, seguimiento de Sprints y asignación de responsabilidades.
- **Código fuente:** archivos desarrollados en Python y archivos necesarios para configurar y ejecutar el sistema.
- **Control de versiones:** repositorio en GitHub para almacenar los avances y facilitar la colaboración.
- **Pruebas:** casos de prueba para verificar que las funcionalidades trabajen correctamente.

### Matriz de responsabilidades del equipo.
| Integrante | Rol | Responsabilidades principales |
|---|---|---|
| **Emmanuel Plata García** | Scrum Master / Desarrollador | Organizar el trabajo del equipo, dar seguimiento a las actividades y participar en el desarrollo de la carga de archivos. |
| **Oswaldo Guerrero García** | Product Owner / Desarrollador | Organizar y priorizar las funcionalidades, definir las necesidades del usuario y participar en el desarrollo del procesamiento y limpieza de datos. |
| **Emmanuel Barrientos Delgado** | Desarrollador / QA | Participar en el diseño del sistema, integrar los módulos, realizar pruebas y verificar el funcionamiento de las funcionalidades. |

## 5. Compromiso de calidad y organización del código.

### Estándares de calidad.
Para mantener la calidad de DataDoc se establecerán las siguientes medidas:

- **Organización del código:** mantener los archivos y módulos ordenados para facilitar su comprensión y mantenimiento.
- **Buenas prácticas de programación:** utilizar nombres claros para las variables y funciones, mantener una estructura consistente y evitar código innecesariamente repetido.
- **Revisión del código:** revisar los cambios realizados por los integrantes antes de integrarlos al proyecto principal.
- **Pruebas del sistema:** comprobar que cada funcionalidad cumpla con los resultados esperados.
- **Protección de los datos:** conservar los datos originales y aplicar operaciones de limpieza únicamente cuando el usuario las solicite.

### Criterios de calidad basados en ISO/IEC 25010.
Se tomarán en cuenta las siguientes características de calidad del software:

- **Adecuación funcional:** las funcionalidades deben cumplir con los requisitos y criterios de aceptación definidos en las historias de usuario.
- **Eficiencia de desempeño:** el sistema debe procesar los archivos de manera adecuada, considerando el tamaño de los datasets y los recursos disponibles.
- **Usabilidad:** la interfaz debe ser sencilla y permitir que el usuario comprenda los resultados del análisis.
- **Fiabilidad:** el sistema debe manejar correctamente los archivos válidos y mostrar mensajes claros cuando encuentre errores.
- **Mantenibilidad:** el código debe estar organizado para facilitar futuras modificaciones y mejoras.

### Mecanismos de control de cambios.
Para mantener organizado el desarrollo del proyecto se utilizarán las siguientes prácticas:

1. **Uso de Git y GitHub:** todos los cambios del proyecto se registrarán mediante el control de versiones.
2. **Ramas de trabajo:** cada integrante podrá trabajar en una rama independiente para desarrollar o modificar funcionalidades.
3. **Revisión de cambios:** antes de integrar modificaciones a la rama principal, se revisará que no existan errores y que los cambios funcionen correctamente.
4. **Cumplimiento de requisitos:** cada funcionalidad deberá cumplir con los criterios de aceptación de su historia de usuario.
5. **Actualización de documentación:** cuando se realicen cambios importantes en el funcionamiento del sistema, también se actualizará la documentación correspondiente.
