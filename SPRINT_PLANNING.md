# Planificación del Sprint 1 (Sprint Planning)

## 1. Meta del Sprint (Sprint Goal)

Construir el pipeline base de ingesta y preprocesamiento de datos, junto con el tablero de visualización de métricas, para tener un flujo funcional de extremo a extremo con validaciones de calidad.

## 2. Historias Compromiso para el Sprint 1

| ID | Historia de Usuario | Story Points | Responsable (Assignee) |
|---|---|---|---|
| 24031042 | Ingesta Automática de Archivos CSV | 5 pts | @EmmanuelPlataGarcia |
| 24031062 | Limpieza y Preprocesamiento de Datos | 8 pts | @OswaldoGuerreroGarcia |
| 24030202 | Tablero de Visualización de Métricas | 5 pts | @EmmanuelBarrientosDelgado |

**Total comprometido:** 18 Story Points

## 3. Acuerdos de Calidad Ágil

- **Definition of Ready (DoR):** Una historia entra al Sprint solo si tiene criterios de aceptación en Gherkin, estimación aprobada por el equipo y dependencias de BD resueltas.
- **Definition of Done (DoD):** Una historia se considera 'Hecha' solo si tiene código revisado por peer review en PR, cumple con el linter de estilo sin errores y los criterios de aceptación fueron validados.

## 4. Historias Diferidas al Sprint 2

| ID | Historia de Usuario | Story Points | Motivo de diferimiento |
|---|---|---|---|
| 24030202 | Entrenamiento de Modelo de Predicción | 13 pts | Depende de 24031042 completada |
| 24030202 | API de Predicciones en Tiempo Real | 8 pts | Depende de 24030202 completada |
| 24031062 | Exportación de Reportes en PDF | 3 pts | Prioridad baja, no bloquea el flujo base |   