# Calcular y mostrar los factores primos de un número

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

## Proceso

1. Solicitar un número entero.
2. Leer el valor de n.
3. Buscar los divisores primos de n.
4. Almacenar cada factor primo en un arreglo.
5. Dividir el número por el factor encontrado.
6. Repetir el proceso hasta que el número sea 1.
7. Mostrar los factores primos almacenados.

## Salidas

| Salida                     |
| -------------------------- |
| Factores primos del número |

---

# Diseño de la Solución

## Secuencia lógica

1. Solicitar un número entero.
2. Leer el valor de n.
3. Crear un arreglo para almacenar los factores primos.
4. Inicializar el divisor en 2.
5. Verificar si el divisor divide exactamente al número.
6. Si divide exactamente, almacenar el divisor como factor primo.
7. Dividir el número por el divisor.
8. Repetir mientras el número siga siendo divisible.
9. Incrementar el divisor cuando ya no sea divisor exacto.
10. Continuar hasta que el número sea 1.
11. Mostrar los factores primos almacenados.
12. Finalizar el algoritmo.

---

## Variables utilizadas

| Variable   | Tipo    | Descripción                  |
| ---------- | ------- | ---------------------------- |
| n          | Entero  | Número ingresado             |
| divisor    | Entero  | Posible factor primo         |
| i          | Entero  | Índice del arreglo           |
| factores[] | Arreglo | Almacena los factores primos |

---

## Operadores utilizados

| Operador | Tipo       | Uso                      |
| -------- | ---------- | ------------------------ |
| =        | Asignación | Asignar valores          |
| %        | Aritmético | Verificar divisibilidad  |
| /        | Aritmético | Reducir el número        |
| ==       | Relacional | Comparar divisibilidad   |
| !=       | Relacional | Controlar ciclos         |
| ++       | Incremento | Avanzar divisor e índice |

---

## Estructuras utilizadas

| Estructura         | Uso                          |
| ------------------ | ---------------------------- |
| Secuencial         | Leer datos y asignar valores |
| Condicional (if)   | Verificar divisibilidad      |
| Repetitiva (while) | Buscar factores primos       |

---

## Fórmulas utilizadas

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

    Definir n, divisor, i Como Entero
    Definir factores[] Como Array

    Escribir "Ingrese un numero: "
    Leer n

    divisor = 2
    i = 0

    While n != 1

        If n % divisor == 0

            factores[i] = divisor

            i++

            n = n / divisor

        Else

            divisor++

        EndIf

    EndWhile

    Escribir "Factores primos: "

    For i = 0; i < cantidadFactores; i++

        Mostrar factores[i]

    EndFor

FIN
```

---

# Prueba de Escritorio

## Caso 1

### Datos de entrada

```text
n = 28
```

### Seguimiento

| n  | divisor | factor almacenado |
| -- | ------- | ----------------- |
| 28 | 2       | 2                 |
| 14 | 2       | 2                 |
| 7  | 7       | 7                 |
| 1  | -       | Fin               |

### Arreglo

```text
factores = [2, 2, 7]
```

### Resultado

```text
2, 2, 7
```

---

## Caso 2

### Datos de entrada

```text
n = 60
```

### Seguimiento

| n  | divisor | factor almacenado |
| -- | ------- | ----------------- |
| 60 | 2       | 2                 |
| 30 | 2       | 2                 |
| 15 | 3       | 3                 |
| 5  | 5       | 5                 |
| 1  | -       | Fin               |

### Arreglo

```text
factores = [2, 2, 3, 5]
```

### Resultado

```text
2, 2, 3, 5
```

---

# Implementación en C++

```cpp
#include <iostream>

using namespace std;

int main() {
    int n, divisor, i;

    cout << "Ingrese un numero: ";
    cin >> n;

    int factores[100];

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

    for (int j = 0; j < i; j++) {
        cout << factores[j] << " ";
    }

    cout << endl;

    return 0;
}
```
