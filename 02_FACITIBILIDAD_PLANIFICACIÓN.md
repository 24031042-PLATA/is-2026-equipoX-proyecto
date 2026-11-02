
# PRÁCTICA 6. FACTIBILIDAD Y PLANIFICACIÓN DEL PROYECTO

**Proyecto:** DataDoc: Plataforma de Procesamiento, Estandarización y Análisis de Datos.

**Documento:** Estudio de factibilidad y planificación.

**Fecha:** 28 de octubre de 2026.



## 1. Introducción

Actualmente, muchas actividades necesitan trabajar con grandes cantidades de datos. Analizar toda esa información manualmente puede tomar mucho tiempo y dificultar la identificación de errores o datos importantes.

Por esta razón, se propone desarrollar DataDoc, una plataforma que permita cargar archivos, analizar su contenido y mostrar los resultados de manera organizada.

En esta práctica se estudia si el proyecto puede realizarse, qué herramientas y recursos se necesitan, cuánto tiempo podría tomar su desarrollo y qué problemas podrían presentarse durante el proceso.

## 2. Descripción del proyecto

DataDoc será una plataforma que ayudará a los usuarios a analizar diferentes conjuntos de datos mediante una interfaz sencilla.

El usuario podrá cargar un archivo compatible y el sistema mostrará información sobre su contenido, como un resumen, estadísticas y posibles problemas en los datos.

También contará con una opción para limpiar y organizar la información. Esta función será opcional, por lo que el usuario decidirá si desea realizar cambios en sus datos.

### 2.1 Problema que se busca resolver

Cuando una persona trabaja con muchos datos, puede ser complicado revisar toda la información manualmente.

Esto dificulta encontrar datos faltantes, identificar errores y comprender las características generales de un archivo.

DataDoc busca facilitar este trabajo mediante un sistema que procese la información y presente los resultados de forma clara.

### 2.2 Solución propuesta

Se propone desarrollar una aplicación que permita:

- Cargar archivos CSV y Excel.
- Mostrar información general del archivo.
- Identificar las filas, columnas y tipos de datos.
- Generar estadísticas básicas.
- Detectar datos faltantes y posibles errores.
- Mostrar información que pueda ser útil para el usuario.
- Ofrecer una opción para limpiar los datos.
- Presentar los resultados de manera ordenada.

## 3. Objetivos

### 3.1 Objetivo general

Desarrollar una plataforma que permita cargar, procesar y analizar conjuntos de datos para obtener resúmenes, estadísticas e información útil, incluyendo una opción de limpieza que el usuario pueda utilizar cuando lo necesite.

### 3.2 Objetivos específicos

1. Permitir que el usuario cargue archivos CSV y Excel.
2. Revisar la estructura y el contenido de los archivos.
3. Obtener estadísticas que ayuden a comprender los datos.
4. Identificar valores faltantes y posibles errores.
5. Ofrecer herramientas para limpiar y organizar los datos de manera opcional.
6. Mostrar los resultados mediante una interfaz sencilla.
7. Realizar pruebas para comprobar que el sistema funcione correctamente.

## 4. Estudio de factibilidad

El estudio de factibilidad permite conocer si el proyecto puede desarrollarse con los recursos disponibles.

Para ello, se revisan cuatro aspectos: las herramientas necesarias, los costos, la facilidad de uso y las consideraciones legales.

### 4.1 Factibilidad técnica

**Objetivo:** comprobar si contamos con las herramientas necesarias para desarrollar el proyecto.

Para construir DataDoc se propone utilizar las siguientes tecnologías:

| Tecnología | ¿Para qué se utilizará? |
|---|---|
| Python | Para programar las funciones del sistema. |
| Pandas | Para leer, organizar y analizar los datos. |
| Streamlit | Para crear la interfaz que utilizará el usuario. |
| Visual Studio Code | Para escribir y modificar el código. |
| Git | Para guardar y controlar los cambios del proyecto. |
| GitHub | Para almacenar el código y trabajar en equipo. |

En la primera versión se busca trabajar con archivos CSV y Excel.

**Evaluación:** el proyecto es técnicamente viable porque existen herramientas que permiten realizar las funciones necesarias sin tener que programar todo desde cero.

**Condiciones:** será necesario instalar las herramientas, configurar el proyecto y realizar pruebas con diferentes archivos para comprobar que funcionen correctamente.

### 4.2 Factibilidad económica

**Objetivo:** identificar cuánto costaría desarrollar el proyecto.

