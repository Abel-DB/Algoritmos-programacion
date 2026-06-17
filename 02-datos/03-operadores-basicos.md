# Operadores Básicos

## ¿Qué es un operador?

Un **operador** es un símbolo que permite realizar una operación sobre uno o más operandos para obtener un resultado.

### Ejemplo conceptual

```text
5 + 3 = 8
```

En este caso:

* 5 y 3 son operandos.
* * es el operador.
* 8 es el resultado.

---

# Importancia

Los operadores permiten:

* Realizar cálculos.
* Comparar valores.
* Evaluar condiciones.
* Asignar resultados.
* Construir expresiones complejas.

Son fundamentales para el desarrollo de algoritmos y la resolución de problemas.

---

# Clasificación de operadores

| Tipo         | Función                            |
| ------------ | ---------------------------------- |
| Aritméticos  | Realizan operaciones matemáticas.  |
| Relacionales | Comparan valores.                  |
| Lógicos      | Combinan condiciones.              |
| Asignación   | Almacenan resultados en variables. |

---

# Operadores aritméticos

Se utilizan para realizar operaciones matemáticas.

| Operador | Descripción      |
| -------- | ---------------- |
| +        | Suma             |
| -        | Resta            |
| *        | Multiplicación   |
| /        | División         |
| %        | Módulo o residuo |

---

## Ejemplos

| Expresión | Resultado |
| --------- | --------- |
| 5 + 3     | 8         |
| 10 - 4    | 6         |
| 6 × 2     | 12        |
| 8 ÷ 2     | 4         |
| 10 % 3    | 1         |

---

# Operadores de asignación

Permiten almacenar valores en variables.

## Asignación simple

```text
edad ← 20
```

La variable recibe el valor indicado.

---

## Ejemplo

```text
total ← 150
promedio ← 85.5
nombre ← "Juan"
```

---

# Operadores relacionales

Permiten comparar dos valores.

El resultado de una comparación es un valor lógico:

```text
Verdadero
Falso
```

---

| Operador | Significado       |
| -------- | ----------------- |
| ==       | Igual a           |
| ≠        | Diferente de      |
| >        | Mayor que         |
| <        | Menor que         |
| ≥        | Mayor o igual que |
| ≤        | Menor o igual que |

---

## Ejemplos

| Expresión | Resultado |
| --------- | --------- |
| 10 > 5    | Verdadero |
| 7 < 3     | Falso     |
| 8 = 8     | Verdadero |
| 4 ≠ 4     | Falso     |

---

# Operadores lógicos

Permiten combinar condiciones.

---

## Operador AND (Y)

El resultado es verdadero únicamente cuando todas las condiciones son verdaderas.

| A | B | A Y B |
| - | - | ----- |
| V | V | V     |
| V | F | F     |
| F | V | F     |
| F | F | F     |

---

## Operador OR (O)

El resultado es verdadero cuando al menos una condición es verdadera.

| A | B | A O B |
| - | - | ----- |
| V | V | V     |
| V | F | V     |
| F | V | V     |
| F | F | F     |

---

## Operador NOT (NO)

Invierte el valor lógico.

| A | NO A |
| - | ---- |
| V | F    |
| F | V    |

---

# Precedencia de operadores

Cuando una expresión contiene varios operadores, algunos se ejecutan antes que otros.

## Prioridad general

1. Paréntesis.
2. Multiplicación, división y módulo.
3. Suma y resta.
4. Operadores relacionales.
5. Operadores lógicos.

---

## Ejemplo

```text
5 + 3 × 2
```

Primero:

```text
3 × 2 = 6
```

Después:

```text
5 + 6 = 11
```

Resultado final:

```text
11
```

---

# Aplicaciones

Los operadores se utilizan en:

* Cálculos matemáticos.
* Procesamiento de información.
* Validación de datos.
* Comparación de valores.
* Toma de decisiones.
* Resolución de problemas.

---

# Errores comunes

| Error                                | Descripción                     |
| ------------------------------------ | ------------------------------- |
| Ignorar la precedencia               | Produce resultados incorrectos. |
| Utilizar operadores inadecuados      | Genera soluciones erróneas.     |
| Confundir asignación con comparación | Produce errores lógicos.        |
| Combinar incorrectamente condiciones | Resultados inesperados.         |

---

# Conclusión

Los operadores permiten manipular datos, realizar cálculos y evaluar condiciones dentro de un algoritmo. Su correcta utilización constituye una base fundamental para la construcción de soluciones eficientes.

---

# Resumen

| Concepto     | Idea principal                                            |
| ------------ | --------------------------------------------------------- |
| Aritméticos  | Realizan operaciones matemáticas.                         |
| Asignación   | Almacenan valores en variables.                           |
| Relacionales | Comparan información.                                     |
| Lógicos      | Combinan condiciones.                                     |
| Precedencia  | Define el orden de evaluación.                            |
| Importancia  | Base para la resolución de problemas mediante algoritmos. |
