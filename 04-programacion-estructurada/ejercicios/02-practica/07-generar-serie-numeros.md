# Generar los n Primeros Términos de una Serie

## Enunciado

Construir un algoritmo que genere y almacene en un arreglo (**array**) los **n** primeros números de la siguiente serie:

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

# Análisis

## Entradas

| Dato | Tipo |
|------|------|
| n | Entero |

---

## Proceso

1. Solicitar la cantidad de términos.
2. Crear un arreglo de tamaño n.
3. Asignar el valor 1 al primer elemento.
4. Generar los siguientes términos multiplicando por 2 el término anterior.
5. Guardar cada término en el arreglo.
6. Mostrar la serie generada.

---

## Salidas

| Salida |
|---------|
| Serie generada |

---

## Restricciones

- La cantidad de términos debe ser mayor que 0.

---

# Casos de Prueba

| Entrada | Salida Esperada |
|----------|----------------|
| 3 | 1, 2, 4 |
| 5 | 1, 2, 4, 8, 16 |
| 7 | 1, 2, 4, 8, 16, 32, 64 |

---

# Estrategia de Solución

Se utilizará un arreglo para almacenar los términos de la serie.

El primer término será 1.

Cada término siguiente se obtendrá multiplicando por 2 el término anterior.

Finalmente se recorrerá el arreglo para mostrar todos los valores generados.

---

# Variables

| Variable | Tipo | Descripción |
|-----------|-----------|-----------|
| n | Entero | Cantidad de términos de la serie |
| i | Entero | Variable de control de los ciclos |
| serie[] | Array de Enteros | Almacena los términos de la serie |

---

# Operadores

| Operador | Tipo | Uso |
|-----------|-----------|-----------|
| = | Asignación | Asignar valores |
| * | Aritmético | Multiplicar por 2 |
| - | Aritmético | Acceder al término anterior |
| < | Relacional | Controlar los ciclos |
| ++ | Incremento | Avanzar posiciones |

---

# Estructuras Utilizadas

```text
Array

For
```

---

# Fórmulas

## Primer Término

```text
serie[0] = 1
```

## Generación de la Serie

```text
serie[i] = serie[i - 1] * 2
```

---

# Secuencia Lógica

1. Inicio.
2. Definir las variables:
   - n
   - i
   - serie[]
3. Solicitar la cantidad de términos.
4. Leer el valor de n.
5. Crear un array de tamaño n.
6. Asignar el valor 1 al primer elemento del array.
7. Recorrer el array desde la posición 1 hasta n - 1.
8. Generar cada término multiplicando por 2 el término anterior.
9. Guardar cada término en el array.
10. Recorrer el array para mostrar todos los términos.
11. Fin.

---

# Pseudocódigo

```text
Inicio

    Definir n Como Entero
    Definir i Como Entero

    Definir serie[] Como Array

    Escribir "Ingrese la cantidad de terminos: "
    Leer n

    serie[0] = 1

    for (i = 1; i < n; i++)
        serie[i] = serie[i - 1] * 2
    endfor

    Escribir "Serie generada: "
    for (i = 0; i < n; i++)
        Escribir serie[i]
    endfor

Fin
```

---

# Diagrama de Flujo

```mermaid
flowchart TD

A([Inicio])

B[/Leer n/]

C[serie[0] = 1]

D[i = 1]

E{i < n}

F[serie[i] = serie[i-1] * 2]

G[i++]

H[Mostrar serie]

I([Fin])

A --> B
B --> C
C --> D

D --> E

E -->|Sí| F
F --> G
G --> E

E -->|No| H
H --> I
```

---

# Prueba de Escritorio

## Caso 1

### Entrada

```text
n = 5
```

### Generación de la Serie

| i | serie[i] |
|---|---|
| 0 | 1 |
| 1 | 2 |
| 2 | 4 |
| 3 | 8 |
| 4 | 16 |

### Salida

```text
1, 2, 4, 8, 16
```

---

## Caso 2

### Entrada

```text
n = 7
```

### Generación de la Serie

| i | serie[i] |
|---|---|
| 0 | 1 |
| 1 | 2 |
| 2 | 4 |
| 3 | 8 |
| 4 | 16 |
| 5 | 32 |
| 6 | 64 |

### Salida

```text
1, 2, 4, 8, 16, 32, 64
```

---

# Implementación

```cpp
#include <iostream>

using namespace std;

int main() {

    int n;
    int i;

    cout << "Ingrese la cantidad de terminos: ";
    cin >> n;

    int serie[n];

    serie[0] = 1;

    for (i = 1; i < n; i++) {
        serie[i] = serie[i - 1] * 2;
    }

    cout << "Serie generada: ";
    for (i = 0; i < n; i++) {
        cout << serie[i];
        if (i < n - 1) {
            cout << ", ";
        }
    }

    cout << endl;

    return 0;
}
```
