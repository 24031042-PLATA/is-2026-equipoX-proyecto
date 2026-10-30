# Reporte Técnico de Selección y Justificación Metodológica
**Asignatura:** Ingeniería de Software | **Unidad 1:** Cierre Sumativo.
**Proyecto Final:** Plataforma de Procesamiento, Estandarización y Análisis de Datos.
**Equipo de Desarrollo:** Datermos. | **Fecha:** 21/10/2026



## 1. Caracterización del Sistema y Entorno de Proyecto
- **Ámbito de Dominio:** Procesamiento de Datos, Inteligencia Artificial y Visualización Analítica.
- **Problema Principal a Resolver:** Ineficiencia, costo temporal y elevado margen de error humano en la revisión, limpieza, estandarización y mapeo manual de heterogéneos archivos de datos (CSV, JSON, XLSX) provenientes de múltiples fuentes con inconsistencias estructurales, nulos y duplicados.
- **Complejidad Técnica y Criticidad:**
  - *Complejidad:* Moderada o Alta debido a la integración con API de IA en tiempo real, procesamiento de archivos heterogéneos e ingeniería de pipelines de preparación (imputación con mediana, eliminación de nulos/duplicados).
  - *Criticidad:* Moderada. Errores en la limpieza pueden corromper la integridad del dataset original; se mitiga preservando el dataset original e implementando un flujo interactivo de confirmación humana antes del guardado/exportación.
  - *Atributos de Calidad:* Rendimiento, Usabilidad e Integridad de Datos (ISO/IEC 25010).
- **Perfil de Integrantes y Cliente:**
  - *Equipo de Desarrollo:* 3 estudiantes de Ingeniería en Datos e Inteligencia Artificial (7° cuatrimestre) con competencias intermedias en Python, análisis de datos, HTML/CSS e integración de APIs.
  - *Cliente / Product Owner:* Docente/Evaluador y rol interno representado por el PO en el backlog, exigiendo entregas incrementales verificables, criterios de aceptación en sintaxis Gherkin e hitos semanales/cuatrimestrales estructurados.

## 2. Evaluación Multicriterio de Alternativas Metodológicas

| Criterio de Evaluación | Enfoque Clásico (Cascada/Espiral) | Enfoque Ágil | Enfoque Híbrido Propuesto |
|---|---|---|---|
| Gestión de Cambios | Alta rigidez ante modificaciones. Requiere re-planificación formal previa. | Alta adaptabilidad e iteración rápida mediante backlog dinámico. | Balanza equilibrada: adaptabilidad ágil en Sprints de 1-2 semanas con control de riesgos estructurado del modelo Espiral. |
| Documentación Exigida | Formal y exhaustiva por etapa. | Mínima suficiente. | Documentación liviana pero estandarizada. |
| Participación del Cliente | Puntos fijos de revisión al inicio y final de las etapas principales. | Continua por Sprint mediante revisiones. | Retroalimentación frecuente al final de cada Sprint con participación del PO y validación con usuarios tipo analista/operador. |
| Velocidad de Entrega | Software operativo únicamente al final del ciclo de vida. | Incrementos funcionales cortos de software valioso y desplegable. | Entregas incrementales en Sprints cortos, priorizando el núcleo de ingesta y limpieza desde el Sprint 1. |

## 3. Justificación Fundada de la Metodología Seleccionada
- **Metodología Seleccionada:** Híbrido Scrum 
- **Argumentación Técnica Fundamentada:**
  La elección de un enfoque **Híbrido Scrum-XP** se fundamenta en los principios de Ian Sommerville (*Ingeniería de Software*, Cap. 2 - Procesos del Software), adaptados a los requerimientos de la asignatura y la naturaleza del proyecto:
  1. *Reducción del Riesgo y Costo de Cambio (Sommerville, Cap. 2):* Los proyectos de Inteligencia Artificial y canalizaciones de datos sufren fluctuaciones en la definición de esquemas y desempeño de los modelos. La estructura en **Sprints de Scrum** permite abordar la incertidumbre iterativamente, priorizando historias de mayor valor o riesgo (como la ingesta y preprocesamiento en el Sprint 1) sobre las secundarias (exportación PDF o Dashboards avanzados).
  2. *Ingeniería de Calidad con XP:* La integración de prácticas de **Extreme Programming (XP)** —tales como la revisión periódica de código entre pares (peer code review), refactorización continua y la exigencia de una *Definition of Done* (DoD) con análisis estático vía Linters— garantiza que la deuda técnica se mantenga en niveles mínimos.
  3. *Optimización de Tiempo y Recursos:* Al ser un equipo pequeño de 3 ingenieros con un margen de tiempo acotado, Scrum elimina la sobrecarga burocrática del modelo Cascada tradicional, mientras que XP previene errores críticos durante la integración con la API de IA mediante revisiones tempranas vía Pull Requests en GitHub.

