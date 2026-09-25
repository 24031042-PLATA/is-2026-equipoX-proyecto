# MATRIZ DE EVALUACIÓN DE RIESGOS (MODELO EN ESPIRAL)

| ID | Descripción del Riesgo | Probabilidad | Impacto | Estrategia de Mitigación |
|---|---|---|---|---|
| R-01 | Requisitos ambiguos sobre el objetivo que debe cumplir cada archivo. | Media | Alto | Definir los requisitos y criterios de aceptación; utilizar el chat para confirmar el objetivo del usuario antes de aplicar transformaciones. |
| R-02 | Archivos CSV, JSON o XLSX con estructuras dañadas, formatos inesperados o información incompleta. | Alta | Alto | Validar el tipo y la estructura del archivo, mostrar errores claros y conservar una copia del archivo original antes de procesarlo. |
| R-03 | La IA puede interpretar incorrectamente el objetivo del archivo o proponer un mapeo inadecuado. | Media | Alto | Solicitar confirmación al usuario, mostrar las sugerencias antes de aplicarlas y permitir deshacer o corregir el mapeo. |
| R-04 | Errores en la limpieza o estandarización que modifiquen datos válidos. | Media | Alto | Mantener los datos originales, registrar cada transformación, validar los resultados y requerir autorización del usuario para aplicar cambios. |
| R-05 | Fallas, límites de uso o cambios en la API de inteligencia artificial. | Media | Alto | Implementar manejo de errores visible, validar las respuestas de la API, limitar las solicitudes y contar con un flujo básico de procesamiento sin IA cuando sea posible. |
| R-06 | Problemas de rendimiento al procesar archivos grandes. | Media | Medio | Establecer un tamaño máximo inicial, procesar la información por bloques y realizar pruebas con archivos de diferentes tamaños. |
| R-07 | Retrasos en el desarrollo por no tener fechas de entrega definidas o por distribuir inadecuadamente las tareas. | Media | Medio | Organizar el trabajo en un tablero Kanban, revisar avances periódicamente y priorizar primero la carga, validación, limpieza y exportación de archivos. |
| R-08 | El dashboard no se completa por falta de tiempo o por problemas de integración. | Media | Medio | Considerarlo como funcionalidad secundaria y garantizar primero el flujo principal de procesamiento; implementar inicialmente reportes simples si el dashboard completo no es viable. |
