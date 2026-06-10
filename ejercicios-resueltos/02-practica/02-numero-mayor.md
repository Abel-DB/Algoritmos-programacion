# Encontrar el número mayor de una lista

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

# Análisis del Problema

## Entradas

| Dato      | Tipo             |
| --------- | ---------------- |
| n         | Entero           |
| numeros[] | Tabla de enteros |

## Proceso

1. Leer la cantidad de números a ingresar.
2. Crear una tabla de tamaño n.
3. Ingresar y almacenar los n números en la tabla.
4. Inicializar la variable mayor con el primer elemento de la tabla.
5. Recorrer la tabla comparando cada elemento con mayor.
6. Actualizar mayor cuando se encuentre un número más grande.
7. Mostrar el número mayor.

## Salidas

| Salida       |
| ------------ |
| Número mayor |

---

# Diseño de la Solución

## Secuencia lógica

1. Solicitar la cantidad de números.
2. Leer el valor de n.
3. Crear una tabla de tamaño n.
4. Ingresar los n números en la tabla.
5. Inicializar la variable mayor con el primer elemento de la tabla.
6. Recorrer la tabla desde la segunda posición.
7. Comparar cada elemento con la variable mayor.
8. Si el elemento es mayor, actualizar la variable mayor.
9. Mostrar el número mayor.

---

## Variables utilizadas

| Variable  | Tipo             | Descripción                    |
| --------- | ---------------- | ------------------------------ |
| n         | Entero           | Cantidad de números            |
| i         | Entero           | Control del ciclo              |
| aux       | Entero           | Número ingresado temporalmente |
| mayor     | Entero           | Almacena el número mayor       |
| numeros[] | Tabla de enteros | Guarda los números ingresados  |

---

## Operadores utilizados

| Operador | Tipo       | Uso                              |
| -------- | ---------- | -------------------------------- |
| =        | Asignación | Asignar valores                  |
| >        | Relacional | Comparar números                 |
| <        | Relacional | Controlar el recorrido del ciclo |
| ++       | Incremento | Avanzar posiciones               |

---

## Estructuras utilizadas

| Estructura              | Uso                             |
| ----------------------- | ------------------------------- |
| Secuencial              | Ejecutar instrucciones en orden |
| Condicional simple (if) | Comparar números                |
| Repetitiva (for)        | Recorrer la tabla               |

---

## Fórmulas utilizadas

### Inicialización del mayor

```text
mayor = numeros[0]
```

### Comparación del mayor

```text
numeros[i] > mayor
```

### Actualización del mayor

```text
mayor = numeros[i]
```

---

# Pseudocódigo

```text
INICIO

    Definir n, i, aux, mayor Como Entero
    Definir numeros[] Como Array

    Escribir "Ingrese la cantidad de numeros:"
    Leer n

    For i = 0; i < n; i++

        Escribir "Ingrese el numero ", i + 1
        Leer aux

        numeros[i] = aux

    EndFor

    mayor = numeros[0]

    For i = 1; i < n; i++

        If numeros[i] > mayor Then

            mayor = numeros[i]

        EndIf

    EndFor

    Mostrar "El numero mayor es ", mayor

FIN
```

---

# Prueba de Escritorio

## Caso 1

### Datos de entrada

```text
n = 5
```

Números ingresados:

```text
[4, 8, 9, 1, 13]
```

### Seguimiento

| i       | numeros[i] | mayor |
| ------- | ---------- | ----- |
| Inicial | 4          | 4     |
| 1       | 8          | 8     |
| 2       | 9          | 9     |
| 3       | 1          | 9     |
| 4       | 13         | 13    |

### Resultado

```text
El numero mayor es 13
```

---

## Caso 2

### Datos de entrada

```text
n = 4
```

Números ingresados:

```text
[7, 3, 2, 5]
```

### Seguimiento

| i       | numeros[i] | mayor |
| ------- | ---------- | ----- |
| Inicial | 7          | 7     |
| 1       | 3          | 7     |
| 2       | 2          | 7     |
| 3       | 5          | 7     |

### Resultado

```text
El numero mayor es 7
```

---

# Implementación en C++

```cpp
#include <iostream>

using namespace std;

int main() {
  int n, i, aux, mayor;

  cout << "Ingrese la cantidad de numeros: ";
  cin >> n;

  int numeros[n];

  for (i = 0; i < n; i++) {
    cout << "Ingrese el numero " << i + 1 << ": ";
    cin >> aux;

    numeros[i] = aux;
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
