# Ejercicio 02 - Consumo de Combustible de una Motocicleta

## Enunciado

Una motocicleta consume 5 litros de combustible por cada 100 kilómetros recorridos. Construir un algoritmo que permita ingresar los datos de una motocicleta y calcular el combustible consumido según la distancia recorrida.

Datos de la motocicleta:

* Marca
* Modelo
* Año de fabricación
* Kilómetros recorridos

---

# Análisis del Problema

## Entradas

| Dato       | Tipo   |
| ---------- | ------ |
| marca      | string |
| modelo     | string |
| anio       | int    |
| kilometros | float  |

---

## Proceso

1. Leer los datos de la motocicleta.
2. Leer los kilómetros recorridos.
3. Calcular el combustible consumido.
4. Mostrar los datos ingresados.
5. Mostrar el combustible consumido.

---

## Salidas

| Salida                  |
| ----------------------- |
| Datos de la motocicleta |
| Litros consumidos       |

---

# Diseño de la Solución

## Secuencia Lógica

1. Inicio.
2. Ingresar marca de la motocicleta.
3. Ingresar modelo.
4. Ingresar año de fabricación.
5. Ingresar kilómetros recorridos.
6. Calcular combustible consumido.
7. Mostrar los datos de la motocicleta.
8. Mostrar el combustible consumido.
9. Fin.

---

## Variables Utilizadas

| Variable    | Tipo   | Descripción              |
| ----------- | ------ | ------------------------ |
| marca       | string | Marca de la motocicleta  |
| modelo      | string | Modelo de la motocicleta |
| anio        | int    | Año de fabricación       |
| kilometros  | float  | Distancia recorrida      |
| combustible | float  | Litros consumidos        |

---

## Estructura Utilizada

```cpp
struct Motocicleta
```

Permite agrupar información relacionada en una sola variable.

---

## Fórmula Utilizada

La motocicleta consume:

```text
5 litros → 100 km
```

Por regla de tres:

```text
combustible = (kilometros * 5) / 100
```

---

# Pseudocódigo

```text
INICIO

    Definir motocicleta

    Leer marca
    Leer modelo
    Leer año
    Leer kilómetros

    combustible ← (kilómetros * 5) / 100

    Mostrar datos de la motocicleta
    Mostrar combustible consumido

FIN
```

---

# Diagrama de Flujo

```mermaid
flowchart TD

    A([Inicio])

    B[/Leer marca, modelo, año y kilómetros/]

    C[combustible = (kilometros * 5) / 100]

    D[Mostrar datos]

    E[Mostrar combustible consumido]

    F([Fin])

    A --> B
    B --> C
    C --> D
    D --> E
    E --> F
```

---

# Prueba de Escritorio

| Kilómetros | Cálculo         | Combustible |
| ---------- | --------------- | ----------- |
| 100        | (100 × 5) / 100 | 5 L         |
| 200        | (200 × 5) / 100 | 10 L        |
| 350        | (350 × 5) / 100 | 17.5 L      |
| 500        | (500 × 5) / 100 | 25 L        |

---

# Implementación en C++

```cpp
#include <iostream>
#include <string>

using namespace std;

struct Motocicleta {

    string marca;
    string modelo;
    int anio;
    float kilometros;

};

int main() {

    Motocicleta moto;

    float combustible;

    cout << "Marca: ";
    cin >> moto.marca;

    cout << "Modelo: ";
    cin >> moto.modelo;

    cout << "Año: ";
    cin >> moto.anio;

    cout << "Kilometros recorridos: ";
    cin >> moto.kilometros;

    combustible = (moto.kilometros * 5) / 100;

    cout << "\n--- Datos de la motocicleta ---\n";

    cout << "Marca: " << moto.marca << endl;
    cout << "Modelo: " << moto.modelo << endl;
    cout << "Año: " << moto.anio << endl;
    cout << "Kilometros: " << moto.kilometros << endl;

    cout << "Combustible consumido: "
         << combustible << " litros" << endl;

    return 0;
}
```

---

# Ejemplo de Ejecución

```text
Marca: Yamaha
Modelo: FZ25
Año: 2022
Kilometros recorridos: 250

--- Datos de la motocicleta ---

Marca: Yamaha
Modelo: FZ25
Año: 2022
Kilometros: 250

Combustible consumido: 12.5 litros
```

---

# Observaciones

* Es un ejercicio secuencial, ya que no utiliza decisiones ni ciclos.
* Introduce el uso de estructuras (`struct`).
* Aplica una fórmula matemática simple mediante una regla de tres.
* Permite agrupar varios datos relacionados en una sola entidad.

---

# Temas Relacionados

* Variables y Tipos de Datos
* Estructuras (`struct`)
* Operadores Aritméticos
* Entrada y Salida
* Diagramas de Flujo
* Pruebas de Escritorio

---

# Resumen

| Concepto               | Aplicación                    |
| ---------------------- | ----------------------------- |
| struct                 | Agrupar datos                 |
| float                  | Kilómetros y combustible      |
| string                 | Marca y modelo                |
| Operadores aritméticos | Cálculo del consumo           |
| Secuencial             | Flujo principal del algoritmo |
