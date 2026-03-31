# Variables y Tipos de Datos

---

## ¿Qué es una variable?

Una **variable** es un espacio en memoria que se utiliza para almacenar datos.

* Su valor puede cambiar durante la ejecución del programa.
* Cada variable tiene un **nombre**, un **tipo** y un **valor**.

---

## Cómo nombrar variables correctamente

Reglas generales:

1. Debe **comenzar con letra o guion bajo** (`_`)
2. No puede contener espacios
3. Evitar nombres reservados por el lenguaje (ej: `int`, `float`)
4. Debe ser **descriptiva**: indicar lo que almacena

   * Ej: `edad`, `suma_total`, `nombre_usuario`

Buenas prácticas:

* Usar **camelCase**: `numeroIngresado`
* Usar **snake_case**: `numero_ingresado`
* Evitar abreviaturas confusas

---

## Tipos de datos

Los tipos de datos indican **qué clase de información** puede almacenar una variable.
Se dividen en **enteros, reales, caracteres, cadenas y booleanos**.

---

### Tipos de datos enteros

| Tipo        | Tamaño aproximado | Rango típico                   | Uso principal       |
| ----------- | ----------------- | ------------------------------ | ------------------- |
| `byte`      | 1 byte            | 0 a 255                        | Pequeños números    |
| `short`     | 2 bytes           | -32,768 a 32,767               | Números pequeños    |
| `int`       | 4 bytes           | -2,147,483,648 a 2,147,483,647 | Números medios      |
| `long`      | 8 bytes           | Muy grande                     | Números grandes     |
| `long long` | 8 bytes           | Más grande que long            | Números muy grandes |

> Nota: Los rangos pueden variar según el lenguaje o compilador.

---

### Tipos de datos reales

| Tipo          | Tamaño aproximado | Precisión             | Uso principal           |
| ------------- | ----------------- | --------------------- | ----------------------- |
| `float`       | 4 bytes           | ~7 dígitos decimales  | Números con decimales   |
| `double`      | 8 bytes           | ~15 dígitos decimales | Mayor precisión         |
| `long double` | 12-16 bytes       | Muy alta precisión    | Científico / financiero |

---

### Otros tipos

| Tipo     | Descripción          | Ejemplo       |
| -------- | -------------------- | ------------- |
| `char`   | Un solo carácter     | 'A', 'b', '1' |
| `string` | Cadena de caracteres | "Hola mundo"  |
| `bool`   | Verdadero o falso    | true, false   |

---

## Uso de variables en un algoritmo

**Problema:** Sumar dos números

---

### Algoritmo

1. Leer número A (`int`)
2. Leer número B (`int`)
3. Suma = A + B
4. Mostrar Suma

---

### Diagrama de flujo

```text id="d4k7xq"
   ┌───────────┐
   │  INICIO   │
   └─────┬─────┘
         │
   ┌───────────────┐
   │ Leer A, B     │  ← Entrada (paralelogramo)
   └─────┬─────────┘
         │
   ┌───────────────┐
   │ Suma = A + B  │  ← Proceso (rectángulo)
   └─────┬─────────┘
         │
   ┌──────────────────┐
   │ Mostrar Suma     │  ← Salida (documento)
   └─────┬────────────┘
         │
   ┌───────────┐
   │   FIN     │
   └───────────┘
```

---

## Prueba de escritorio

Supongamos que:

* A = 123 (`int`)
* B = 77 (`int`)

| Paso    | A   | B  | Suma |
| ------- | --- | -- | ---- |
| Leer A  | 123 | -  | -    |
| Leer B  | 123 | 77 | -    |
| Proceso | 123 | 77 | 200  |
| Mostrar | 123 | 77 | 200  |

---

## Reglas importantes

* No mezclar tipos sin conversión (ej: sumar `int` + `string`)
* Elegir el tipo adecuado según el rango de valores esperado
* Nombrar variables de forma clara y consistente

---

## Resumen

* Una variable almacena datos y tiene **nombre, tipo y valor**
* Tipos de datos **enteros**: byte, short, int, long, long long
* Tipos de datos **reales**: float, double, long double
* Otros tipos: char, string, bool
* Nombrar variables correctamente evita errores y hace el código más legible
* La prueba de escritorio permite verificar la lógica antes de programar

---