Se propone utilizar herramientas gratuitas o que cuenten con una versión gratuita, para evitar gastos innecesarios.

| Recurso | Costo previsto | Uso |
|---|---|---|
| Python | Gratuito | Programar el sistema. |
| Pandas | Gratuito | Procesar y analizar los datos. |
| Streamlit | Gratuito para desarrollo local | Crear la interfaz. |
| Visual Studio Code | Gratuito | Escribir el código. |
| Git | Gratuito | Controlar los cambios. |
| GitHub | Cuenta gratuita disponible | Guardar y compartir el proyecto. |
| Computadora | Recurso disponible | Desarrollar y probar el sistema. |


**Evaluación:** el proyecto es económicamente viable porque se pueden utilizar herramientas gratuitas y los equipos de cómputo disponibles.

**Consideraciones:** si en el futuro se desea publicar la aplicación en internet o contratar servicios adicionales, podrían generarse nuevos gastos.

### 4.3 Factibilidad operativa

**Objetivo:** comprobar si el sistema será fácil de utilizar.

DataDoc estará pensado para personas que necesitan analizar archivos de datos sin tener que realizar todo el proceso manualmente o escribir código.

#### ¿Cómo utilizará el usuario el sistema?

1. El usuario abre DataDoc.
2. Selecciona un archivo CSV o Excel.
3. El sistema revisa y procesa la información.
4. Se muestra un resumen del contenido del archivo.
5. El usuario puede consultar estadísticas y posibles problemas encontrados.
6. Si lo desea, puede utilizar la opción de limpieza.
7. El sistema muestra los resultados después de realizar los cambios.
8. Si esta función está disponible, el usuario podrá descargar el archivo procesado.

**Evaluación:** el proyecto es operativamente viable porque propone un proceso sencillo, en el que el usuario solo necesita cargar su archivo y consultar los resultados.

**Condiciones:** la interfaz debe ser fácil de entender y mostrar mensajes claros cuando ocurra algún error. También debe informar al usuario sobre los cambios realizados durante la limpieza.

### 4.4 Factibilidad legal

**Objetivo:** identificar los aspectos legales que deben respetarse durante el desarrollo y uso del sistema.

Para utilizar DataDoc correctamente, se deben considerar los siguientes puntos:

- **Licencias de software:** respetar las condiciones de uso de Python, Pandas, Streamlit y las demás herramientas utilizadas.
- **Derechos de los datos:** utilizar archivos propios o información cuyo uso esté permitido.
- **Privacidad:** proteger los datos personales o confidenciales que puedan contener los archivos.
- **Conservación de la información:** evitar modificar el archivo original sin autorización del usuario.
- **Seguridad:** procurar que los archivos del usuario se manejen de forma adecuada.

En la primera versión se propone que los archivos se procesen directamente en la computadora del usuario, sin enviarlos a otros servicios.

**Evaluación:** el proyecto es legalmente viable siempre que se respeten las licencias de las herramientas y se proteja la información utilizada.

## 5. Recursos necesarios

Para desarrollar DataDoc se necesitarán personas, programas y equipos de cómputo.

### 5.1 Recursos humanos

| Rol | Actividad |
|---|---|
| Desarrollo | Programar las funciones del sistema. |
| Diseño de interfaz | Organizar las pantallas y la información que verá el usuario. |
| Pruebas | Comprobar que el sistema funcione y encontrar errores. |
| Documentación | Elaborar los documentos del proyecto y las instrucciones de uso. |

Estas actividades se repartirán entre los integrantes del equipo de acuerdo con sus conocimientos y disponibilidad.

### 5.2 Recursos de software

- Python.
- Pandas.
- Streamlit.
- Visual Studio Code.
- Git.
- GitHub.

### 5.3 Recursos de hardware

- Una computadora para programar y ejecutar el sistema.
- Espacio de almacenamiento para guardar el código y los archivos de prueba.
- Conexión a internet para consultar información y trabajar con GitHub.

## 6. Planificación del proyecto

La planificación permite organizar las actividades y establecer cuánto tiempo se necesita para desarrollar el sistema.

Se propone realizar el proyecto en siete semanas. Este tiempo es una estimación y puede cambiar dependiendo del avance del equipo.

### 6.1 Cronograma de actividades

