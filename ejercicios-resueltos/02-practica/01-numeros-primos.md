# Determinar si un número es primo

## Enunciado

Construir un algoritmo que solicite al usuario un número entero n y determine si es primo.

### Ejemplo

Si:

```text
n = 29
```

Mostrar:

```text
El número 29 es primo
```

Si:

```text
n = 28
```

Mostrar:

```text
El número 28 no es primo
```

---

# Análisis del Problema

## Entradas

| Dato | Tipo   |
| ---- | ------ |
| n    | Entero |

## Proceso

1. Leer un número entero.
2. Verificar si el número es mayor que 1.
3. Revisar los posibles divisores desde 2 hasta n − 1.
4. Determinar si existe algún divisor exacto.
5. Si existe un divisor exacto, el número no es primo.
6. Si no existe ningún divisor exacto, el número es primo.

## Salidas

| Salida                |
| --------------------- |
| El número es primo    |
| El número no es primo |

---

# Diseño de la Solución

## Secuencia lógica

1. Solicitar un número entero.
2. Leer el número ingresado.
3. Inicializar la variable esPrimo en verdadero.
4. Verificar si el número es menor o igual a 1.
5. Recorrer los divisores desde 2 hasta n − 1.
6. Verificar si existe algún divisor exacto.
7. Si existe, cambiar esPrimo a falso.
8. Mostrar el resultado.

---

## Variables utilizadas

| Variable | Tipo     | Descripción                     |
| -------- | -------- | ------------------------------- |
| n        | Entero   | Número ingresado por el usuario |
| divisor  | Entero   | Posible divisor del número      |
| es_primo  | Booleano | Indica si el número es primo    |

---

## Operadores utilizados

| Operador | Tipo       | Uso                                 |
| -------- | ---------- | ----------------------------------- |
| %        | Aritmético | Obtener residuo                     |
| ==       | Relacional | Comparar igualdad                   |
| <=       | Relacional | Verificar si n es menor o igual a 1 |
| =        | Asignación | Asignar valores                     |
| ++       | Incremento | Avanzar divisores                   |

---

## Estructuras utilizadas

| Estructura       | Uso                             |
| ---------------- | ------------------------------- |
| Secuencial       | Ejecutar instrucciones en orden |
| Condicional (if) | Verificar divisibilidad         |
| Repetitiva (for) | Recorrer divisores              |

---

## Fórmulas utilizadas

### Verificación de divisibilidad

```text
n % divisor == 0
```

---

# Pseudocódigo

```text
INICIO

    Definir n, divisor Como Entero
    Definir es_primo Como Booleano

    es_primo = True

    Escribir "Ingrese un numero entero:"
    Leer n

    If (n <= 1) Then
        esPrimo = False
    End If

    For (divisor = 2; divisor < n; divisor++)

        If (n % divisor == 0) Then
            es_primo = False
            Break
        End If

    End For

    If (es_primo) Then
        Mostrar "El numero ", n, " es primo"
    Else
        Mostrar "El numero ", n, " no es primo"
    End If

FIN
```

---

# Prueba de Escritorio

## Caso 1

### Datos de entrada

```text
n = 7
```

### Seguimiento

| Paso          | divisor | n | n % divisor | es_primo  |
| ------------- | ------- | - | ----------- | --------- |
| Inicial       | -       | 7 | -           | True      |
| n <= 1 ?      | -       | 7 | -           | True      |
| Iteración 1   | 2       | 7 | 1           | True      |
| Iteración 2   | 3       | 7 | 1           | True      |
| Iteración 3   | 4       | 7 | 3           | True      |
| Iteración 4   | 5       | 7 | 2           | True      |
| Iteración 5   | 6       | 7 | 1           | True      |
| Fin del ciclo | -       | 7 | -           | True      |

### Resultado

```text
El numero 7 es primo
```

---

## Caso 2

### Datos de entrada

```text
n = 8
```

### Seguimiento

| Paso        | divisor | n | n % divisor | es_primo  |
| ----------- | ------- | - | ----------- | --------- |
| Inicial     | -       | 8 | -           | True      |
| n <= 1 ?    | -       | 8 | -           | True      |
| Iteración 1 | 2       | 8 | 0           | False     |
| Break       | -       | 8 | -           | False     |

### Resultado

```text
El numero 8 no es primo
```

---

## Caso 3

### Datos de entrada

```text
n = 1
```

### Seguimiento


| Paso              | divisor | n | es_primo  |
| ----------------- | ------- | - | --------- |
| Inicial           | -       | 1 | True      |
| n <= 1            | -       | 1 | False     |
| No entra al ciclo | -       | 1 | False     |


### Resultado

```text
El numero 1 no es primo
```

# Implementacion en C++

```cpp
#include <iostream>

using namespace std;

int main() {
    int n;
    int divisor;
    bool es_primo;

    es_primo = true;

    cout << "Ingrese un numero entero: ";
    cin >> n;

    if (n <= 1) {
        esPrimo = false;
    }

    for (divisor = 2; divisor < n; divisor++) {
        if (n % divisor == 0) {
            esPrimo = false;
            break;
        }
    }

    if (es_primo) {
        cout << "El numero " << n << " es primo";
    } else {
        cout << "El numero " << n << " no es primo";
    }

    return 0;
}
```
