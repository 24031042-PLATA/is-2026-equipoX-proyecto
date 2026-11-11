# REPORTE TÉCNICO DE SELECCIÓN Y JUSTIFICACIÓN METODOLOGICA.
**Asignatura:** Ingeniería de Software.  
**Unidad:** 1. Cierre Sumativo.  
**Proyecto Final:** Plataforma de Procesamiento, Estandarización y Análisis de Datos.  
**Nombre del proyecto:** DataDoc.
**Fecha:** 21/10/2026

## 1. Introducción.
El este reporte se explica cómo se organizará el desarrollo de DataDoc, una plataforma que permitirá procesar, organizar y analizar conjuntos de datos.

El proyecto surge de la necesidad de facilitar el manejo de archivos que contienen información, permitiendo conocer su contenido, encontrar datos importantes y obtener resultados fáciles de entender.

La plataforma contará con funciones para cargar archivos, revisar su información y realizar análisis. También permitirá limpiar y organizar los datos de manera opcional, cuando el usuario lo necesite.

En este documento se presentan los objetivos, el alcance, las tecnologías y la metodología que se tomarán en cuenta para desarrollar el proyecto.

## 2. Descripción general del proyecto
DataDoc es un proyecto de software que busca facilitar el análisis de conjuntos de datos que pueden tener diferentes cantidades y tipos de información.

El usuario podrá cargar archivos compatibles y obtener información sobre su contenido, como la cantidad de filas y columnas, los tipos de datos y algunas estadísticas.

También se podrán identificar datos faltantes o repetidos. Además, el sistema ofrecerá opciones para limpiar y organizar la información, pero el usuario decidirá si desea utilizarlas.

### 2.1 Objetivo general
Desarrollar una plataforma que permita cargar, procesar y analizar conjuntos de datos para conocer su contenido, identificar información importante y realizar una limpieza opcional.

### 2.2 Objetivos específicos
- Permitir la carga de archivos en formatos compatibles.
- Revisar la estructura y el contenido de los datos.
- Mostrar la cantidad de filas y columnas.
- Obtener estadísticas básicas de la información.
- Detectar datos faltantes y repetidos.
- Ofrecer opciones para limpiar y organizar los datos.
- Mostrar los resultados de forma clara y ordenada.
- Facilitar la comprensión de la información mediante una interfaz sencilla.

## 3. Problemática identificada
Revisar y analizar archivos de datos manualmente puede tomar mucho tiempo, especialmente cuando contienen mucha información o presentan problemas como datos faltantes, repetidos o desorganizados.
Esto puede dificultar la comprensión de la información y hacer más complicado encontrar datos importantes.
Por esta razón, DataDoc busca reunir diferentes funciones en una sola plataforma para que el usuario pueda revisar sus archivos, conocer sus características y obtener resultados sin tener que realizar todo el proceso manualmente.

## 4. Alcance del proyecto
La primera versión de DataDoc contará con las siguientes funciones:
- Cargar archivos CSV y Excel.
- Mostrar el contenido de los archivos.
- Identificar la cantidad de filas y columnas.
- Reconocer los tipos de datos.
- Obtener estadísticas básicas.
- Detectar datos faltantes y repetidos.
- Permitir la limpieza y organización de los datos de forma opcional.
- Mostrar los resultados del análisis de manera ordenada.
- Permitir descargar los resultados del análisis, si se completa esta funcionalidad durante el desarrollo.

## 5. Justificación de la selección metodológica
Para desarrollar DataDoc es importante contar con una metodología que permita organizar las actividades, repartir responsabilidades y revisar el avance del proyecto.
La metodología se seleccionará tomando en cuenta los siguientes aspectos:
- La dificultad de las funciones que tendrá el sistema.
- El tiempo disponible para desarrollar el proyecto.
- La distribución de actividades entre los integrantes.
- La necesidad de realizar pruebas durante el desarrollo.
- La posibilidad de corregir errores y hacer mejoras.
- El uso de Git y GitHub para guardar y organizar los cambios del código.

## 6. Tecnologías propuestas
| Tecnología | Uso en el proyecto |
|---|---|
| Python | Crear las funciones principales del sistema. |
| Pandas | Leer, organizar y analizar los datos. |
| Streamlit | Crear la interfaz que utilizará el usuario. |
| Visual Studio Code | Escribir y modificar el código. |
| Git | Guardar y controlar los cambios del proyecto. |
| GitHub | Compartir el código y trabajar en equipo. |


## 7. Resultados esperados
Al finalizar el desarrollo, se espera contar con una plataforma que permita:
1. Cargar archivos CSV y Excel.
2. Conocer la cantidad de filas, columnas y tipos de datos.
3. Obtener estadísticas básicas.
4. Identificar datos faltantes y repetidos.
5. Limpiar y organizar los datos cuando el usuario lo decida.
6. Consultar los resultados de manera clara y ordenada.
7. Descargar los resultados del análisis, si esta función queda implementada.

## 8. Conclusión
DataDoc busca facilitar el trabajo con conjuntos de datos mediante una plataforma que permita cargar archivos, revisar su contenido y obtener información útil.
También ofrecerá opciones de limpieza para que el usuario pueda decidir si desea modificar y organizar sus datos.

La elección de las tecnologías y la metodología permitirá organizar el desarrollo, repartir las actividades y revisar el funcionamiento de cada parte del sistema.

Este reporte establece una base para continuar con las siguientes etapas del proyecto, como la definición de requisitos, el diseño, la programación y las pruebas.

