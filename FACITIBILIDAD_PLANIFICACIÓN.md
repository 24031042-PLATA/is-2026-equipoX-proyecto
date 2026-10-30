
# PRÁCTICA 6. FACTIBILIDAD Y PLANIFICACIÓN DEL PROYECTO
**Proyecto:** Plataforma de Procesamiento, Estandarización y Análisis de Datos. 
**Documento:** Estudio de factibilidad y planificación.  
**Fecha:** 28 / ctubre / 2026
**Equipo:** Datermos.


## Índice
1. Introducción.
2. Descripción del proyecto.
3. Objetivos.
4. Estudio de factibilidad.
   - 4.1 Factibilidad técnica.
   - 4.2 Factibilidad económica.
   - 4.3 Factibilidad operativa.
   - 4.4 Factibilidad legal.
5. Recursos necesarios.
6. Planificación del proyecto.
7. Identificación de riesgos.
8. Alcance y limitaciones.
9. Conclusión.


## 1. Introducción
El análisis de datos es un proceso importante para comprender información, identificar patrones y apoyar la toma de decisiones. Pero revisar grandes cantidades de datos manualmente puede resultar complicado y consumir mucho tiempo.

Por eso se propone desarrollar un sistema de software que permita cargar diferentes conjuntos de datos, conocidos como *datasets*, procesarlos y presentar sus resultados.

En esta práctica se analiza la factibilidad del proyecto desde los aspectos técnico, económico, operativo y legal. También se encuentran los recursos necesarios, las actividades de desarrollo y los posibles riesgos.


## 2. Descripción del proyecto
El proyecto consiste en desarrollar una plataforma que facilite el análisis de diferentes conjuntos de datos mediante una interfaz sencilla. 

El usuario puede cargar un archivo compatible y obtener un resumen de su contenido, estadísticas descriptivas e información que pueda resultar relevante. Adicionalmente, podrá utilizar una función de limpieza de datos cuando lo considere necesario.

La limpieza será opcional, de modo que el usuario pueda consultar primero los datos originales y decidir si desea aplicar cambios.

### 2.1 Problema que se busca resolver

Analizar datasets manualmente puede dificultar la identificación de valores faltantes, características generales, estadísticas y posibles inconsistencias.

El sistema busca reducir este esfuerzo mediante el procesamiento automatizado y la presentación organizada de los resultados.

### 2.2 Solución propuesta

Desarrollar una aplicación que permita:

- Cargar conjuntos de datos desde archivos compatibles.
- Mostrar información general sobre los datos.
- Generar estadísticas descriptivas.
- Detectar valores faltantes y posibles inconsistencias.
- Identificar información potencialmente relevante.
- Ofrecer herramientas de limpieza de datos de manera opcional.
- Presentar los resultados en una interfaz comprensible.

## 3. Objetivos

### 3.1 Objetivo general

Desarrollar un sistema de análisis y procesamiento de datasets que permita obtener resúmenes, estadísticas e información relevante de manera organizada, ofreciendo funciones opcionales para la limpieza de datos.

### 3.2 Objetivos específicos

1. Permitir la carga de archivos de datos en formatos compatibles.
2. Procesar los datos para conocer su estructura y características generales.
3. Generar estadísticas descriptivas que faciliten su interpretación.
4. Identificar valores faltantes y posibles inconsistencias.
5. Implementar una función opcional de limpieza que permita preparar los datos para su análisis.
6. Presentar los resultados mediante una interfaz sencilla.
7. Realizar pruebas para comprobar el funcionamiento y la confiabilidad del sistema.

## 4. Estudio de factibilidad

El estudio de factibilidad permite determinar si el proyecto puede desarrollarse considerando las herramientas disponibles, los costos, la forma de utilización y los aspectos legales.

### 4.1 Factibilidad técnica

**Objetivo:** determinar si se cuenta con las tecnologías y los recursos necesarios para desarrollar el sistema.

Se propone utilizar las siguientes tecnologías:

| Tecnología | Función dentro del proyecto |
|---|---|
| Python | Implementar la lógica y el procesamiento de datos. |
| Pandas | Leer, organizar y analizar los datasets. |
| Streamlit | Construir la interfaz de usuario. |
| Visual Studio Code | Editar y desarrollar el código. |
| Git | Controlar las versiones del proyecto. |
| GitHub | Alojar el repositorio y facilitar la colaboración. |

Para la primera versión se propone admitir archivos CSV y Excel. La compatibilidad definitiva dependerá de las funciones implementadas y de las bibliotecas utilizadas.

