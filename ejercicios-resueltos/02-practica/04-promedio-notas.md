# Calcular el promedio de n notas

## Enunciado

Construir un algoritmo que pida al usuario **n** notas de estudiantes, las notas deberán ser guardadas en un arreglo (array), calcular y mostrar el promedio de las mismas.

### Ejemplo

Si:

```text
n = 5
```

Ingresar:

```text
70
90
51
80
30
```

Mostrar:

```text
El promedio es: 64.2
```

---

# Análisis del Problema

## Entradas

| Dato    | Tipo               |
| ------- | ------------------ |
| n       | Entero             |
| notas[] | Arreglo de enteros |

## Proceso

1. Pedir la cantidad de notas.
2. Almacenar las notas en un arreglo.
3. Sumar todas las notas.
4. Dividir la suma entre la cantidad de notas.
5. Mostrar el promedio.

## Salidas

| Salida                |
| --------------------- |
| Promedio de las notas |

---

# Diseño de la Solución

## Secuencia lógica

1. Solicitar la cantidad de notas.
2. Leer el valor de n.
3. Crear un arreglo para almacenar las notas.
4. Inicializar la variable suma en 0.
5. Ingresar las n notas y almacenarlas en el arreglo.
6. Recorrer el arreglo sumando todas las notas.
7. Calcular el promedio dividiendo la suma entre n.
8. Mostrar el promedio obtenido.
9. Finalizar el algoritmo.

---

## Variables utilizadas

| Variable | Tipo    | Descripción                   |
| -------- | ------- | ----------------------------- |
| n        | Entero  | Cantidad de notas             |
| i        | Entero  | Control del ciclo             |
| aux      | Entero  | Nota ingresada temporalmente  |
| suma     | Real    | Acumulador de las notas       |
| promedio | Real    | Promedio calculado            |
| notas[]  | Arreglo | Almacena las notas ingresadas |

---

## Operadores utilizados

| Operador | Tipo                 | Uso                |
| -------- | -------------------- | ------------------ |
| =        | Asignación           | Asignar valores    |
| +        | Aritmético           | Sumar notas        |
| +=       | Asignación compuesta | Acumular notas     |
| /        | Aritmético           | Calcular promedio  |
| <        | Relacional           | Controlar ciclos   |
| ++       | Incremento           | Avanzar posiciones |

---

## Estructuras utilizadas

| Estructura       | Uso                    |
| ---------------- | ---------------------- |
| Secuencial       | Leer y procesar datos  |
| Repetitiva (for) | Ingresar y sumar notas |

---

## Fórmulas utilizadas

### Acumulación de notas

```text
suma += notas[i]
```

### Cálculo del promedio

```text
promedio = suma / n
```

---

# Pseudocódigo

```text
INICIO

    Definir suma Como Real
    Definir promedio Como Real
    Definir i, n, aux Como Entero

    Definir notas[] Como Array

    Escribir "Ingrese la cantidad de notas: "
    Leer n

    suma = 0

    For (i = 0; i < n; i++)

        Escribir "Ingrese la nota ", i + 1
        Leer aux

        notas[i] = aux

    EndFor

    For (i = 0; i < n; i++)

        suma += notas[i]

    EndFor

    promedio = suma / n

    Mostrar "El promedio es: ", promedio

FIN
```

---

# Prueba de Escritorio

## Caso 1

### Datos de entrada

```text
n = 5
```

Notas:

```text
80
70
90
60
100
```

### Primer FOR (guardar las notas)

| n | i | aux | notas[]           |
| - | - | --- | ----------------- |
| 5 | 0 | 80  | [80]              |
| 5 | 1 | 70  | [80,70]           |
| 5 | 2 | 90  | [80,70,90]        |
| 5 | 3 | 60  | [80,70,90,60]     |
| 5 | 4 | 100 | [80,70,90,60,100] |

> Al terminar:

```text
suma = 0
notas = [80,70,90,60,100]
```

### Segundo FOR (sumar las notas)

| i | notas[i] | suma |
| - | -------- | ---- |
| 0 | 80       | 80   |
| 1 | 70       | 150  |
| 2 | 90       | 240  |
| 3 | 60       | 300  |
| 4 | 100      | 400  |

### Cálculo del promedio

```text
promedio = suma / n

promedio = 400 / 5

promedio = 80
```

### Resultado

```text
El promedio es: 80
```

---

# Implementación en C++

```cpp
#include <iostream>

using namespace std;

int main() {
    double suma;
    double promedio;
    int i, n, aux;

    cout << "Ingrese la cantidad de notas: ";
    cin >> n;

    int notas[n];

    suma = 0;

    for (i = 0; i < n; i++) {
        cout << "Ingrese la nota " << i + 1 << ": ";
        cin >> aux;

        notas[i] = aux;
    }

    for (i = 0; i < n; i++) {
        suma += notas[i];
    }

    promedio = suma / n;

    cout << "El promedio es: " << promedio << endl;

    return 0;
}
```
