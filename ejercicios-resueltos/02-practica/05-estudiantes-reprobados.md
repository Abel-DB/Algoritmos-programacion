# Contar estudiantes aprobados y reprobados

## Enunciado

Construir un algoritmo que pida al usuario **n** notas de estudiantes, contar y mostrar el número de estudiantes aprobados y el número de estudiantes reprobados.

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
El numero de estudiantes aprobados es: 4
El numero de estudiantes reprobados es: 1
```

---

# Análisis del Problema

## Entradas

| Dato    | Tipo               |
| ------- | ------------------ |
| n       | Entero             |
| notas[] | Arreglo de enteros |

## Proceso

1. Pedir la cantidad de estudiantes.
2. Almacenar las notas en una tabla.
3. Recorrer la tabla de notas.
4. Determinar si cada nota está aprobada o reprobada.
5. Contar la cantidad de aprobados.
6. Contar la cantidad de reprobados.
7. Mostrar los resultados obtenidos.

## Salidas

| Salida                             |
| ---------------------------------- |
| Cantidad de estudiantes aprobados  |
| Cantidad de estudiantes reprobados |

---

# Diseño de la Solución

## Secuencia lógica

1. Solicitar la cantidad de estudiantes.
2. Leer el valor de n.
3. Crear una tabla para almacenar las notas.
4. Inicializar los contadores aprobados y reprobados en 0.
5. Ingresar las n notas y almacenarlas en la tabla.
6. Recorrer la tabla de notas.
7. Verificar si cada nota está aprobada o reprobada.
8. Incrementar el contador correspondiente.
9. Mostrar la cantidad de aprobados.
10. Mostrar la cantidad de reprobados.
11. Finalizar el algoritmo.

---

## Variables utilizadas

| Variable   | Tipo    | Descripción                        |
| ---------- | ------- | ---------------------------------- |
| n          | Entero  | Cantidad de estudiantes            |
| i          | Entero  | Control del ciclo                  |
| aux        | Entero  | Nota ingresada temporalmente       |
| aprobados  | Entero  | Cantidad de estudiantes aprobados  |
| reprobados | Entero  | Cantidad de estudiantes reprobados |
| notas[]    | Arreglo | Almacena las notas ingresadas      |

---

## Operadores utilizados

| Operador | Tipo                 | Uso                    |
| -------- | -------------------- | ---------------------- |
| =        | Asignación           | Asignar valores        |
| >=       | Relacional           | Determinar aprobación  |
| <        | Relacional           | Controlar ciclos       |
| +=       | Asignación compuesta | Incrementar contadores |
| ++       | Incremento           | Avanzar posiciones     |

---

## Estructuras utilizadas

| Estructura              | Uso                               |
| ----------------------- | --------------------------------- |
| Secuencial              | Leer y almacenar datos            |
| Condicional (if - else) | Determinar aprobados y reprobados |
| Repetitiva (for)        | Recorrer la tabla                 |

---

## Fórmulas utilizadas

### Verificación de aprobación

```text
notas[i] >= 51
```

### Conteo de aprobados

```text
aprobados += 1
```

### Conteo de reprobados

```text
reprobados += 1
```

---

# Pseudocódigo

```text
INICIO

    Definir n, i, aux, aprobados, reprobados Como Entero
    Definir notas[] Como Array

    Escribir "Ingrese la cantidad de estudiantes: "
    Leer n

    aprobados = 0
    reprobados = 0

    For i = 0; i < n; i++

        Escribir "Ingrese la nota ", i + 1
        Leer aux

        notas[i] = aux

    EndFor

    For i = 0; i < n; i++

        If notas[i] >= 51

            aprobados += 1

        Else

            reprobados += 1

        EndIf

    EndFor

    Escribir "El numero de estudiantes aprobados es: ", aprobados
    Escribir "El numero de estudiantes reprobados es: ", reprobados

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
45
51
89
45
30
```

### Seguimiento

| i       | nota | aprobados | reprobados |
| ------- | ---- | --------- | ---------- |
| Inicial | -    | 0         | 0          |
| 0       | 45   | 0         | 1          |
| 1       | 51   | 1         | 1          |
| 2       | 89   | 2         | 1          |
| 3       | 45   | 2         | 2          |
| 4       | 30   | 2         | 3          |

### Resultado

```text
El numero de estudiantes aprobados es: 2

El numero de estudiantes reprobados es: 3
```

---

# Implementación en C++

```cpp
#include <iostream>

using namespace std;

int main() {
    int n, i, aux, aprobados, reprobados;

    cout << "Ingrese la cantidad de estudiantes: ";
    cin >> n;

    int notas[n];

    aprobados = 0;
    reprobados = 0;

    for (i = 0; i < n; i++) {
        cout << "Ingrese la nota " << i + 1 << ": ";
        cin >> aux;

        notas[i] = aux;
    }

    for (i = 0; i < n; i++) {
        if (notas[i] >= 51) {
            aprobados += 1;
        } else {
            reprobados += 1;
        }
    }

    cout << "El numero de estudiantes aprobados es: "
         << aprobados << endl;

    cout << "El numero de estudiantes reprobados es: "
         << reprobados << endl;

    return 0;
}
```
