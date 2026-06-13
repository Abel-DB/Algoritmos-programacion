# Registro de Socios de un Club

## Enunciado

Construir una estructura **struct** que permita registrar socios de un club solicitando:

* Nombre
* Apellido
* Edad

Se debe mostrar el porcentaje de socios de cada categoría:

* **Mayores:** edad mayor o igual a 21 años.
* **Juveniles:** edad menor de 21 y mayor o igual a 16 años.
* **Pre-juveniles:** edad menor de 16 y mayor o igual a 12 años.
* **Niños:** edad menor a 12 años.

---

# Análisis del Problema

## Entradas

| Dato     | Tipo   |
| -------- | ------ |
| n        | Entero |
| nombre   | Cadena |
| apellido | Cadena |
| edad     | Entero |

---

## Proceso

1. Solicitar la cantidad de socios.
2. Leer el valor de n.
3. Registrar nombre, apellido y edad de cada socio.
4. Almacenar los datos en una estructura.
5. Clasificar cada socio según su edad.
6. Contar la cantidad de socios por categoría.
7. Calcular el porcentaje de cada categoría.
8. Mostrar los resultados.

---

## Salidas

| Salida                      |
| --------------------------- |
| Porcentaje de Mayores       |
| Porcentaje de Juveniles     |
| Porcentaje de Pre-juveniles |
| Porcentaje de Niños         |

---

# Variables Utilizadas

| Variable        | Tipo   | Descripción                      |
| --------------- | ------ | -------------------------------- |
| n               | Entero | Cantidad de socios               |
| i               | Entero | Control del ciclo                |
| mayores         | Entero | Cantidad de socios mayores       |
| juveniles       | Entero | Cantidad de socios juveniles     |
| prejuveniles    | Entero | Cantidad de socios pre-juveniles |
| ninos           | Entero | Cantidad de socios niños         |
| porMayores      | Real   | Porcentaje de mayores            |
| porJuveniles    | Real   | Porcentaje de juveniles          |
| porPrejuveniles | Real   | Porcentaje de pre-juveniles      |
| porNinos        | Real   | Porcentaje de niños              |

---

# Estructura Utilizada

```cpp
struct Socio {
    string nombre;
    string apellido;
    int edad;
};
```

---

# Operadores Utilizados

| Operador | Tipo       | Uso                    |
| -------- | ---------- | ---------------------- |
| =        | Asignación | Asignar valores        |
| >=       | Relacional | Clasificar edades      |
| <        | Relacional | Clasificar edades      |
| ++       | Incremento | Incrementar contadores |
| *        | Aritmético | Calcular porcentajes   |
| /        | Aritmético | Calcular porcentajes   |

---

# Estructuras Utilizadas

| Estructura                 | Uso                       |
| -------------------------- | ------------------------- |
| Secuencial                 | Lectura y cálculos        |
| Condicional (if - else if) | Clasificar categorías     |
| Repetitiva (for)           | Recorrer socios           |
| Struct                     | Almacenar datos de socios |

---

# Fórmulas Utilizadas

### Porcentaje de Mayores

```text
porMayores = (mayores * 100.0) / n
```

### Porcentaje de Juveniles

```text
porJuveniles = (juveniles * 100.0) / n
```

### Porcentaje de Pre-juveniles

```text
porPrejuveniles = (prejuveniles * 100.0) / n
```

### Porcentaje de Niños

```text
porNinos = (ninos * 100.0) / n
```

---

# Secuencia Lógica

1. Solicitar la cantidad de socios.
2. Leer el valor de n.
3. Crear una estructura para almacenar los datos del socio.
4. Inicializar los contadores de categorías en 0.
5. Ingresar nombre, apellido y edad de cada socio.
6. Clasificar al socio según su edad.
7. Incrementar el contador correspondiente.
8. Repetir el proceso para todos los socios.
9. Calcular los porcentajes de cada categoría.
10. Mostrar los porcentajes obtenidos.
11. Finalizar el algoritmo.

---

# Pseudocódigo

