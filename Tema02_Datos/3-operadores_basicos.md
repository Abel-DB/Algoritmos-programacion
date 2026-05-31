# Operadores Básicos

## ¿Qué es un operador?

Un **operador** es un símbolo que permite realizar una operación sobre uno o más operandos (datos o variables) para obtener un resultado.

### Ejemplo

```cpp
int suma = 5 + 3;
```

En este caso:

* `5` y `3` son operandos.
* `+` es el operador.
* `8` es el resultado.

---

# Importancia

Los operadores permiten:

* Realizar cálculos.
* Comparar valores.
* Evaluar condiciones.
* Modificar variables.
* Construir expresiones complejas.

Son fundamentales para el desarrollo de algoritmos y programas.

---

# Clasificación de operadores

| Tipo                    | Función                            |
| ----------------------- | ---------------------------------- |
| Aritméticos             | Realizan operaciones matemáticas.  |
| Relacionales            | Comparan valores.                  |
| Lógicos                 | Combinan condiciones.              |
| Asignación              | Asignan valores a variables.       |
| Incremento y decremento | Modifican variables en una unidad. |

---

# Operadores aritméticos

Se utilizan para realizar operaciones matemáticas.

| Operador | Descripción    | Ejemplo |
| -------- | -------------- | ------- |
| +        | Suma           | a + b   |
| -        | Resta          | a - b   |
| *        | Multiplicación | a * b   |
| /        | División       | a / b   |
| %        | Módulo (resto) | a % b   |

---

## Ejemplo

```cpp
int a = 10;
int b = 3;

cout << a + b << endl; // 13
cout << a - b << endl; // 7
cout << a * b << endl; // 30
cout << a / b << endl; // 3
cout << a % b << endl; // 1
```

---

# Operadores de asignación

Permiten almacenar valores en variables.

| Operador | Descripción         | Ejemplo |
| -------- | ------------------- | ------- |
| =        | Asignación simple   | a = 5   |
| +=       | Suma y asigna       | a += 2  |
| -=       | Resta y asigna      | a -= 2  |
| *=       | Multiplica y asigna | a *= 2  |
| /=       | Divide y asigna     | a /= 2  |
| %=       | Módulo y asigna     | a %= 2  |

---

## Ejemplo

```cpp
int numero = 10;

numero += 5; // 15
numero -= 2; // 13
numero *= 2; // 26
```

---

# Operadores relacionales

Comparan dos valores y devuelven un resultado lógico.

| Operador | Significado       |
| -------- | ----------------- |
| ==       | Igual a           |
| !=       | Distinto de       |
| >        | Mayor que         |
| <        | Menor que         |
| >=       | Mayor o igual que |
| <=       | Menor o igual que |

---

## Ejemplo

```cpp
int a = 10;
int b = 20;

cout << (a < b) << endl;
cout << (a == b) << endl;
```

---

# Operadores lógicos

Permiten combinar expresiones lógicas.

| Operador | Significado |
| -------- | ----------- |
| &&       | AND (Y)     |
| ||       | OR (O)      |
| !        | NOT (NO)    |

---

## Ejemplo

```cpp
int edad = 20;
bool estudiante = true;

cout << (edad >= 18 && estudiante);
```

---

# Operadores de incremento y decremento

Permiten aumentar o disminuir una unidad.

| Operador | Descripción     |
| -------- | --------------- |
| ++       | Incrementa en 1 |
| --       | Decrementa en 1 |

---

## Ejemplo

```cpp
int contador = 5;

contador++;
contador--;

cout << contador;
```

---

# Precedencia de operadores

Cuando una expresión contiene varios operadores, algunos se ejecutan antes que otros.

| Prioridad | Operadores             |
| --------- | ---------------------- |
| Alta      | (), ++, --             |
| Media     | *, /, %                |
| Baja      | +, -                   |
| Muy baja  | Relacionales y lógicos |

---

## Ejemplo

```cpp
int resultado = 5 + 3 * 2;
```

Primero:

```text
3 * 2 = 6
```

Luego:

```text
5 + 6 = 11
```

Resultado:

```text
11
```

---

# Aplicaciones

Los operadores se utilizan en:

* Cálculos matemáticos.
* Validación de datos.
* Toma de decisiones.
* Control de flujo.
* Manipulación de variables.

---

# Errores comunes

| Error                                | Descripción                              |
| ------------------------------------ | ---------------------------------------- |
| Confundir `=` con `==`               | Asignación y comparación son diferentes. |
| División entre enteros               | Puede perder decimales.                  |
| Olvidar la precedencia               | Produce resultados inesperados.          |
| Uso incorrecto de operadores lógicos | Condiciones erróneas.                    |

---

# Información complementaria

Los operadores relacionales y lógicos serán utilizados ampliamente en:

- [Instrucciones de control](../Tema05_instrucciones_control/)

---

# Conclusión

Los operadores permiten realizar cálculos, comparaciones y evaluaciones lógicas dentro de un programa. Su correcta utilización es esencial para desarrollar soluciones eficientes y resolver problemas de forma adecuada.

---

# Resumen

| Concepto                | Idea principal                     |
| ----------------------- | ---------------------------------- |
| Aritméticos             | Operaciones matemáticas.           |
| Asignación              | Almacenamiento de valores.         |
| Relacionales            | Comparación de datos.              |
| Lógicos                 | Combinación de condiciones.        |
| Incremento y decremento | Modificación de variables.         |
| Importancia             | Base de la lógica de programación. |
