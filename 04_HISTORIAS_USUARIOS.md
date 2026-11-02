
# Inventario de Historias de Usuario

**Proyecto:** DataDoc: Plataforma de Procesamiento, Estandarización y Análisis de Datos.  
**Asignatura:** Ingeniería de Software.  


## Integrantes del equipo

| Matrícula | Integrante |
|---|---|
| 24031062 | Oswaldo Guerrero García |
| 24030202 | Emmanuel Barrientos Delgado |
| 24031042 | Emmanuel Plata García |

---

# Actividades asignadas

## Usuario: Oswaldo Guerrero García

**ID del usuario:** 24031062

### Actividad: Procesar y revisar los datos

- **Como:** Usuario del sistema.
- **Quiero:** Conocer cómo está organizado mi archivo.
- **Para:** Saber cuántas filas y columnas tiene y qué tipo de información contiene.
- **Puntos:** 5.
- **Prioridad:** Alta.

#### Criterios de aceptación

**Escenario 1: Revisión de los datos**

- **Dado que** el usuario ya cargó un archivo.
- **Cuando** el sistema lo procesa.
- **Entonces** debe mostrar la cantidad de filas, columnas y los tipos de datos que contiene.

**Escenario 2: Archivo sin información**

- **Dado que** el usuario carga un archivo vacío.
- **Cuando** el sistema intenta revisarlo.
- **Entonces** debe mostrar un mensaje indicando que no hay datos para analizar.

### Actividad: Crear un resumen de los datos

- **Como:** Usuario del sistema.
- **Quiero:** Obtener un resumen general de la información de mi archivo.
- **Para:** Comprender de manera rápida qué datos contiene y cuáles podrían ser importantes.
- **Puntos:** 5.
- **Prioridad:** Alta.

#### Criterios de aceptación

**Escenario 1: Mostrar un resumen**

- **Dado que** el sistema ya procesó un archivo.
- **Cuando** el usuario solicita ver el resumen.
- **Entonces** el sistema debe mostrar información general sobre los datos.

**Escenario 2: Mostrar información importante**

- **Dado que** el archivo contiene diferentes tipos de información.
- **Cuando** el sistema realiza el análisis.
- **Entonces** debe mostrar observaciones sobre los datos que podrían ser importantes para el usuario.

### Actividad: Descargar los resultados

- **Como:** Usuario del sistema.
- **Quiero:** Descargar los resultados del análisis.
- **Para:** Guardar la información y poder consultarla después.
- **Puntos:** 3.
- **Prioridad:** Baja.

#### Criterios de aceptación

**Escenario 1: Descarga de resultados**

- **Dado que** el sistema ya terminó de analizar un archivo.
- **Cuando** el usuario solicita descargar los resultados.
- **Entonces** el sistema debe generar un archivo con el resumen y las estadísticas disponibles.

**Escenario 2: No hay resultados para descargar**

- **Dado que** el usuario todavía no ha realizado ningún análisis.
- **Cuando** intenta descargar los resultados.
- **Entonces** el sistema debe mostrar un mensaje indicando que primero debe analizar un archivo.

---

## Usuario: Emmanuel Barrientos Delgado

**ID del usuario:** 24030202

### Actividad: Obtener estadísticas y detectar problemas

- **Como:** Usuario del sistema.
- **Quiero:** Obtener estadísticas y encontrar datos faltantes o repetidos.
- **Para:** Conocer mejor la información y detectar posibles problemas en el archivo.
- **Puntos:** 8.
- **Prioridad:** Alta.

#### Criterios de aceptación

**Escenario 1: Análisis de los datos**

- **Dado que** el usuario cargó un archivo con información.
- **Cuando** solicita analizarlo.
- **Entonces** el sistema debe mostrar estadísticas básicas y revisar si existen datos faltantes o repetidos.

**Escenario 2: Encontrar problemas**

- **Dado que** el archivo contiene datos faltantes o repetidos.
- **Cuando** el sistema realiza el análisis.
- **Entonces** debe indicar cuántos problemas encontró y dónde se encuentran, cuando sea posible.

### Actividad: Limpiar y organizar los datos de forma opcional

- **Como:** Usuario del sistema.
- **Quiero:** Elegir qué datos deseo limpiar o corregir.
- **Para:** Mejorar la información de mi archivo sin modificar el original automáticamente.
- **Puntos:** 8.
- **Prioridad:** Media.

#### Criterios de aceptación

**Escenario 1: El usuario desea limpiar los datos**

- **Dado que** el archivo contiene datos faltantes o repetidos.
- **Cuando** el usuario selecciona una opción de limpieza y confirma.
- **Entonces** el sistema debe realizar los cambios seleccionados y mostrar qué se modificó.

**Escenario 2: El usuario no desea limpiar los datos**

- **Dado que** el usuario ya cargó y analizó un archivo.
- **Cuando** decide no utilizar la limpieza.
- **Entonces** el sistema debe conservar los datos originales sin realizar cambios.

---

## Usuario: Emmanuel Plata García

**ID del usuario:** 24031042

### Actividad: Cargar archivos CSV y Excel

- **Como:** Usuario del sistema.
- **Quiero:** Cargar archivos CSV y Excel.
- **Para:** Poder analizar la información que contienen.
- **Puntos:** 5.
- **Prioridad:** Alta.

#### Criterios de aceptación

**Escenario 1: Archivo cargado correctamente**

- **Dado que** el usuario tiene un archivo CSV o Excel.
- **Cuando** lo selecciona y lo carga.
- **Entonces** el sistema debe leerlo y mostrar su contenido.

**Escenario 2: Archivo no permitido**

- **Dado que** el usuario selecciona un archivo de otro formato.
- **Cuando** intenta cargarlo.
- **Entonces** el sistema debe mostrar un mensaje indicando que no se puede utilizar ese archivo.

### Actividad: Mostrar los resultados del análisis

- **Como:** Usuario del sistema.
- **Quiero:** Ver los resultados del análisis en una interfaz sencilla.
- **Para:** Comprender fácilmente las estadísticas y los problemas encontrados.
- **Puntos:** 5.
- **Prioridad:** Alta.

#### Criterios de aceptación

**Escenario 1: Mostrar los resultados**

- **Dado que** el sistema terminó de analizar un archivo.
- **Cuando** el usuario entra a la sección de resultados.
- **Entonces** debe mostrar el resumen, las estadísticas y los problemas encontrados.

**Escenario 2: Todavía no hay resultados**

- **Dado que** el usuario aún no ha cargado ni analizado un archivo.
- **Cuando** entra a la sección de resultados.
- **Entonces** el sistema debe indicar que primero necesita cargar y analizar un archivo.

---

## Resumen de actividades

| ID del usuario | Integrante | Actividades asignadas |
|---|---|---|
| 24031062 | Oswaldo Guerrero García | Procesar y revisar los datos, crear un resumen y descargar los resultados. |
| 24030202 | Emmanuel Barrientos Delgado | Obtener estadísticas, detectar problemas y realizar la limpieza opcional. |
| 24031042 | Emmanuel Plata García | Cargar archivos CSV y Excel y mostrar los resultados del análisis. |
