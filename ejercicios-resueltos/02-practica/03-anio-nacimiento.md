# Calcular el año de nacimiento y mostrar los años cumplidos

## Enunciado

Construir un algoritmo que pida al usuario su edad, calcule el año de nacimiento y muestre por pantalla todos los años que ha cumplido.

### Ejemplo

Si:

```text
edad = 4
```

Mostrar:

```text
Anio 2022: Nacio
Anio 2023: Cumplio 1 anio
Anio 2024: Cumplio 2 anios
Anio 2025: Cumplio 3 anios
Anio 2026: Cumplio 4 anios
```

---

# Análisis del Problema

## Entradas

| Dato | Tipo   |
| ---- | ------ |
| edad | Entero |

## Proceso

1. Leer la edad del usuario.
2. Asignar el año actual.
3. Calcular el año de nacimiento.
4. Recorrer los años desde el nacimiento hasta el año actual.
5. Verificar si el año recorrido corresponde al año de nacimiento.
6. Si corresponde al año de nacimiento, mostrar que nació ese año.
7. En caso contrario, calcular los años cumplidos.
8. Mostrar el año y la edad cumplida.

## Salidas

| Salida            |
| ----------------- |
| Año de nacimiento |
| Años cumplidos    |

---

# Diseño de la Solución

## Secuencia lógica

1. Solicitar la edad del usuario.
2. Leer el valor de la edad.
3. Asignar el año actual.
4. Calcular el año de nacimiento.
5. Recorrer los años desde el año de nacimiento hasta el año actual.
6. Verificar si el año recorrido corresponde al año de nacimiento.
7. Si corresponde al año de nacimiento, mostrar que nació ese año.
8. En caso contrario, calcular los años cumplidos.
9. Mostrar el año y la edad cumplida.
10. Finalizar el algoritmo.

---

## Variables utilizadas

| Variable        | Tipo   | Descripción                          |
| --------------- | ------ | ------------------------------------ |
| edad            | Entero | Edad ingresada por el usuario        |
| anio_actual     | Entero | Año de referencia                    |
| anio_nacimiento | Entero | Año calculado de nacimiento          |
| anio            | Entero | Variable de control del ciclo        |
| cumplidos       | Entero | Años cumplidos en cada año recorrido |

---

## Operadores utilizados

| Operador | Tipo       | Uso                          |
| -------- | ---------- | ---------------------------- |
| =        | Asignación | Asignar valores              |
| -        | Aritmético | Calcular diferencias de años |
| ==       | Relacional | Comparar años                |
| <=       | Relacional | Controlar el ciclo           |
| ++       | Incremento | Avanzar años                 |

---

## Estructuras utilizadas

| Estructura              | Uso                                                |
| ----------------------- | -------------------------------------------------- |
| Secuencial              | Leer datos y realizar cálculos                     |
| Condicional (if - else) | Diferenciar el año de nacimiento de los cumpleaños |
| Repetitiva (for)        | Recorrer los años                                  |

---

## Fórmulas utilizadas

### Año de nacimiento

```text
anio_nacimiento = anio_actual - edad
```

### Años cumplidos

```text
cumplidos = anio - anio_nacimiento
```

---

# Pseudocódigo

```text
INICIO

    Definir edad, anio, anio_actual Como Entero
    Definir anio_nacimiento, cumplidos Como Entero

    Escribir "Ingrese su edad:"
    Leer edad

    anio_actual = 2026

    anio_nacimiento = anio_actual - edad

    for (anio = anio_nacimiento; anio <= anio_actual; anio++)

        if (anio == anio_nacimiento) Then

            Mostrar "Anio ", anio, ": Nacio"

        else

            cumplidos = anio - anio_nacimiento

            Mostrar "Anio ", anio, ": Cumplio ", cumplidos, " anios"

        EndIf

    EndFor

FIN
```

---

# Prueba de Escritorio

## Caso 1

### Datos de entrada

```text
edad = 7
```

### Cálculos

```text
anio_actual = 2026

anio_nacimiento = 2026 - 4

anio_nacimiento = 2022
```

### Seguimiento

| edad | anio_actual | anio_nacimiento | anio | cumplidos | Salida                   |
| ---- | ----------- | --------------- | ---- | --------- | ------------------------ |
| 7    | 2026        | 2019            | 2019 | -         | Año 2019: Nació          |
| 7    | 2026        | 2019            | 2020 | 1         | Año 2020: Cumplió 1 año  |
| 7    | 2026        | 2019            | 2021 | 2         | Año 2021: Cumplió 2 años |
| 7    | 2026        | 2019            | 2022 | 3         | Año 2022: Cumplió 3 años |
| 7    | 2026        | 2019            | 2023 | 4         | Año 2023: Cumplió 4 años |
| 7    | 2026        | 2019            | 2024 | 5         | Año 2024: Cumplió 5 años |
| 7    | 2026        | 2019            | 2025 | 6         | Año 2025: Cumplió 6 años |
| 7    | 2026        | 2019            | 2026 | 7         | Año 2026: Cumplió 7 años |

### Resultado

```text
Año 2019: Nació
Año 2020: Cumplió 1 año
Año 2021: Cumplió 2 años
Año 2022: Cumplió 3 años
Año 2023: Cumplió 4 años
Año 2024: Cumplió 5 años
Año 2025: Cumplió 6 años
Año 2026: Cumplió 7 años
```

---

# Implementación en C++

```cpp
#include <iostream>

using namespace std;

int main() {
    int edad, anio, anio_actual, anio_nacimiento, cumplidos;

    cout << "Ingrese su edad: ";
    cin >> edad;

    anio_actual = 2026;

    anio_nacimiento = anio_actual - edad;

    for (anio = anio_nacimiento; anio <= anio_actual; anio++) {

        if (anio == anio_nacimiento) {

            cout << "Anio " << anio << ": Nacio" << endl;

        } else {

            cumplidos = anio - anio_nacimiento;

            cout << "Anio " << anio << ": Cumplio " << cumplidos << " anios" << endl;
        }
    }

    return 0;
}
```
