# Inventario de Historias de Usuario - Proyecto Final

## Historia de Usuario 24031042: Ingesta Automática de Archivos CSV
- **ID:** 24031042
- **Nombre:** Ingesta Automática de Archivos CSV
- **Como:** Analista de Datos
- **Quiero:** Cargar un archivo CSV mediante interfaz web
- **Para:** Visualizar las métricas procesadas en el tablero general
- **Estimación (Story Points):** 5
- **Prioridad:** Alta
- **Criterios de Aceptación (Gherkin):**
  - **Escenario 1 (Carga Exitosa):** **Dado que** el usuario seleccionó un archivo .csv válido de menos de 10MB, **Cuando** hace clic en 'Procesar', **Entonces** el sistema valida las columnas y muestra el mensaje 'Datos cargados exitosamente'.
  - **Escenario 2 (Archivo Inválido):** **Dado que** el usuario selecciona un archivo con extensión no permitida (.docx), **Cuando** intenta cargarlo, **Entonces** el sistema bloquea el envío y muestra una alerta de error de formato.

## Historia de Usuario 24031042: Limpieza y Preprocesamiento de Datos
- **ID:** 24031042
- **Nombre:** Limpieza y Preprocesamiento de Datos
- **Como:** Científico de Datos
- **Quiero:** Que el sistema detecte y gestione automáticamente valores nulos, duplicados y outliers
- **Para:** Garantizar la calidad del dataset antes del entrenamiento del modelo
- **Estimación (Story Points):** 8
- **Prioridad:** Alta
- **Criterios de Aceptación (Gherkin):**
  - **Escenario 1 (Limpieza Automática):** **Dado que** el dataset contiene 5% de valores nulos y registros duplicados, **Cuando** se ejecuta el pipeline de preprocesamiento, **Entonces** el sistema elimina duplicados, imputa nulos con la mediana y genera un informe de cambios.
  - **Escenario 2 (Dataset Limpio):** **Dado que** el dataset no contiene nulos ni duplicados, **Cuando** se ejecuta el pipeline, **Entonces** el sistema reporta 'Dataset válido, sin cambios aplicados' y continúa al siguiente paso.

## Historia de Usuario 24030202: Entrenamiento de Modelo de Predicción
- **ID:** 24030202
- **Nombre:** Entrenamiento de Modelo de Predicción
- **Como:** Ingeniero de IA
- **Quiero:** Entrenar un modelo de machine learning sobre el dataset preprocesado
- **Para:** Obtener un modelo capaz de predecir la variable objetivo con precisión aceptable
- **Estimación (Story Points):** 13
- **Prioridad:** Alta
- **Criterios de Aceptación (Gherkin):**
  - **Escenario 1 (Entrenamiento Exitoso):** **Dado que** el dataset preprocesado tiene al menos 1000 filas y la variable objetivo está definida, **Cuando** se ejecuta el entrenamiento, **Entonces** el sistema genera un modelo con métricas (accuracy, precision, recall, F1) superiores al 75%.
  - **Escenario 2 (Dataset Insuficiente):** **Dado que** el dataset tiene menos de 100 filas, **Cuando** se intenta entrenar, **Entonces** el sistema muestra el error 'Datos insuficientes para entrenamiento' y sugiere ampliar el dataset.

## Historia de Usuario 24031062: Tablero de Visualización de Métricas
- **ID:** 24031062
- **Nombre:** Tablero de Visualización de Métricas
- **Como:** Product Owner
- **Quiero:** Visualizar en un dashboard las métricas clave del proyecto en tiempo real
- **Para:** Tomar decisiones informadas sobre el avance y calidad del modelo
- **Estimación (Story Points):** 5
- **Prioridad:** Media
- **Criterios de Aceptación (Gherkin):**
  - **Escenario 1 (Visualización Correcta):** **Dado que** el modelo está entrenado y las métricas están disponibles, **Cuando** el usuario accede al tablero, **Entonces** se muestran gráficas de accuracy, distribución de datos y tiempo de inferencia.
  - **Escenario 2 (Sin Modelo Entrenado):** **Dado que** no existe un modelo entrenado, **Cuando** el usuario accede al tablero, **Entonces** se muestra el mensaje 'Entrene un modelo para ver las métricas'.

## Historia de Usuario 24030202 API de Predicciones en Tiempo Real
- **ID:** 24030202
- **Nombre:** API de Predicciones en Tiempo Real
- **Como:** Desarrollador
- **Quiero:** Consumir una API REST que devuelva predicciones del modelo
- **Para:** Integrar la capacidad predictiva en aplicaciones externas
- **Estimación (Story Points):** 8
- **Prioridad:** Media
- **Criterios de Aceptación (Gherkin):**
  - **Escenario 1 (Predicción Exitosa):** **Dado que** el modelo está desplegado y el usuario envía un POST con los features correctos, **Cuando** la API recibe la solicitud, **Entonces** devuelve un JSON con la predicción y su probabilidad en menos de 500ms.
  - **Escenario 2 (Solicitud Inválida):** **Dado que** el usuario envía un POST con campos faltantes o de tipo incorrecto, **Cuando** la API procesa la solicitud, **Entonces** devuelve un error HTTP 400 con el mensaje 'Payload inválido: [campo] requerido'.

## Historia de Usuario 24031062: Exportación de Reportes en PDF
- **ID:** 24031062
- **Nombre:** Exportación de Reportes en PDF
- **Como:** Product Owner
- **Quiero:** Descargar un reporte en PDF con los resultados del análisis
- **Para:** Compartir los hallazgos con stakeholders que no tienen acceso a la plataforma
- **Estimación (Story Points):** 3
- **Prioridad:** Baja
- **Criterios de Aceptación (Gherkin):**
  - **Escenario 1 (Exportación Exitosa):** **Dado que** existe al menos un análisis completado, **Cuando** el usuario hace clic en 'Exportar Reporte', **Entonces** se genera y descarga un PDF con gráficas, métricas y resumen ejecutivo.
  - **Escenario 2 (Sin Datos para Exportar):** **Dado que** no hay análisis completados, **Cuando** el usuario intenta exportar, **Entonces** el sistema muestra la alerta 'No hay datos disponibles para generar el reporte'.   