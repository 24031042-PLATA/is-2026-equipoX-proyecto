# MATRIZ DE ATRIBUTOS DE CALIDAD

## 1. Mantenibilidad

**Objetivo**
El código deberá ser claro, modular y fácil de modificar.

**Estándares**
- PEP8
- Variables en snake_case
- Máximo 15 líneas por función cuando sea posible
---

## 2. Confiabilidad y Seguridad

**Objetivo**
Evitar errores y proteger la información del proyecto.

**Acciones**
- Validar entradas
- Utilizar bloques try-except
- No subir contraseñas ni tokens al repositorio
---

## 3. Eficiencia

**Objetivo**
Utilizar correctamente la memoria y reducir tiempos de respuesta.

**Acciones**
- Evitar procesos repetitivos
- Utilizar listas y diccionarios de forma adecuada
---

## 4. Aceptabilidad

**Objetivo**
El sistema debe ser fácil de comprender y utilizar.

**Acciones**
- Documentar funciones
- Mantener una interfaz sencilla
- Utilizar nombres descriptivos

flake8 . --max-line-length=100 --statistics