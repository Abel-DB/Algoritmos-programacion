# Macros

---

## ¿Qué es una macro?

Una **macro** es una instrucción que permite definir un valor o expresión que será **reemplazado automáticamente** antes de la compilación de un programa.

No se ejecuta como una instrucción normal, sino que actúa como una **sustitución de texto**.

---

## Idea clave

Una macro funciona como un **reemplazo automático** que ocurre antes de que el programa sea procesado.

---

## ¿Dónde se utilizan?

Las macros se utilizan en la etapa de:

**Preprocesamiento**

Flujo general:

Código → Preprocesamiento → Compilación → Ejecución

---

## Tipos de macros

---

### 1. Macros constantes

Definen valores fijos que pueden reutilizarse.

Ejemplos conceptuales:

* PI → 3.1416
* MAX → 100

---

### 2. Macros con parámetros

Permiten definir expresiones que reciben valores.

Ejemplo conceptual:

* SUMA(a, b) → a + b

---

## Características

* Se expanden antes de la compilación
* No tienen tipo de dato
* No realizan validaciones
* Son sustituciones directas de texto

---

## Ventajas

* Evitan la repetición de valores
* Facilitan cambios globales
* Simplifican expresiones
* Mejoran la organización

---

## Desventajas

* No validan tipos de datos
* Pueden generar errores difíciles de detectar
* No respetan siempre la prioridad de operaciones
* Pueden reducir la claridad si se usan en exceso

---

## Diferencia con funciones

| Macro                | Función           |
| -------------------- | ----------------- |
| Sustitución de texto | Código ejecutable |
| No valida tipos      | Sí valida         |
| Más rápida           | Más segura        |
| Menos control        | Más control       |

---

## Buenas prácticas

* Usarlas principalmente para constantes
* Escribir sus nombres en mayúsculas
* Utilizar paréntesis en expresiones
* Evitar macros complejas

---

## Conceptos relacionados

### Preprocesador

Es el encargado de transformar el código antes de compilarlo.

---

### Sustitución textual

Proceso en el cual el contenido de la macro reemplaza directamente al texto original.

---

### Expansión de macros

Es el proceso mediante el cual se realiza el reemplazo automático.

---

## Errores comunes

* No usar paréntesis en expresiones
* Usar macros como si fueran funciones complejas
* Confundir macros con variables
* No considerar el proceso de preprocesamiento

---

## Conclusión

Las macros permiten simplificar y organizar el código mediante reemplazos automáticos, pero deben utilizarse con cuidado debido a sus limitaciones.

---

## Resumen

* Son reemplazos automáticos de texto
* Se aplican antes de la compilación
* No son funciones reales
* Son útiles principalmente para constantes

---
