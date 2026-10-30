# Plan de Pruebas
**Asignatura:** Ingeniería de Software  
**Proyecto Final:** Plataforma de Procesamiento, Estandarización y Análisis de Datos  
**Equipo de Desarrollo:** Datermos  

---

## 1. Introducción

El presente documento establece las pruebas que se realizarán al sistema Datermos para verificar que sus funcionalidades cumplan con los requisitos establecidos.

Las pruebas permitirán identificar errores durante la carga, procesamiento, análisis y limpieza opcional de los datasets.

## 2. Objetivo

Comprobar que Datermos procese correctamente diferentes tipos de archivos, genere resultados útiles y permita realizar operaciones de limpieza cuando el usuario lo solicite.

## 3. Alcance de las pruebas

Se evaluarán las siguientes funcionalidades:

- Carga de archivos CSV y Excel.
- Lectura y procesamiento de datasets.
- Identificación de filas y columnas.
- Detección de valores faltantes.
- Detección de registros duplicados.
- Generación de estadísticas y resúmenes.
- Identificación de información relevante.
- Limpieza opcional de los datos.
- Manejo de archivos incorrectos o incompatibles.

## 4. Tipos de pruebas

### 4.1 Pruebas funcionales

Verifican que cada función del sistema realice correctamente la tarea para la que fue diseñada.

### 4.2 Pruebas de validación

Comprueban que el sistema identifique archivos vacíos, formatos no compatibles o datos incorrectos.

### 4.3 Pruebas de integración

Verifican que los módulos de carga, procesamiento, análisis y limpieza trabajen correctamente en conjunto.

### 4.4 Pruebas de usabilidad

Evalúan que el usuario pueda utilizar el sistema y comprender los resultados presentados.

## 5. Casos de prueba

| ID | Funcionalidad | Acción de prueba | Resultado esperado |
|---|---|---|---|
| CP-01 | Carga de archivos | Cargar un archivo CSV válido. | El sistema carga y muestra los datos. |
| CP-02 | Carga de archivos | Cargar un archivo Excel válido. | El sistema lee correctamente el contenido. |
| CP-03 | Validación | Cargar un archivo vacío. | El sistema informa que no hay datos para procesar. |
| CP-04 | Validación | Cargar un formato no compatible. | El sistema muestra un mensaje de error. |
| CP-05 | Procesamiento | Procesar un dataset válido. | El sistema identifica filas y columnas. |
| CP-06 | Análisis | Analizar un dataset con valores faltantes. | El sistema identifica los valores faltantes. |
| CP-07 | Análisis | Analizar un dataset con registros duplicados. | El sistema detecta los registros repetidos. |
| CP-08 | Estadísticas | Analizar columnas numéricas. | El sistema genera estadísticas descriptivas. |
| CP-09 | Resumen | Solicitar un resumen del dataset. | El sistema presenta información general y relevante. |
| CP-10 | Limpieza | Solicitar la eliminación de duplicados. | El sistema genera un resultado sin esos duplicados. |
| CP-11 | Limpieza | No solicitar modificaciones. | El sistema conserva los datos originales. |
| CP-12 | Integración | Ejecutar el proceso completo. | La carga, análisis y presentación de resultados funcionan correctamente. |

## 6. Datos de prueba

Para realizar las pruebas se utilizarán datasets de ejemplo que contengan diferentes características:

- Archivos CSV y Excel.
- Columnas numéricas y de texto.
- Valores faltantes.
- Registros duplicados.
- Columnas con diferentes tipos de información.
- Archivos vacíos o con formatos no compatibles.

Estos datos permitirán comprobar el comportamiento del sistema ante diferentes escenarios.

## 7. Criterios de aceptación

Una prueba se considerará satisfactoria cuando:

- El sistema cargue correctamente los archivos compatibles.
- Los datos se procesen sin errores.
- Las estadísticas y resúmenes correspondan con la información analizada.
- Los valores faltantes y duplicados se identifiquen correctamente.
- La limpieza se realice únicamente cuando el usuario la solicite.
- Los datos originales no se modifiquen accidentalmente.
- Los errores se comuniquen mediante mensajes comprensibles.

## 8. Registro de resultados

Los resultados de las pruebas se registrarán durante la etapa de implementación.

| ID de prueba | Resultado obtenido | Estado | Observaciones |
|---|---|---|---|
| CP-01 | Pendiente | No ejecutada | Se realizará durante las pruebas. |
| CP-02 | Pendiente | No ejecutada | Se realizará durante las pruebas. |
| CP-03 | Pendiente | No ejecutada | Se realizará durante las pruebas. |
| CP-04 | Pendiente | No ejecutada | Se realizará durante las pruebas. |
| CP-05 | Pendiente | No ejecutada | Se realizará durante las pruebas. |

**Nota:** Los casos restantes se registrarán de la misma manera conforme se ejecuten las pruebas.

## 9. Conclusión

El plan de pruebas permitirá verificar que Datermos cumpla con las funcionalidades establecidas y que el procesamiento de los datasets sea confiable.

Además, ayudará a detectar errores, mejorar el funcionamiento del sistema y comprobar que la limpieza de datos sea una operación opcional controlada por el usuario.