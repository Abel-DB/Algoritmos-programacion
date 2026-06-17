# Registro de Socios de un Club

## Enunciado

Construir una estructura que permita registrar socios de un club solicitando:

* Nombre
* Apellido
* Edad

Se debe mostrar el porcentaje de socios de cada categoría:

* Mayores: edad mayor o igual a 21 años.
* Juveniles: edad menor de 21 y mayor o igual a 16 años.
* Pre-juveniles: edad menor de 16 y mayor o igual a 12 años.
* Niños: edad menor a 12 años.

---

# Análisis

## Entradas

| Dato | Tipo |
|--------|--------|
| n | Entero |
| nombre | Cadena |
| apellido | Cadena |
| edad | Entero |

---

## Proceso

1. Solicitar la cantidad de socios.
2. Registrar nombre, apellido y edad de cada socio.
3. Almacenar los datos en una estructura.
4. Clasificar cada socio según su edad.
5. Contar la cantidad de socios por categoría.
6. Calcular los porcentajes de cada categoría.
7. Mostrar los resultados.

---

## Salidas

| Salida |
|---------|
| Porcentaje de Mayores |
| Porcentaje de Juveniles |
| Porcentaje de Pre-juveniles |
| Porcentaje de Niños |

---

## Restricciones

* La cantidad de socios debe ser mayor que 0.
* La edad no puede ser negativa.

---

# Casos de Prueba

| Socios | Mayores | Juveniles | Pre-juveniles | Niños |
|---------|---------|---------|---------|---------|
| 5 | 40% | 20% | 20% | 20% |
| 4 | 25% | 25% | 25% | 25% |
| 3 | 100% | 0% | 0% | 0% |

---

# Estrategia de Solución

Se utilizará una estructura para almacenar los datos de cada socio.

A medida que se registren los socios, se clasificará cada uno según su edad y se incrementará el contador correspondiente.

Finalmente se calcularán los porcentajes de cada categoría utilizando la cantidad total de socios.

---

# Variables

| Variable | Tipo | Descripción |
|-----------|-----------|-----------|
| n | Entero | Cantidad de socios |
| i | Entero | Control del ciclo |
| mayores | Entero | Cantidad de socios mayores |
| juveniles | Entero | Cantidad de socios juveniles |
| prejuveniles | Entero | Cantidad de socios pre-juveniles |
| ninos | Entero | Cantidad de socios niños |
| por_mayores | Real | Porcentaje de socios mayores |
| por_juveniles | Real | Porcentaje de socios juveniles |
| por_prejuveniles | Real | Porcentaje de socios pre-juveniles |
| por_ninos | Real | Porcentaje de socios niños |
| socios[] | Array de Socio | Almacena los datos de los socios |

---

# Operadores

| Operador | Tipo | Uso |
|-----------|-----------|-----------|
| = | Asignación | Asignar valores |
| >= | Relacional | Clasificar edades |
| < | Relacional | Clasificar edades |
| ++ | Incremento | Incrementar contadores |
| * | Aritmético | Calcular porcentajes |
| / | Aritmético | Calcular porcentajes |

---

# Estructuras Utilizadas

```text
If Else If
```

Permite clasificar los socios según su edad.

```text
For
```

Permite recorrer todos los socios registrados.

---

# Estructura de Datos Utilizada

```text
Struct Socio
```

Permite agrupar los datos relacionados con cada socio.

---

# Fórmulas

### Porcentaje de Mayores

```text
por_mayores = (mayores * 100.0) / n
```

### Porcentaje de Juveniles

```text
por_juveniles = (juveniles * 100.0) / n
```

### Porcentaje de Pre-juveniles

```text
por_prejuveniles = (prejuveniles * 100.0) / n
```

### Porcentaje de Niños

```text
por_ninos = (ninos * 100.0) / n
```

---

# Secuencia Lógica

1. Inicio.
2. Definir la estructura Socio.
3. Definir las variables necesarias.
4. Inicializar los contadores en cero.
5. Solicitar la cantidad de socios.
6. Crear el array de socios.
7. Registrar nombre, apellido y edad de cada socio.
8. Clasificar cada socio según su edad.
9. Incrementar el contador correspondiente.
10. Calcular los porcentajes de cada categoría.
11. Mostrar los porcentajes obtenidos.
12. Fin.

---

# Pseudocódigo

```text
Inicio

    Definir Socio

        nombre : Cadena
        apellido : Cadena
        edad : Entero

    FinDefinir

    Definir n Como Entero
    Definir i Como Entero

    Definir mayores Como Entero
    Definir juveniles Como Entero
    Definir prejuveniles Como Entero
    Definir ninos Como Entero

    Definir por_mayores Como Real
    Definir por_juveniles Como Real
    Definir por_prejuveniles Como Real
    Definir por_ninos Como Real

    Definir socios[] Como Array de Socio

    mayores = 0
    juveniles = 0
    prejuveniles = 0
    ninos = 0

    Escribir "Ingrese la cantidad de socios: "
    Leer n

    for (i = 0; i < n; i++)

        Escribir "Nombre: "
        Leer socios[i].nombre

        Escribir "Apellido: "
        Leer socios[i].apellido

        Escribir "Edad: "
        Leer socios[i].edad

        if (socios[i].edad >= 21) then
            mayores++
        else if (socios[i].edad >= 16) then
            juveniles++
        else if (socios[i].edad >= 12) then
            prejuveniles++
        else
            ninos++
        endif
    endfor

    por_mayores = (mayores * 100.0) / n
    por_juveniles = (juveniles * 100.0) / n
    por_prejuveniles = (prejuveniles * 100.0) / n
    por_ninos = (ninos * 100.0) / n

    Escribir "Porcentaje de Mayores: ", por_mayores, "%"
    Escribir "Porcentaje de Juveniles: ", por_juveniles, "%"
    Escribir "Porcentaje de Pre-juveniles: ", por_prejuveniles, "%"
    Escribir "Porcentaje de Ninos: ", por_ninos, "%"

Fin
```

---

# Prueba de Escritorio

## Caso 1

### Entrada

| Nombre | Apellido | Edad |
|----------|----------|------|
| Juan | Perez | 25 |
| Ana | Lopez | 18 |
| Carlos | Ruiz | 14 |
| Maria | Flores | 10 |
| Pedro | Gomez | 22 |

### Conteo

| Categoría | Cantidad |
|------------|----------|
| Mayores | 2 |
| Juveniles | 1 |
| Pre-juveniles | 1 |
| Niños | 1 |

### Cálculo

```text
por_mayores = (2 * 100) / 5 = 40

por_juveniles = (1 * 100) / 5 = 20

por_prejuveniles = (1 * 100) / 5 = 20

por_ninos = (1 * 100) / 5 = 20
```

### Salida

```text
Porcentaje de Mayores: 40%

Porcentaje de Juveniles: 20%

Porcentaje de Pre-juveniles: 20%

Porcentaje de Ninos: 20%
```

---

# Implementación

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

    int n;
    int i;

    int mayores;
    int juveniles;
    int prejuveniles;
    int ninos;

    double por_mayores;
    double por_juveniles;
    double por_prejuveniles;
    double por_ninos;

    mayores = 0;
    juveniles = 0;
    prejuveniles = 0;
    ninos = 0;

    cout << "Ingrese la cantidad de socios: ";
    cin >> n;

    Socio socios[n];

    for (i = 0; i < n; i++) {

        cout << "\nNombre: ";
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