**Evaluación:** el proyecto es técnicamente viable porque existen herramientas que permiten implementar las funciones principales sin desarrollar desde cero todos los componentes.

**Condiciones:** será necesario instalar y configurar las dependencias, comprobar la compatibilidad de los archivos y realizar pruebas con datasets de distintos tamaños y características.

### 4.2 Factibilidad económica

**Objetivo:** evaluar los costos necesarios para desarrollar y utilizar el sistema.

Se propone utilizar herramientas gratuitas y de código abierto cuando sea posible.

| Recurso | Costo previsto | Justificación |
|---|---|---|
| Python | Sin costo de licencia | Permite desarrollar la lógica del sistema. |
| Pandas | Sin costo de licencia | Facilita el procesamiento de datos. |
| Streamlit | Sin costo para el desarrollo local | Permite crear la interfaz. |
| Visual Studio Code | Sin costo de licencia | Se utiliza para programar. |
| Git | Sin costo de licencia | Permite controlar versiones. |
| GitHub | Plan gratuito disponible | Facilita el almacenamiento del repositorio. |
| Equipo de cómputo | Recurso disponible | Se utilizará para desarrollar y probar el sistema. |
| Alojamiento web | No requerido inicialmente | La primera versión podrá ejecutarse localmente. |

**Evaluación:** el proyecto es económicamente viable para un desarrollo académico local, siempre que se cuente con una computadora y acceso a los recursos necesarios.

**Consideraciones:** publicar la aplicación en internet, utilizar infraestructura adicional o contratar servicios externos podría generar costos posteriores.

### 4.3 Factibilidad operativa

**Objetivo:** determinar si el sistema podrá utilizarse de manera práctica por sus usuarios.

La aplicación estará orientada a personas que necesitan analizar datos sin tener que programar manualmente cada operación.

#### Flujo de funcionamiento propuesto

1. El usuario abre la aplicación.
2. Selecciona y carga un archivo compatible.
3. El sistema verifica y procesa su contenido.
4. Se presenta un resumen con las características principales del dataset.
5. Se muestran estadísticas y posibles datos relevantes.
6. El usuario decide si desea utilizar la función de limpieza.
7. Si aplica una limpieza, revisa los cambios y los resultados.
8. El usuario puede descargar los datos procesados si esta función está implementada.

**Evaluación:** el proyecto es operativamente viable porque propone un flujo de trabajo sencillo y organizado.

**Condiciones:** la interfaz deberá presentar mensajes claros, informar sobre los errores de carga y permitir que el usuario comprenda qué cambios se realizan durante la limpieza.

### 4.4 Factibilidad legal

**Objetivo:** identificar las consideraciones legales relacionadas con el desarrollo y uso del sistema.

Se deberán considerar los siguientes aspectos:

- **Licencias de software:** revisar las condiciones de uso y distribución de Python, Pandas, Streamlit y las demás dependencias.
- **Derechos sobre los datos:** utilizar archivos propios o datasets cuyo uso esté autorizado.
- **Privacidad:** evitar la exposición de información personal o confidencial.
- **Integridad de los datos:** conservar el archivo original y evitar modificaciones no autorizadas.
- **Seguridad:** informar al usuario sobre el tratamiento de sus archivos y limitar el acceso a la información.

Para la versión local se propone procesar los archivos en el equipo del usuario, sin enviarlos a servicios externos, salvo que una función futura requiera expresamente ese comportamiento.

**Evaluación:** el proyecto es legalmente viable si se respetan las licencias aplicables, los derechos sobre los datos y las obligaciones de privacidad correspondientes.

## 5. Recursos necesarios

### 5.1 Recursos humanos

| Rol | Responsabilidad |
|---|---|
| Desarrollo | Implementar la lógica y las funciones del sistema. |
| Diseño de interfaz | Organizar la presentación de la información. |
| Pruebas | Verificar el funcionamiento y detectar errores. |
| Documentación | Elaborar los documentos técnicos y el manual de usuario. |

Los roles podrán distribuirse entre los integrantes del equipo según sus habilidades y disponibilidad.

### 5.2 Recursos de software

- Python.
- Pandas.
- Streamlit.
- Visual Studio Code.
- Git.
- GitHub.

### 5.3 Recursos de hardware

- Computadora para programar y ejecutar la aplicación.
- Espacio de almacenamiento para el código y los archivos de prueba.
- Conexión a internet para consultar documentación y colaborar en el repositorio.

## 6. Planificación del proyecto

La planificación organiza las actividades necesarias para desarrollar el sistema. La siguiente propuesta contempla siete semanas de trabajo y deberá ajustarse al calendario real del equipo.

### 6.1 Cronograma de actividades

