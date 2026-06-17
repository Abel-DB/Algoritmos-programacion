# Encontrar el Número Mayor de una Lista

## Enunciado

Construir un algoritmo que pida al usuario un número entero **n**, luego ingresar **n** números y mostrar el número mayor.

### Ejemplo

Si:

```text
n = 5
```

Ingresar:

```text
4
8
9
1
13
```

Mostrar:

```text
El numero mayor es 13
```

---

# Análisis

## Entradas

| Dato | Tipo |
|------|------|
| n | Entero |
| numeros[] | Array de Enteros |

---

## Proceso

1. Leer la cantidad de números.
2. Crear un array de tamaño n.
3. Ingresar los n números.
4. Inicializar la variable mayor con el primer elemento.
5. Recorrer el array desde la segunda posición.
6. Comparar cada elemento con mayor.
7. Actualizar mayor cuando corresponda.
8. Mostrar el número mayor.

---

## Salidas

| Salida |
|---------|
| Número mayor |

---

## Restricciones

- La cantidad de números debe ser mayor que 0.
- Los datos ingresados deben ser números enteros.

---

# Casos de Prueba

| Entrada | Salida Esperada |
|----------|----------------|
| 8, 3, 12, 7, 5 | El numero mayor es 12 |
| 10, 25, 4, 9 | El numero mayor es 25 |
| -5, -2, -10, -1 | El numero mayor es -1 |
| 7 | El numero mayor es 7 |

---

# Estrategia de Solución

Se utilizará un array para almacenar los números ingresados.

Posteriormente se inicializará la variable mayor con el primer elemento del array.

Luego se recorrerá el array comparando cada elemento con la variable mayor.

Si se encuentra un valor más grande, la variable mayor será actualizada.

Finalmente se mostrará el número mayor encontrado.

---

# Variables

| Variable | Tipo | Descripción |
|-----------|-----------|-----------|
| n | Entero | Cantidad de números |
| i | Entero | Control del ciclo |
| mayor | Entero | Almacena el número mayor |
| numeros[] | Array de Enteros | Guarda los números ingresados |

---

# Operadores

| Operador | Tipo | Uso |
|-----------|-----------|-----------|
| = | Asignación | Asignar valores |
| > | Relacional | Comparar números |
| < | Relacional | Controlar el ciclo |
| ++ | Incremento | Avanzar posiciones |

---

# Estructuras Utilizadas

```text
For

If
```

---

# Fórmulas

## Inicialización del Mayor

```text
mayor = numeros[0]
```

## Comparación

```text
numeros[i] > mayor
```

## Actualización

```text
mayor = numeros[i]
```

---

# Secuencia Lógica

1. Inicio.
2. Definir las variables:
   - n
   - i
   - mayor
   - numeros[]
3. Solicitar la cantidad de números.
4. Leer el valor de n.
5. Ingresar los n números y almacenarlos en el array.
6. Inicializar la variable mayor con el primer elemento del array.
7. Recorrer el array desde la segunda posición.
8. Comparar cada elemento con la variable mayor.
9. Si el elemento es mayor, actualizar la variable mayor.
10. Mostrar el número mayor.
11. Fin.

---

# Pseudocódigo

```text
Inicio

    Definir n Como Entero
    Definir i Como Entero
    Definir mayor Como Entero

    Definir numeros[] Como Array

    Escribir "Ingrese la cantidad de numeros: "
    Leer n

    for (i = 0; i < n; i++)
        Escribir "Ingrese el numero ", i + 1, ": "
        Leer numeros[i]
    endfor

    mayor = numeros[0]

    for (i = 1; i < n; i++)
        if (numeros[i] > mayor) then
            mayor = numeros[i]
        endif
    endfor

    Escribir "El numero mayor es ", mayor

Fin
```

---

# Diagrama de Flujo

```mermaid
flowchart TD

A([Inicio])

B[/Leer cantidad de numeros/]

C[/Ingresar numeros en el array/]

D[mayor = numeros[0]]

E[Recorrer array]

F{numeros[i] > mayor}

G[Actualizar mayor]

H[Mostrar mayor]

I([Fin])

A --> B
B --> C
C --> D
D --> E

E --> F

F -->|Sí| G
G --> E

F -->|No| E

E --> H

H --> I
```

---

# Prueba de Escritorio

## Caso 1

### Entrada

```text
n = 5

numeros = [8, 3, 12, 7, 5]
```

### Carga del Array

| i | numeros[i] |
|---|------------|
| 0 | 8 |
| 1 | 3 |
| 2 | 12 |
| 3 | 7 |
| 4 | 5 |

### Búsqueda del Mayor

| i | numeros[i] | mayor |
|---|------------|-------|
| Inicial | 8 | 8 |
| 1 | 3 | 8 |
| 2 | 12 | 12 |
| 3 | 7 | 12 |
| 4 | 5 | 12 |

### Salida

```text
El numero mayor es 12
```

---

## Caso 2

### Entrada

```text
n = 4

numeros = [-5, -2, -10, -1]
```

### Búsqueda del Mayor

| i | numeros[i] | mayor |
|---|------------|-------|
| Inicial | -5 | -5 |
| 1 | -2 | -2 |
| 2 | -10 | -2 |
| 3 | -1 | -1 |

### Salida

```text
El numero mayor es -1
```

---

# Implementación

```cpp
#include <iostream>

using namespace std;

int main() {

    int n;
    int i;
    int mayor;

    cout << "Ingrese la cantidad de numeros: ";
    cin >> n;

    int numeros[n];

    for (i = 0; i < n; i++) {
        cout << "Ingrese el numero " << i + 1 << ": ";
        cin >> numeros[i];
    }

    mayor = numeros[0];

    for (i = 1; i < n; i++) {
        if (numeros[i] > mayor) {
            mayor = numeros[i];
        }
    }

    cout << "El numero mayor es " << mayor << endl;

    return 0;
}
```
