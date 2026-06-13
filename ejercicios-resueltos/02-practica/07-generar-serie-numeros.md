# Generar los n primeros términos de una serie

## Enunciado

Construir un algoritmo que genere y almacene en un arreglo los **n** primeros números de la siguiente serie:

```text
1, 2, 4, 8, 16, 32, 64, 128, ...
```

### Ejemplo

Si:

```text
n = 5
```

Mostrar:

```text
1, 2, 4, 8, 16
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
3. Crear un arreglo para almacenar la serie.
4. Generar los términos de la serie.
5. Guardar cada término en el arreglo.
6. Mostrar la serie generada.

## Salidas

| Salida         |
| -------------- |
| Serie generada |

---

# Diseño de la Solución

## Secuencia lógica

1. Solicitar la cantidad de términos de la serie.
2. Leer el valor de n.
3. Crear un arreglo para almacenar la serie.
4. Asignar el valor 1 al primer elemento del arreglo.
5. Recorrer el arreglo desde la posición 1 hasta n - 1.
6. Generar cada término multiplicando el término anterior por 2.
7. Guardar cada término generado en el arreglo.
8. Recorrer el arreglo para mostrar todos los términos de la serie.
9. Mostrar la serie generada.
10. Finalizar el algoritmo.

---

## Variables utilizadas

| Variable | Tipo    | Descripción                       |
| -------- | ------- | --------------------------------- |
| n        | Entero  | Cantidad de términos de la serie  |
| i        | Entero  | Variable de control del ciclo     |
| serie[]  | Arreglo | Almacena los términos de la serie |

---

## Operadores utilizados

| Operador | Tipo       | Uso                         |
| -------- | ---------- | --------------------------- |
| =        | Asignación | Asignar valores             |
| *        | Aritmético | Multiplicar por 2           |
| -        | Aritmético | Acceder al término anterior |
| <        | Relacional | Controlar el ciclo          |
| ++       | Incremento | Avanzar posiciones          |

---

## Estructuras utilizadas

| Estructura       | Uso                          |
| ---------------- | ---------------------------- |
| Secuencial       | Leer datos y asignar valores |
| Repetitiva (for) | Generar y mostrar la serie   |

---

## Fórmulas utilizadas

### Primer término

```text
serie[0] = 1
```

### Generación de la serie

```text
serie[i] = serie[i - 1] * 2
```

---

# Pseudocódigo

```text
INICIO

    Definir n, i Como Entero
    Definir serie[] Como Array

    Escribir "Ingrese la cantidad de terminos de la serie: "
    Leer n

    serie[0] = 1

    For (i = 1; i < n; i++)

        serie[i] = serie[i - 1] * 2

    EndFor

    For (i = 0; i < n; i++)

        Mostrar serie[i]

    EndFor

FIN
```

---

# Prueba de Escritorio

## Caso 1

### Datos de entrada

```text
n = 5
```

### Datos iniciales

```text
serie[0] = 1
```

### Primer FOR 

| i | serie[i] |
| - | -------- |
| 0 | 1        |
| 1 | 2        |
| 2 | 4        |
| 3 | 8        |
| 4 | 16       |

> Porque:

```text
serie[1] = 1 * 2 = 2
serie[2] = 2 * 2 = 4
serie[3] = 4 * 2 = 8
serie[4] = 8 * 2 = 16
```

### Segundo FOR (Mostrar la serie)

| i | Mostrar serie[i] |
| - | ---------------- |
| 0 | 1                |
| 1 | 2                |
| 2 | 4                |
| 3 | 8                |
| 4 | 16               |
    

### Resultado

```text
1, 2, 4, 8, 16
```

---

# Implementación en C++

```cpp
#include <iostream>

using namespace std;

int main() {
    int n, i;

    cout << "Ingrese la cantidad de terminos de la serie: ";
    cin >> n;

    int serie[n];

    serie[0] = 1;

    for (i = 1; i < n; i++) {
        serie[i] = serie[i - 1] * 2;
    }

    for (i = 0; i < n; i++) {
        cout << serie[i] << ", ";
    }

    cout << endl;

    return 0;
}
```
