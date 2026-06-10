# Registro de socios de un club utilizando struct

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

## Proceso

1. Solicitar la cantidad de socios.
2. Registrar nombre, apellido y edad de cada socio.
3. Clasificar cada socio según su edad.
4. Contar la cantidad de socios por categoría.
5. Calcular el porcentaje de cada categoría.
6. Mostrar los resultados.

## Salidas

| Salida                      |
| --------------------------- |
| Porcentaje de Mayores       |
| Porcentaje de Juveniles     |
| Porcentaje de Pre-juveniles |
| Porcentaje de Niños         |

---

# Diseño de la Solución

## Secuencia lógica

1. Solicitar la cantidad de socios.
2. Leer el valor de n.
3. Crear una estructura para almacenar los datos del socio.
4. Inicializar los contadores de categorías en 0.
5. Ingresar nombre, apellido y edad de cada socio.
6. Clasificar al socio según su edad.
7. Incrementar el contador correspondiente.
8. Repetir el proceso para todos los socios.
9. Calcular el porcentaje de cada categoría.
10. Mostrar los porcentajes obtenidos.
11. Finalizar el algoritmo.

---

## Variables utilizadas

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

## Estructura utilizada

```cpp
struct Socio {
    string nombre;
    string apellido;
    int edad;
};
```

---

## Operadores utilizados

| Operador | Tipo       | Uso                    |
| -------- | ---------- | ---------------------- |
| =        | Asignación | Asignar valores        |
| >=       | Relacional | Clasificar edades      |
| <        | Relacional | Clasificar edades      |
| ++       | Incremento | Incrementar contadores |
| *        | Aritmético | Calcular porcentajes   |
| /        | Aritmético | Calcular porcentajes   |

---

## Estructuras utilizadas

| Estructura                 | Uso                         |
| -------------------------- | --------------------------- |
| Secuencial                 | Lectura y cálculos          |
| Condicional (if - else if) | Clasificación de categorías |
| Repetitiva (for)           | Recorrer socios             |
| Struct                     | Almacenar datos de socios   |

---

## Fórmulas utilizadas

### Porcentaje de mayores

```text
(mayores * 100.0) / n
```

### Porcentaje de juveniles

```text
(juveniles * 100.0) / n
```

### Porcentaje de pre-juveniles

```text
(prejuveniles * 100.0) / n
```

### Porcentaje de niños

```text
(ninos * 100.0) / n
```

---

# Pseudocódigo

```text
INICIO

    Definir n, i Como Entero
    Definir mayores, juveniles, prejuveniles, ninos Como Entero
    Definir porMayores, porJuveniles, porPrejuveniles, porNinos Como Real

    mayores = 0
    juveniles = 0
    prejuveniles = 0
    ninos = 0

    Leer n

    Para i = 0 Hasta n - 1

        Leer nombre
        Leer apellido
        Leer edad

        Si edad >= 21 Entonces

            mayores++

        Sino Si edad >= 16 Entonces

            juveniles++

        Sino Si edad >= 12 Entonces

            prejuveniles++

        Sino

            ninos++

        FinSi

    FinPara

    porMayores = (mayores * 100.0) / n
    porJuveniles = (juveniles * 100.0) / n
    porPrejuveniles = (prejuveniles * 100.0) / n
    porNinos = (ninos * 100.0) / n

    Mostrar porMayores
    Mostrar porJuveniles
    Mostrar porPrejuveniles
    Mostrar porNinos

FIN
```

---

# Prueba de Escritorio

## Datos de entrada

| Nombre | Apellido | Edad |
| ------ | -------- | ---- |
| Juan   | Perez    | 25   |
| Ana    | Lopez    | 18   |
| Luis   | Garcia   | 14   |
| Pedro  | Rojas    | 10   |

### Conteo

| Categoría     | Cantidad |
| ------------- | -------- |
| Mayores       | 1        |
| Juveniles     | 1        |
| Pre-juveniles | 1        |
| Niños         | 1        |

### Porcentajes

| Categoría     | Porcentaje |
| ------------- | ---------- |
| Mayores       | 25%        |
| Juveniles     | 25%        |
| Pre-juveniles | 25%        |
| Niños         | 25%        |

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
    int n, i;
    int mayores, juveniles, prejuveniles, ninos;

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

    double porMayores = (mayores * 100.0) / n;
    double porJuveniles = (juveniles * 100.0) / n;
    double porPrejuveniles = (prejuveniles * 100.0) / n;
    double porNinos = (ninos * 100.0) / n;

    cout << "\nPorcentaje de Mayores: " << porMayores << "%" << endl;
    cout << "Porcentaje de Juveniles: " << porJuveniles << "%" << endl;
    cout << "Porcentaje de Pre-juveniles: " << porPrejuveniles << "%" << endl;
    cout << "Porcentaje de Ninos: " << porNinos << "%" << endl;

    return 0;
}
```
