# Factores Primos de un Número

## Enunciado

Construir un algoritmo que pida al usuario un número entero **n**, calcular, almacenar en un arreglo (**array**) y mostrar sus factores primos.

### Ejemplo

Si:

```text
n = 28
```

Mostrar:

```text
2, 2, 7
```

Porque:

```text
28 = 2 × 2 × 7
```

---

# Análisis

## Entradas

| Dato | Tipo |
|------|------|
| n | Entero |

---

## Proceso

1. Leer un número entero.
2. Crear un array para almacenar los factores primos.
3. Inicializar el divisor en 2.
4. Buscar divisores exactos.
5. Guardar cada factor primo encontrado.
6. Reducir el número dividiéndolo por el factor encontrado.
7. Continuar hasta que el número sea igual a 1.
8. Mostrar los factores almacenados.

---

## Salidas

| Salida |
|---------|
| Factores primos del número |

---

## Restricciones

- El número debe ser mayor que 1.

---

# Casos de Prueba

| Entrada | Salida Esperada |
|----------|----------------|
| 12 | 2, 2, 3 |
| 18 | 2, 3, 3 |
| 28 | 2, 2, 7 |
| 45 | 3, 3, 5 |

---

# Estrategia de Solución

Se utilizará un divisor que inicialmente tendrá el valor 2.

Mientras el número sea diferente de 1, se verificará si es divisible por el divisor actual.

Si es divisible, el divisor se almacenará como factor primo y el número se reducirá mediante una división.

Si no es divisible, se incrementará el divisor.

Todos los factores encontrados se almacenarán en un array para mostrarlos posteriormente.

---

# Variables

| Variable | Tipo | Descripción |
|-----------|-----------|-----------|
| n | Entero | Número ingresado por el usuario |
| divisor | Entero | Posible factor primo |
| i | Entero | Índice para almacenar factores |
| j | Entero | Índice para mostrar factores |
| factores[] | Array de Enteros | Almacena los factores primos |

---

# Operadores

| Operador | Tipo | Uso |
|-----------|-----------|-----------|
| = | Asignación | Asignar valores |
| % | Aritmético | Verificar divisibilidad |
| / | Aritmético | Reducir el número |
| == | Relacional | Comparar igualdad |
| != | Relacional | Controlar el ciclo |
| < | Relacional | Controlar el ciclo for |
| ++ | Incremento | Avanzar índices |

---

# Estructuras Utilizadas

```text
Array

If Else

While

For
```

---

# Fórmulas

## Verificación de Divisibilidad

```text
n % divisor == 0
```

## Reducción del Número

```text
n = n / divisor
```

---

# Secuencia Lógica

1. Inicio.
2. Definir las variables:
   - n
   - divisor
   - i
   - j
   - factores[]
3. Solicitar un número entero.
4. Leer el valor de n.
5. Crear un array de tamaño n.
6. Inicializar divisor en 2.
7. Inicializar i en 0.
8. Mientras n sea diferente de 1:
   - Verificar si n es divisible por divisor.
   - Si es divisible:
     - Guardar divisor en el array.
     - Incrementar i.
     - Dividir n entre divisor.
   - Caso contrario:
     - Incrementar divisor.
9. Mostrar los factores almacenados.
10. Fin.

---

# Pseudocódigo

```text
Inicio

    Definir n Como Entero
    Definir divisor Como Entero
    Definir i Como Entero
    Definir j Como Entero

    Definir factores[] Como Array

    Escribir "Ingrese un numero: "
    Leer n

    divisor = 2
    i = 0

    while (n != 1)
        if (n % divisor == 0) then
            factores[i] = divisor
            i++
            n = n / divisor
        else
            divisor++
        endif
    endwhile

    Escribir "Factores primos: "

    for (j = 0; j < i; j++)
        Escribir factores[j]
    endfor

Fin
```

---

# Diagrama de Flujo

```mermaid
flowchart TD

A([Inicio])

B[/Leer n/]

C[divisor = 2<br>i = 0]

D{n != 1}

E{n % divisor == 0}

F[factores[i] = divisor<br>i++<br>n = n / divisor]

G[divisor++]

H[Mostrar factores]

I([Fin])

A --> B
B --> C
C --> D

D -->|Sí| E

E -->|Sí| F
E -->|No| G

F --> D
G --> D

D -->|No| H
H --> I
```

---

# Prueba de Escritorio

## Caso 1

### Entrada

```text
n = 12
```

### Seguimiento

| Vuelta | n | divisor | Factor Guardado |
|---------|---------|---------|---------|
| 1 | 12 | 2 | 2 |
| 2 | 6 | 2 | 2 |
| 3 | 3 | 2 | - |
| 4 | 3 | 3 | 3 |

### Factores

```text
[2, 2, 3]
```

### Salida

```text
2, 2, 3
```

---

## Caso 2

### Entrada

```text
n = 28
```

### Seguimiento

| Vuelta | n | divisor | Factor Guardado |
|---------|---------|---------|---------|
| 1 | 28 | 2 | 2 |
| 2 | 14 | 2 | 2 |
| 3 | 7 | 2 | - |
| 4 | 7 | 3 | - |
| 5 | 7 | 4 | - |
| 6 | 7 | 5 | - |
| 7 | 7 | 6 | - |
| 8 | 7 | 7 | 7 |

### Factores

```text
[2, 2, 7]
```

### Salida

```text
2, 2, 7
```

---

# Implementación

```cpp
#include <iostream>

using namespace std;

int main() {

    int n;
    int divisor;
    int i;
    int j;

    cout << "Ingrese un numero: ";
    cin >> n;

    int factores[n];

    divisor = 2;
    i = 0;

    while (n != 1) {
        if (n % divisor == 0) {
            factores[i] = divisor;
            i++;
            n = n / divisor;
        } else {
            divisor++;
        }
    }

    cout << "Factores primos: ";

    for (j = 0; j < i; j++) {
        cout << factores[j];
        if (j < i - 1) {
            cout << ", ";
        }
    }

    cout << endl;

    return 0;
}
```
