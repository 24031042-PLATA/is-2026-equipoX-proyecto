# Reporte Técnico de Selección y Justificación Metodológica

**Asignatura:** Ingeniería de Software  
**Unidad:** 1. Cierre Sumativo  
**Proyecto Final:** Plataforma de Procesamiento, Estandarización y Análisis de Datos  
**Nombre del proyecto:** Datermos  
**Fecha:** 21/10/2026

---

## 1. Introducción

El presente reporte técnico documenta la selección y justificación metodológica para el desarrollo de Datermos, una plataforma orientada al procesamiento, la estandarización y el análisis de conjuntos de datos.

El proyecto surge de la necesidad de facilitar el manejo de diferentes datasets mediante herramientas que permitan examinar su estructura, identificar información relevante y generar resultados comprensibles para los usuarios.

La plataforma busca integrar funciones de carga, procesamiento y análisis de datos, además de ofrecer operaciones opcionales de limpieza y estandarización cuando sean necesarias.

Este documento establece las bases para justificar las decisiones metodológicas y técnicas del proyecto, considerando sus objetivos, alcance y necesidades de desarrollo.

## 2. Descripción general del proyecto

Datermos es una propuesta de software que busca facilitar el análisis de conjuntos de datos provenientes de diferentes fuentes y con estructuras variables.

El sistema permitirá que el usuario cargue archivos compatibles para obtener información sobre su contenido, visualizar estadísticas descriptivas e identificar posibles problemas en los datos.

Asimismo, se contempla una función opcional de limpieza y estandarización que permitirá preparar la información antes de realizar análisis adicionales.

### 2.1 Objetivo general

Desarrollar una plataforma de procesamiento, estandarización y análisis de datos que facilite la exploración de datasets, la identificación de información relevante y la preparación opcional de los datos para su utilización posterior.

### 2.2 Objetivos específicos

- Permitir la carga de conjuntos de datos en formatos compatibles.
- Examinar la estructura y las características de los datos.
- Generar resúmenes y estadísticas descriptivas.
- Detectar valores faltantes y posibles inconsistencias.
- Ofrecer operaciones opcionales de limpieza y estandarización.
- Presentar los resultados de manera organizada y comprensible.
- Facilitar la interpretación de los datos mediante una interfaz accesible.

## 3. Problemática identificada

El análisis manual de datasets puede requerir tiempo y conocimientos técnicos, especialmente cuando los archivos contienen grandes cantidades de información, valores faltantes, formatos inconsistentes o estructuras diferentes.

Estas dificultades pueden complicar la interpretación de los datos y retrasar la identificación de información útil.

Por ello, Datermos propone centralizar operaciones básicas de procesamiento y análisis en una plataforma que permita explorar los datos y decidir cuándo es necesario realizar una limpieza o estandarización.

## 4. Alcance del proyecto

La primera versión de Datermos se enfocará en las siguientes funcionalidades:

- Carga de archivos en formatos definidos por el equipo.
- Visualización de la estructura general del dataset.
- Identificación del número de filas y columnas.
- Reconocimiento de los tipos de datos.
- Generación de estadísticas descriptivas.
- Detección de valores faltantes y posibles inconsistencias.
- Limpieza y estandarización opcionales.
- Presentación organizada de los resultados.

Las funciones avanzadas de análisis, automatización o detección de patrones complejos podrán considerarse en versiones posteriores, dependiendo del tiempo y los recursos disponibles.

## 5. Justificación de la selección metodológica

La metodología de desarrollo deberá permitir organizar el trabajo, establecer responsabilidades, documentar los requisitos y comprobar progresivamente el funcionamiento del sistema.

La selección definitiva de la metodología se justificará considerando:

- La complejidad de las funcionalidades.
- El tiempo disponible para desarrollar el proyecto.
- La distribución del trabajo entre los integrantes.
- La necesidad de probar los módulos durante su implementación.
- La posibilidad de realizar ajustes a partir de los resultados obtenidos.
- El control de versiones y la integración de los cambios mediante Git y GitHub.

La metodología elegida deberá favorecer el desarrollo gradual de Datermos y permitir verificar que cada función cumpla con los requisitos establecidos.

## 6. Tecnologías propuestas

| Tecnología | Aplicación en el proyecto |
|---|---|
| Python | Desarrollo de la lógica de procesamiento. |
| Pandas | Manipulación, limpieza y análisis de datos. |
| Streamlit | Construcción de la interfaz de usuario. |
| Visual Studio Code | Edición y desarrollo del código. |
| Git | Control de versiones. |
| GitHub | Gestión del repositorio y colaboración del equipo. |

Estas tecnologías constituyen una propuesta inicial y deberán confirmarse de acuerdo con las decisiones técnicas del equipo.

## 7. Resultados esperados

Al finalizar el desarrollo, se espera contar con una plataforma que permita:

1. Cargar datasets compatibles.
2. Consultar información general sobre su estructura.
3. Obtener estadísticas descriptivas.
4. Identificar posibles problemas en los datos.
5. Ejecutar operaciones de limpieza y estandarización cuando el usuario lo decida.
6. Consultar los resultados de forma organizada.

La validación de estos resultados se realizará mediante pruebas con archivos de ejemplo y la comparación de los resultados obtenidos con valores conocidos.

## 8. Conclusión

Datermos busca facilitar el procesamiento, la estandarización y el análisis de datasets mediante una plataforma que reúna funciones esenciales en una interfaz accesible.

La selección metodológica y tecnológica deberá responder a los objetivos del proyecto, los recursos disponibles y las necesidades del equipo de desarrollo.

La documentación de estas decisiones permitirá establecer una base organizada para las siguientes etapas de ingeniería de software, desde la especificación de requisitos hasta el diseño, la implementación y las pruebas.

---

**Documento elaborado para el proyecto Datermos.**