```text
INICIO

    Definir Socio
        nombre : cadena
        apellido : cadena
        edad : entero
    FinDefinir

    Definir n, i Como Entero
    Definir mayores, juveniles, prejuveniles, ninos Como Entero
    Definir por_mayores, por_juveniles, por_prejuveniles, por_ninos Como Real

    mayores = 0
    juveniles = 0
    prejuveniles = 0
    ninos = 0

    Escribir "Ingrese la cantidad de socios: "
    Leer n

    Socio socios[n]

    For (i = 0; i < n; i++)

        Escribir "Nombre: "
        Leer socios[i].nombre

        Escribir "Apellido: "
        Leer socios[i].apellido

        Escribir "Edad: "
        Leer socios[i].edad

        If (socios[i].edad >= 21) Then

            mayores++

        Else If (socios[i].edad >= 16) Then

            juveniles++

        Else If (socios[i].edad >= 12) Then

            prejuveniles++

        Else

            ninos++

        EndIf

    EndFor

    por_mayores = (mayores * 100.0) / n
    por_juveniles = (juveniles * 100.0) / n
    por_prejuveniles = (prejuveniles * 100.0) / n
    por_ninos = (ninos * 100.0) / n

    Mostrar por_mayores
    Mostrar por_juveniles
    Mostrar por_prejuveniles
    Mostrar por_ninos

FIN
```

---

# Prueba de Escritorio

## Datos de entrada

| i | Nombre | Apellido | Edad |
| - | ------ | -------- | ---- |
| 0 | Juan   | Pérez    | 25   |
| 1 | Ana    | López    | 18   |
| 2 | Carlos | Ruiz     | 14   |
| 3 | María  | Flores   | 10   |
| 4 | Pedro  | Gómez    | 22   |


### Conteo

| i | Edad | Categoría  | Mayores | Juveniles | Prejuveniles | Niños |
| - | ---- | ---------- | ------- | --------- | ------------ | ----- |
| 0 | 25   | Mayor      | 1       | 0         | 0            | 0     |
| 1 | 18   | Juvenil    | 1       | 1         | 0            | 0     |
| 2 | 14   | Prejuvenil | 1       | 1         | 1            | 0     |
| 3 | 10   | Niño       | 1       | 1         | 1            | 1     |
| 4 | 22   | Mayor      | 2       | 1         | 1            | 1     |

| Variable     | Valor |
| ------------ | ----- |
| mayores      | 2     |
| juveniles    | 1     |
| prejuveniles | 1     |
| ninos        | 1     |
| n            | 5     |


### Porcentajes

| Categoría     | Porcentaje |
| ------------- | ---------- |
| Mayores       | 40%        |
| Juveniles     | 20%        |
| Pre-juveniles | 20%        |
| Niños         | 20%        |

---

# Implementación en C++

```cpp
#include <iostream>
#include <string>

using namespace std;

struct Socio {
    string nombre;
    string apellido;
    int edad;
};

int main() {
    int n, i, mayores, juveniles, prejuveniles, ninos;
    double por_mayores, por_juveniles, por_prejuveniles, por_ninos;

    mayores = 0;
    juveniles = 0;
    prejuveniles = 0;
    ninos = 0;

    cout << "Ingrese la cantidad de socios: ";
    cin >> n;

    Socio socios[n];

    for (i = 0; i < n; i++) {

        cout << "Nombre: ";
        cin >> socios[i].nombre;

        cout << "Apellido: ";
        cin >> socios[i].apellido;

        cout << "Edad: ";
        cin >> socios[i].edad;

        if (socios[i].edad >= 21) {

            mayores++;

        } else if (socios[i].edad >= 16) {

            juveniles++;

        } else if (socios[i].edad >= 12) {

            prejuveniles++;

        } else {

            ninos++;
        }
    }

    por_mayores = (mayores * 100.0) / n;
    por_juveniles = (juveniles * 100.0) / n;
    por_prejuveniles = (prejuveniles * 100.0) / n;
    por_ninos = (ninos * 100.0) / n;

    cout << "\nPorcentaje de Mayores: " << por_mayores << "%" << endl;
    cout << "Porcentaje de Juveniles: " << por_juveniles << "%" << endl;
    cout << "Porcentaje de Pre-juveniles: " << por_prejuveniles << "%" << endl;
    cout << "Porcentaje de Ninos: " << por_ninos << "%" << endl;

    return 0;
}
```