## 4. Definición del Proceso Adaptado y Artefactos
- **Fases o Ciclos del Proceso:**
  - *Sprint 1 (Duración: 1-2 semanas):* Ingesta de archivos CSV/JSON/XLSX, canalización de limpieza y preprocesamiento de datos, y tablero base de métricas.
  - *Sprint 2 (Duración: 1-2 semanas):* Entrenamiento e inferencia del modelo de predicción, API REST para predicciones en tiempo real e integración del chat conversacional con IA.
  - *Sprint 3 / Cierre:* Refinamiento del dashboard, exportación de reportes PDF y preparación del cierre sumativo.
- **Artefactos Obligatorios a Generar:**
  - *Documentación Estructurada:* `CASO_ESTUDIO.md`, `HISTORIAS_USUARIOS.md`, `SPRINT_PLANNING.md`, `CICLO_VIDA.md`, `RIESGOS.md`, `REPORTE_METODOLOGIA.md`.
  - *Gestión y Código Fuente:* Product Backlog (Kanban Board), Pull Requests, Código Fuente en Python/HTML/CSS, Archivos de configuración de linters.
  - *Manuales y Entrega:* Manual de Usuario y Documentación de la API (Swagger/OpenAPI o Markdown).
- **Matriz de Responsabilidades de Equipo:**

| Integrante del Equipo | Rol Scrum/XP | Responsabilidades Clave |
|---|---|---|
| **Emmanuel Plata García** | Scrum Master / Dev Team | Facilitador del proceso, aseguramiento del DoR/DoD, desarrollo de ingesta de archivos CSV/JSON/XLSX. |
| **Oswaldo Guerrero García** | Product Owner / Dev Team | Priorización de backlog, definición de criterios Gherkin, desarrollo de módulos de limpieza, preprocesamiento y reglas de IA. |
| **Emmanuel Barrientos Delgado** | Lead Developer / QA / DevOps | Arquitectura de código, configuración de CI/Git, integración de API REST, tableros de métricas y pruebas del sistema. |

## 5. Compromiso de Calidad y Gobernanza de Código
- **Alineación con PARADIGMA.md y CALIDAD.md:**
  - *Suscripción a Git/GitHub:* Uso de ramificación tipo *Feature Branching* (ej. `feature/ingesta-csv`). Prohibido hacer commits directos a la rama principal (`main`).
  - *Estándares de Código y Linters:* Adherencia estricta a PEP 8 para Python (validado automáticamente mediante `flake8`/`black`) y validación HTML/CSS.
  - *Métricas ISO/IEC 25010:*
    - **Adecuación Funcional:** Cumplimiento estricto del $100\%$ de los criterios de aceptación en Gherkin definidos en `HISTORIAS_USUARIOS.md`.
    - **Eficiencia de Desempeño:** Tiempo de respuesta de API $< 500\text{ ms}$ y límites de procesamiento de archivos de $10\text{ MB}$.
    - **Mantenibilidad:** Cohesión alta, bajo acoplamiento y ausencia de errores críticos en linters.
- **Mecanismos de Control de Cambios:**
  - *Revisión de Código Obligatoria:* Ninguna Pull Request (PR) podrá fusionarse a `main` sin al menos un *approval* de revisión entre pares (peer review).
  - *Criterios para Fusionar (DoD Compliance):* La PR debe pasar las validaciones del linter, estar libre de conflictos de fusión y satisfacer los criterios de aceptación especificados en la Historia de Usuario correspondiente.