| Etapa | Actividades principales | Duración estimada | Resultado esperado |
|---|---|---|---|
| 1. Análisis | Definir el problema, los objetivos y los requisitos. | 1 semana | Requisitos del sistema. |
| 2. Diseño | Definir la arquitectura y elaborar los diagramas. | 1 semana | Diseño del sistema. |
| 3. Desarrollo inicial | Crear la estructura del proyecto, la interfaz y la carga de archivos. | 1 semana | Primera versión funcional. |
| 4. Análisis de datos | Implementar resúmenes y estadísticas descriptivas. | 1 semana | Módulo de análisis. |
| 5. Limpieza opcional | Desarrollar funciones para detectar y tratar problemas en los datos. | 1 semana | Módulo de limpieza. |
| 6. Pruebas | Probar distintos archivos, verificar resultados y corregir errores. | 1 semana | Versión probada. |
| 7. Documentación y entrega | Preparar documentación, revisar el repositorio y organizar la entrega. | 1 semana | Versión final documentada. |

**Duración total estimada: 7 semanas.**

### 6.2 Seguimiento del proyecto

Para comprobar el avance se propone:

- Registrar las actividades completadas y pendientes.
- Distribuir las tareas entre los integrantes.
- Utilizar Git para controlar los cambios.
- Revisar el código antes de integrar modificaciones.
- Realizar pruebas al finalizar cada módulo.
- Actualizar la documentación cuando cambien los requisitos o el diseño.

## 7. Identificación de riesgos

Los riesgos son situaciones que podrían afectar el desarrollo, el funcionamiento o la entrega del proyecto.

| Riesgo | Probabilidad estimada | Impacto | Medida preventiva |
|---|---|---|---|
| Archivos incompatibles | Media | Medio | Definir los formatos admitidos y validar los archivos. |
| Datasets demasiado grandes | Media | Alto | Probar los límites de memoria y optimizar el procesamiento. |
| Datos incompletos o inconsistentes | Alta | Medio | Detectar valores faltantes y advertir al usuario. |
| Pérdida o modificación accidental de datos | Media | Alto | Conservar el archivo original y trabajar sobre una copia. |
| Retrasos en el desarrollo | Media | Alto | Priorizar las funciones esenciales y revisar el avance. |
| Errores de integración | Media | Medio | Usar Git, revisar cambios y ejecutar pruebas frecuentes. |
| Uso de datos confidenciales sin protección | Baja | Alto | Utilizar datos de prueba y aplicar medidas de privacidad. |

Las probabilidades son estimaciones iniciales y deberán revisarse durante el desarrollo.

## 8. Alcance y limitaciones

### 8.1 Alcance de la primera versión

La primera versión se enfocará en las siguientes funciones:

- Carga de archivos CSV y Excel.
- Visualización de filas, columnas y nombres de campos.
- Identificación de los tipos de datos.
- Detección de valores faltantes.
- Generación de estadísticas descriptivas básicas.
- Presentación de un resumen general.
- Limpieza opcional de datos.
- Visualización de resultados de forma organizada.
- Descarga de los datos procesados, si se implementa esta función.

### 8.2 Limitaciones previstas

- El sistema solo admitirá los formatos que se implementen.
- El rendimiento dependerá del tamaño del dataset y de los recursos del equipo.
- Los resultados dependerán de la calidad y estructura de los datos.
- La identificación de información relevante no garantiza conclusiones correctas para todos los contextos.
- Las funciones avanzadas podrán quedar fuera de la primera versión.

### 8.3 Mejoras futuras

En versiones posteriores se podrían incorporar nuevos formatos, visualizaciones avanzadas, métodos de detección de patrones y herramientas adicionales de limpieza.

## 9. Conclusión

A partir del análisis realizado, se considera que el desarrollo del sistema de análisis y procesamiento de datasets es viable para un proyecto académico.

La factibilidad técnica se sustenta en la disponibilidad de herramientas que permiten procesar datos y crear una interfaz. La factibilidad económica es favorable para una primera versión local, debido a que pueden utilizarse herramientas sin costo de licencia. La factibilidad operativa depende de ofrecer una interfaz comprensible, mientras que la factibilidad legal requiere respetar las licencias, la privacidad y los derechos sobre los datos.

La planificación propuesta divide el desarrollo en etapas que facilitan la organización del trabajo, el seguimiento de los avances y la detección de riesgos.

En conclusión, el proyecto puede desarrollarse de manera gradual, comenzando con las funciones esenciales de carga y análisis, para después incorporar la limpieza opcional y otras mejoras según los resultados de las pruebas.