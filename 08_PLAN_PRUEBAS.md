# PLAN DE PRUEBAS.

**Asignatura:** Ingeniería de Software.  
**Proyecto Final:** Plataforma de Procesamiento, Estandarización y Análisis de Datos.  
**Nombre del proyecto:** DataDoc.  


## 1. Introducción.
Este documento describe las pruebas que se realizarán a DataDoc para comprobar que sus funciones trabajen correctamente.

Las pruebas ayudarán a encontrar errores al cargar archivos, procesar información, realizar análisis y limpiar los datos cuando el usuario lo solicite.

## 2. Objetivo.
Comprobar que DataDoc pueda cargar y analizar archivos correctamente, mostrar resultados claros y permitir la limpieza de datos cuando el usuario decida utilizarla.

## 3. Alcance de las pruebas.
Se realizarán pruebas a las siguientes funciones:

- Cargar archivos CSV y Excel.
- Leer y procesar los archivos.
- Identificar la cantidad de filas y columnas.
- Detectar datos faltantes.
- Encontrar registros duplicados.
- Generar estadísticas y resúmenes.
- Mostrar información importante de los datos.
- Realizar la limpieza de forma opcional.
- Identificar archivos vacíos o con formatos no permitidos.

## 4. Tipos de pruebas.
### 4.1 Pruebas funcionales:
Permiten comprobar que cada función del sistema realice correctamente su tarea.

### 4.2 Pruebas de validación:
Comprueban que el sistema pueda identificar archivos vacíos, formatos no permitidos o información incorrecta.

### 4.3 Pruebas de integración:
Verifican que las diferentes partes del sistema, como la carga, el procesamiento y el análisis, funcionen correctamente en conjunto.

### 4.4 Pruebas de usabilidad:
Permiten revisar que el usuario pueda utilizar el sistema fácilmente y entender los resultados que se muestran.

## 5. Casos de prueba:
En la siguiente tabla se muestran algunas pruebas que se realizarán para comprobar el funcionamiento de DataDoc.

| ID | Funcionalidad | Acción de prueba | Resultado esperado |
|---|---|---|---|
| CP-01 | Carga de archivos | Cargar un archivo CSV válido. | El sistema carga y muestra los datos. |
| CP-02 | Carga de archivos | Cargar un archivo Excel válido. | El sistema lee correctamente la información. |
| CP-03 | Validación | Cargar un archivo vacío. | El sistema indica que no hay datos para procesar. |
| CP-04 | Validación | Cargar un archivo con formato no permitido. | El sistema muestra un mensaje de error. |
| CP-05 | Procesamiento | Procesar un archivo válido. | El sistema identifica las filas y columnas. |
| CP-06 | Análisis | Analizar un archivo con datos faltantes. | El sistema identifica los datos faltantes. |
| CP-07 | Análisis | Analizar un archivo con datos repetidos. | El sistema detecta los registros duplicados. |
| CP-08 | Estadísticas | Analizar columnas con datos numéricos. | El sistema muestra estadísticas básicas. |
| CP-09 | Resumen | Solicitar un resumen del archivo. | El sistema muestra información general de los datos. |
| CP-10 | Limpieza | Solicitar la eliminación de duplicados. | El sistema genera una copia sin los registros duplicados. |
| CP-11 | Limpieza | No solicitar cambios en los datos. | El sistema conserva la información original. |
| CP-12 | Integración | Realizar el proceso completo. | La carga, el análisis y la presentación de resultados funcionan correctamente. |

## 6. Datos de prueba.
Para realizar las pruebas se utilizarán archivos de ejemplo que contengan diferentes tipos de información.

Se utilizarán:
- Archivos CSV y Excel.
- Columnas con números y texto.
- Datos faltantes.
- Registros repetidos.
- Columnas con diferentes tipos de datos.
- Archivos vacíos.
- Archivos con formatos no permitidos.

Estos archivos permitirán comprobar cómo responde el sistema en diferentes situaciones.

## 7. Criterios de aceptación.
Las pruebas se considerarán satisfactorias cuando:

- El sistema cargue correctamente los archivos CSV y Excel.
- La información se procese correctamente.
- Las estadísticas y los resúmenes coincidan con los datos del archivo.
- Se detecten los datos faltantes y repetidos.
- La limpieza se realice solamente cuando el usuario la solicite.
- Los archivos originales se conserven sin modificaciones.
- El sistema muestre mensajes claros cuando ocurra un error.

## 8. Registro de resultados.
Durante el desarrollo se registrarán los resultados de cada prueba para saber si funcionó correctamente o si necesita alguna corrección.

| ID de prueba | Resultado obtenido | Estado | Observaciones |
|---|---|---|---|
| CP-01 | Pendiente | No ejecutada | Se realizará durante las pruebas. |
| CP-02 | Pendiente | No ejecutada | Se realizará durante las pruebas. |
| CP-03 | Pendiente | No ejecutada | Se realizará durante las pruebas. |
| CP-04 | Pendiente | No ejecutada | Se realizará durante las pruebas. |
| CP-05 | Pendiente | No ejecutada | Se realizará durante las pruebas. |
| CP-06 | Pendiente | No ejecutada | Se realizará durante las pruebas. |
| CP-07 | Pendiente | No ejecutada | Se realizará durante las pruebas. |
| CP-08 | Pendiente | No ejecutada | Se realizará durante las pruebas. |
| CP-09 | Pendiente | No ejecutada | Se realizará durante las pruebas. |
| CP-10 | Pendiente | No ejecutada | Se realizará durante las pruebas. |
| CP-11 | Pendiente | No ejecutada | Se realizará durante las pruebas. |
| CP-12 | Pendiente | No ejecutada | Se realizará durante las pruebas. |


## 9. Conclusión.
El plan de pruebas permitirá comprobar que DataDoc funcione correctamente y cumpla con las funciones establecidas.
También ayudará a encontrar y corregir errores durante el desarrollo, verificar que los resultados sean correctos y asegurar que la limpieza de los datos sea opcional.

De esta manera, se busca que el sistema sea fácil de utilizar y que permita analizar la información de forma organizada y confiable.
