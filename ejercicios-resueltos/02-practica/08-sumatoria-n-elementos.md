# Sumatoria de n términos de la serie

## Enunciado

Construir un algoritmo que realice la siguiente sumatoria de **n** elementos:

```text
Σ = 1 + (2*2) + (3*3*3) + (4*4*4*4) + (5*5*5*5*5) + ...
```

### Ejemplo

Si:

```text
n = 3
```

La sumatoria será:

```text
1 + (2*2) + (3*3*3)

1 + 4 + 27

Σ = 32
```

---

# Análisis del Problema

## Entradas

| Dato | Tipo   |
| ---- | ------ |
| n    | Entero |

## Proceso

1. Pedir la cantidad de términos.
2. Leer el valor de n.
3. Generar cada término de la sumatoria.
4. Calcular el valor de cada término.
5. Acumular los términos en una suma.
6. Mostrar el resultado final.

## Salidas

| Salida                    |
| ------------------------- |
| Resultado de la sumatoria |

---

# Diseño de la Solución

## Secuencia lógica

1. Solicitar la cantidad de términos.
2. Leer el valor de n.
3. Inicializar suma en 0.
4. Recorrer los términos desde 1 hasta n.
5. Inicializar aux en 1 para cada término.
6. Calcular el valor de i elevado a i mediante multiplicaciones sucesivas.
7. Acumular el resultado en suma.
8. Repetir el proceso para todos los términos.
9. Mostrar el resultado de la sumatoria.
10. Finalizar el algoritmo.

---

## Variables utilizadas

| Variable | Tipo   | Descripción                       |
| -------- | ------ | --------------------------------- |
| n        | Entero | Cantidad de términos              |
| i        | Entero | Control del ciclo principal       |
| j        | Entero | Control del ciclo interno         |
| aux      | Entero | Almacena el valor de cada término |
| suma     | Entero | Acumulador de la sumatoria        |

---

## Operadores utilizados

| Operador | Tipo       | Uso                |
| -------- | ---------- | ------------------ |
| =        | Asignación | Asignar valores    |
| *        | Aritmético | Calcular potencias |
| +        | Aritmético | Acumular la suma   |
| <        | Relacional | Controlar ciclos   |
| ++       | Incremento | Avanzar contadores |

---

## Estructuras utilizadas

| Estructura               | Uso                                |
| ------------------------ | ---------------------------------- |
| Secuencial               | Leer datos e inicializar variables |
| Repetitiva (for)         | Generar los términos               |
| Repetitiva anidada (for) | Calcular cada potencia             |

---

## Fórmulas utilizadas

### Cálculo de cada término

```text
aux = aux * i
```

### Acumulación de la sumatoria

```text
suma = suma + aux
```

---

# Pseudocódigo

```text
INICIO

    Definir n, i, j, aux, suma Como Entero

    Escribir "Ingrese la cantidad de terminos: "
    Leer n

    suma = 0

    For i = 1; i <= n; i++

        aux = 1

        For j = 1; j <= i; j++

            aux = aux * i

        EndFor

        suma = suma + aux

    EndFor

    Mostrar suma

FIN
```

---

# Prueba de Escritorio

## Caso 1

### Datos de entrada

```text
n = 3
```

### Seguimiento

| i | aux (i^i) | suma |
| - | --------- | ---- |
| 1 | 1         | 1    |
| 2 | 4         | 5    |
| 3 | 27        | 32   |

### Resultado

```text
Σ = 32
```

---

## Caso 2

### Datos de entrada

```text
n = 4
```

### Seguimiento

| i | aux (i^i) | suma |
| - | --------- | ---- |
| 1 | 1         | 1    |
| 2 | 4         | 5    |
| 3 | 27        | 32   |
| 4 | 256       | 288  |

### Resultado

```text
Σ = 288
```

---

# Implementación en C++

```cpp
#include <iostream>

using namespace std;

int main() {
    int n, i, j, aux, suma;

    cout << "Ingrese la cantidad de terminos: ";
    cin >> n;

    suma = 0;

    for (i = 1; i <= n; i++) {
        aux = 1;

        for (j = 1; j <= i; j++) {
            aux = aux * i;
        }

        suma = suma + aux;
    }

    cout << "Σ = " << suma << endl;

    return 0;
}
```
