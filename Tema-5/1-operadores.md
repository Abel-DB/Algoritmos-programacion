# Operadores Basicos

---

## ¿Qué es un operador?

Un **operador** es un símbolo que indica una operación sobre uno o más valores (operandos).
Se utiliza para **realizar cálculos, comparaciones o decisiones**.

---

## Tipos de operadores

### 1. Operadores aritméticos

| Operador | Significado    | Ejemplo       |
| -------- | -------------- | ------------- |
| +        | Suma           | A + B         |
| -        | Resta          | A - B         |
| *        | Multiplicación | A * B         |
| /        | División       | A / B         |
| %        | Módulo         | A % B (resto) |

---

### 2. Operadores de comparacion - relacionales

| Operador | Significado   | Ejemplo |
| -------- | ------------- | ------- |
| ==       | Igual a       | A == B  |
| !=       | Distinto de   | A != B  |
| >        | Mayor que     | A > B   |
| <        | Menor que     | A < B   |
| >=       | Mayor o igual | A >= B  |
| <=       | Menor o igual | A <= B  |

---

### 3. Operadores lógicos

| Operador | Significado | Ejemplo        |
| -------- | ----------- | -------------- |
| &&       | Y lógico    | (A > 0 && B>0) |
| ||       | O lógico    | (A > 0 || B>0) |
| !        | Negación    | !(A == B)      |

---

### 4. Operadores de asignación - abreviados

| Operador | Significado    | Ejemplo            |
| -------- | -------------- | ------------------ |
|  =       | asignación     | A = 5              |
| +=       | Suma y asigna  | A += 5 → A = A + 5 |
| -=       | Resta y asigna | A -= 3 → A = A - 3 |
| *=       | Multiplica     | A *= 2 → A = A * 2 |
| /=       | Divide         | A /= 4 → A = A / 4 |
| %=       | Módulo         | A %= 2 → A = A % 2 |

---

## Ejemplo lógico con operadores

**Problema:** Sumar dos números y verificar si el resultado es mayor que 10

### Algoritmo

1. Leer A
2. Leer B
3. Suma = A + B
4. Si Suma > 10 → mostrar "Mayor que 10"
5. Sino → mostrar "10 o menor"

---

### Diagrama de flujo con símbolos

* **Óvalo:** Inicio/Fin
* **Paralelogramo:** Entrada/Salida
* **Rectángulo:** Proceso
* **Rombo:** Decisión

```text id="9t2xq5"
   ┌───────────┐       ← Óvalo (INICIO)
   │  INICIO   │
   └─────┬─────┘
         │
   ┌───────────────┐    ← Paralelogramo (Entrada)
   │ Leer A, B     │
   └─────┬─────────┘
         │
   ┌───────────────┐    ← Rectángulo (Proceso)
   │ Suma = A + B  │
   └─────┬─────────┘
         │
   ┌────────────────────────┐  ← Rombo (Decisión)
   │ Suma > 10?             │
   └─────┬───────────┬─────┘
       Sí│           │No
         │           │
 ┌───────────────┐ ┌───────────────┐
 │ Mostrar "Mayor"│ │ Mostrar "10 o ≤"│
 │ (Paralelogramo)│ │ (Paralelogramo)│
 └─────┬─────────┘ └─────┬─────────┘
       │                 │
       └───────┬─────────┘
               │
           ┌───────────┐    ← Óvalo (FIN)
           │   FIN     │
           └───────────┘
```

---

## Prueba de escritorio

Supongamos:

* A = 6
* B = 5

| Paso    | A | B | Suma | Condición    | Salida         |
| ------- | - | - | ---- | ------------ | -------------- |
| Leer A  | 6 | - | -    | -            | -              |
| Leer B  | 6 | 5 | -    | -            | -              |
| Proceso | 6 | 5 | 11   | 11 > 10 = Sí | -              |
| Mostrar | 6 | 5 | 11   | Sí           | "Mayor que 10" |

---

## Resumen

* Los operadores permiten **cálculos, comparaciones y decisiones**

* Diagramas y prueba de escritorio ayudan a **verificar la lógica antes de programar**

---