| Etapa | Actividades | Duración | Resultado esperado |
|---|---|---|---|
| 1. Análisis | Definir el problema, los objetivos y lo que hará el sistema. | 1 semana | Requisitos del proyecto. |
| 2. Diseño | Organizar cómo funcionará el sistema y elaborar los diagramas. | 1 semana | Diseño del sistema. |
| 3. Desarrollo inicial | Crear el proyecto, la interfaz y la carga de archivos. | 1 semana | Primera versión funcional. |
| 4. Análisis de datos | Programar los resúmenes y las estadísticas. | 1 semana | Funciones de análisis. |
| 5. Limpieza opcional | Agregar opciones para detectar y corregir problemas en los datos. | 1 semana | Funciones de limpieza. |
| 6. Pruebas | Probar diferentes archivos y corregir errores. | 1 semana | Sistema probado. |
| 7. Documentación y entrega | Terminar los documentos y preparar la entrega. | 1 semana | Proyecto final. |

**Duración total estimada: 7 semanas.**

### 6.2 Seguimiento del proyecto

Para conocer el avance y mantener organizado el trabajo, se propone:

- Revisar qué actividades ya se terminaron y cuáles faltan.
- Repartir las tareas entre los integrantes.
- Utilizar Git para guardar los cambios realizados.
- Revisar el código antes de agregar modificaciones al proyecto principal.
- Probar cada función después de desarrollarla.
- Actualizar los documentos cuando existan cambios en el proyecto.

## 7. Identificación de riesgos

Durante el desarrollo pueden presentarse situaciones que dificulten el trabajo o afecten el funcionamiento del sistema.

En la siguiente tabla se muestran algunos problemas posibles y cómo se podrían prevenir:

| Riesgo | Probabilidad | Impacto | ¿Cómo prevenirlo? |
|---|---|---|---|
| El archivo no es compatible. | Media | Medio | Comprobar el formato antes de procesarlo. |
| El archivo contiene demasiados datos. | Media | Alto | Probar archivos de diferentes tamaños. |
| Los datos tienen errores o están incompletos. | Alta | Medio | Detectar los problemas y avisar al usuario. |
| Se modifica o pierde el archivo original. | Media | Alto | Trabajar sobre una copia y conservar el original. |
| El equipo se retrasa con las actividades. | Media | Alto | Organizar las tareas y revisar los avances. |
| Aparecen errores al unir el trabajo de los integrantes. | Media | Medio | Revisar los cambios y realizar pruebas frecuentes. |
| Se utilizan datos privados sin protección. | Baja | Alto | Trabajar con archivos de prueba y proteger la información. |

Las probabilidades son estimaciones iniciales y podrán cambiar conforme avance el proyecto.

## 8. Alcance y limitaciones

En esta sección se explica qué funciones tendrá la primera versión de DataDoc y qué aspectos podrían quedar pendientes.

### 8.1 Alcance de la primera versión

La primera versión del sistema incluirá:

- Carga de archivos CSV y Excel.
- Visualización de filas y columnas.
- Identificación de los nombres y tipos de datos.
- Detección de valores faltantes.
- Generación de estadísticas básicas.
- Elaboración de un resumen general del archivo.
- Limpieza de datos de manera opcional.
- Presentación organizada de los resultados.
- Descarga de los datos procesados, si se implementa esta función.

### 8.2 Limitaciones previstas

- Solo se podrán cargar los formatos que el sistema tenga implementados.
- El funcionamiento dependerá del tamaño del archivo y de la capacidad de la computadora.
- Los resultados dependerán de la calidad de los datos cargados.
- La información identificada como relevante deberá ser revisada por el usuario, ya que su utilidad depende del contexto.
- Algunas funciones avanzadas podrían no estar disponibles en la primera versión.

### 8.3 Mejoras futuras

En futuras versiones se podrían agregar más formatos de archivos, nuevas gráficas, herramientas para encontrar patrones y opciones adicionales para limpiar los datos.

## 9. Conclusión

Después de analizar los diferentes aspectos del proyecto, se considera que DataDoc es viable para desarrollarse como un proyecto académico.

En el aspecto técnico, existen herramientas que permiten crear el sistema y procesar los archivos. En el aspecto económico, se pueden utilizar programas gratuitos, por lo que no se necesita una inversión importante para comenzar.

En cuanto a su uso, se busca que cualquier persona pueda cargar un archivo y consultar sus resultados mediante una interfaz sencilla. También será importante proteger la información y respetar las licencias de las herramientas utilizadas.

Finalmente, la planificación propuesta permite dividir el trabajo en diferentes etapas, organizar las actividades y reducir los posibles problemas durante el desarrollo.

Por lo tanto, se propone comenzar con las funciones principales de carga y análisis de datos, para después incorporar la limpieza opcional y otras mejoras conforme avance el proyecto.
