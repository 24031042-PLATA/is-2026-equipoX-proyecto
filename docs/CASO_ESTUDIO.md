# CASO DE ESTUDIO: Plataforma dedicada a el procesamiento y estandarización de datos

## 1. Definición del Problema Real

Dia a dia se reciben archivos de datos provenientes de multiples fuentes y con formatos distitnos. Estos archivos pueden albergar informacion incompleta, columnas con nombres inconsistentes, valores duplicados, errores de formato y datos que nos estan estandarizados. La revision y preparacion manual de esta informacion ocupa tiempo, conocimientos tecnicos y esfuerzo, lo que entorpece su analisis y aprovechamiento.

El proyecto propone desarrollar un software capaz de cargar archivos CSv, JSON y XLSX para procesarlos, limpiarlos, estandarizarlos, mapearlos y analizarlo. La solución usará una Inteligencia Artificial conectada mediante una API. Por medio de un chat, la IA preguntará al usuario cual es el objetivo del archivo y, con base en sus respuestas, sugerirá el mapeo de campos, detectará datos faltantes y recomendará acciones de limpieza y estandarización. El usuario podrá revisar y confirmar os cambios antes de generar el archivo procesado. 

## 2. Objetivos del Sistema

- **Objetivo General:** Desarrollar una plataforma capaz de cargar, procesar, limpiar, estandarizar, mapear y analizar archivos CSV, JSON y XLSX con el apoyo de una Inteligencia Artificial conectada mediante una API.
- **Objetivos Específicos:**
  1. Permitir la carga y el análisis inicial de archivos CSV, JSON y XLSX, identificando su estructura, columnas, tipos de datos y problemas de calidad.
  2. Utilizar un chat con inteligencia artificial para conocer el objetivo del archivo, proponer el mapeo de sus campos y detectar información faltante, duplicados, valores inválidos e inconsistencias.
  3. Aplicar procesos de limpieza y estandarización, generar un archivo procesado y mostrar un resumen de las transformaciones realizadas.
  4. Implementar, si el tiempo disponible lo permite, un dashboard con indicadores y gráficas que pueda ser consultado o expuesto por un agente sin IA.

## 3. Actores del Sistema (Usuarios)

| Actor | Rol y Responsabilidad | Perfil Técnico | Access Level |
|---|---|---|---|
| Administrador | Configura la plataforma, la conexión con la API y los parámetros generales del sistema. | Técnico alto | Full |
| Operador / Analista | Carga archivos, conversa con la IA, revisa las sugerencias, confirma transformaciones y descarga los resultados. | Medio | Read/Write |
| Usuario final | Consulta los archivos procesados, reportes y, si se implementa, el dashboard. | Básico | Read Only |
| Agente sin IA | Expone o consulta la información procesada y el dashboard mediante las funciones disponibles del sistema. | Medio | Read Only |

## 4. Alcance y Límites del Proyecto

- **Incluye:**
  - Carg y lectura de archivos CSV, JSON y XLSX.
  - Análisis de la estructura y calidad de los datos.
  - Detección de campos faltantes, duplicados, valores inválidos y errores de formato.
  - Mapeo de columnas de acuerdo con el objetivo indicado por el usuario.
  - Limpieza y estandarización de datos con revisión/confirmación del usuario.
  - Interación con una inteligencia artificial mediante API y chat.
  - Exportación del archivo procesado y un resumen de los cambios realizados.
  - Análisis básico de los datos resultantes.
  - Desarrollo de un dashboard visual y su consulta mediante un agente sin IA, sujeto al tiempo disponible.

- **No Incluye:**
  - Procesamiento de bases de datos empresariales en tiempo real.
  - Automatización de cambios sin revisión o confirmación del usuario.
  - Garantía de que la inteligencia artificial corriga todos los errores sin intervención humana.
  - Integraciones con múltiples sistemas extrnos fuera de la API necesaria para el funcionamiento inicial.
  - Un dashboard avanzado si no se cuenta con el tiempo suficiente para implementarlo y validarlo.
