# Factores Primos de un Número

## Enunciado

Construir un algoritmo que pida al usuario un número entero **n**, calcular, almacenar en un arreglo y mostrar sus factores primos.

### Ejemplo

Si:

```text
n = 28
```

Mostrar:

```text
2, 2, 7
```

Porque:

```text
28 = 2 × 2 × 7
```

---

# Análisis del Problema

## Entradas

| Dato | Tipo   |
| ---- | ------ |
| n    | Entero |

---

## Proceso

1. Solicitar un número entero.
2. Leer el valor de n.
3. Crear un arreglo para almacenar los factores primos.
4. Inicializar el divisor en 2.
5. Inicializar el índice del arreglo en 0.
6. Verificar si el divisor divide exactamente al número.
7. Si divide exactamente, almacenar el divisor como factor primo.
8. Dividir el número por el divisor.
9. Si no divide exactamente, incrementar el divisor.
10. Continuar el proceso hasta que el número sea 1.
11. Recorrer el arreglo de factores primos.
12. Mostrar los factores almacenados.
13. Finalizar el algoritmo.

---

## Salidas

| Salida                     |
| -------------------------- |
| Factores primos del número |

---

# Variables Utilizadas

| Variable   | Tipo   | Descripción                    |
| ---------- | ------ | ------------------------------ |
| n          | Entero | Número ingresado               |
| divisor    | Entero | Posible factor primo           |
| i          | Entero | Índice del arreglo             |
| j          | Entero | Índice para mostrar el arreglo |
| factores[] | Array  | Almacena los factores primos   |

---

# Operadores Utilizados

| Operador | Tipo       | Uso                       |
| -------- | ---------- | ------------------------- |
| =        | Asignación | Asignar valores           |
| %        | Aritmético | Verificar divisibilidad   |
| /        | Aritmético | Reducir el número         |
| ==       | Relacional | Comparar divisibilidad    |
| !=       | Relacional | Controlar el while        |
| <        | Relacional | Controlar el for          |
| ++       | Incremento | Avanzar índices y divisor |

---

# Estructuras Utilizadas

| Estructura         | Uso                              |
| ------------------ | -------------------------------- |
| Secuencial         | Lectura y asignaciones           |
| Condicional (if)   | Verificar divisibilidad          |
| Repetitiva (while) | Buscar factores primos           |
| Repetitiva (for)   | Mostrar los factores almacenados |

---

# Fórmulas Utilizadas

### Verificación de divisibilidad

```text
n % divisor == 0
```

### Reducción del número

```text
n = n / divisor
```

---

# Pseudocódigo

```text
INICIO

    Definir n, divisor, i, j Como Entero
    Definir factores[] Como Array

    Escribir "Ingrese un numero: "
    Leer n

    divisor = 2
    i = 0

    While (n != 1)

        If (n % divisor == 0) Then

            factores[i] = divisor

            i++

            n = n / divisor

        Else

            divisor++

        EndIf

    EndWhile

    Mostrar "Factores primos: "

    For (j = 0; j < i; j++)

        Mostrar factores[j]

    EndFor

FIN
```

---

# Prueba de Escritorio

## Caso 1

### Datos de entrada

```text
n = 12
```

### Seguimiento

| Vuelta | n  | divisor | n % divisor | factores[i] | i | Acción           |
| ------ | -- | ------- | ----------- | ----------- | - | ---------------- |
| 1      | 12 | 2       | 0           | 2           | 1 | Guarda 2 y n = 6 |
| 2      | 6  | 2       | 0           | 2           | 2 | Guarda 2 y n = 3 |
| 3      | 3  | 2       | 1           | -           | 2 | divisor = 3      |
| 4      | 3  | 3       | 0           | 3           | 3 | Guarda 3 y n = 1 |

> Al finalizar:

```text
factores = [2, 2, 3]
i = 3
n = 1
```

### Resultado

```text
2, 2, 3
```

---

## Caso 2

### Datos de entrada

```text
n = 18
```

### Seguimiento

| Vuelta | n  | divisor | n % divisor | factores[i] | i | Acción           |
| ------ | -- | ------- | ----------- | ----------- | - | ---------------- |
| 1      | 18 | 2       | 0           | 2           | 1 | Guarda 2 y n = 9 |
| 2      | 9  | 2       | 1           | -           | 1 | divisor = 3      |
| 3      | 9  | 3       | 0           | 3           | 2 | Guarda 3 y n = 3 |
| 4      | 3  | 3       | 0           | 3           | 3 | Guarda 3 y n = 1 |

> Al finalizar:

```text
factores = [2, 3, 3]
i = 3
n = 1
```

### Resultado

```text
2, 3, 3
```

---

# Implementación en C++

```cpp
#include <iostream>

using namespace std;

int main() {
    int n, divisor, i, j;

    cout << "Ingrese un numero: ";
    cin >> n;

    int factores[n];

    divisor = 2;
    i = 0;

    while (n != 1) {

        if (n % divisor == 0) {

            factores[i] = divisor;
            i++;

            n = n / divisor;

        } else {

            divisor++;
        }
    }

    cout << "Factores primos: ";

    for (j = 0; j < i; j++) {
        cout << factores[j] << ", ";
    }

    cout << endl;

    return 0;
}
```
