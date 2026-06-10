# Invertir un número y verificar si es capicúa

## Enunciado

Construir un algoritmo que pida al usuario un número entero **num**, invertir el número y verificar si es capicúa o no.

### Ejemplo

Si:

```text
num = 256
```

Mostrar:

```text
El numero invertido es: 652
El numero no es capicua
```

---

# Análisis del Problema

## Entradas

| Dato | Tipo   |
| ---- | ------ |
| num  | Entero |

## Proceso

1. Solicitar un número entero.
2. Leer el número ingresado.
3. Invertir el número.
4. Comparar el número original con el número invertido.
5. Determinar si es capicúa o no.
6. Mostrar los resultados.

## Salidas

| Salida                     |
| -------------------------- |
| Número invertido           |
| Indicar si es capicúa o no |

---

# Diseño de la Solución

## Secuencia lógica

1. Solicitar un número entero.
2. Leer el número ingresado.
3. Guardar una copia del número original.
4. Inicializar el número invertido en 0.
5. Obtener el último dígito del número.
6. Agregar el dígito al número invertido.
7. Eliminar el último dígito del número.
8. Repetir el proceso mientras el número sea mayor que 0.
9. Comparar el número original con el número invertido.
10. Determinar si el número es capicúa o no.
11. Mostrar el número invertido.
12. Mostrar si el número es capicúa o no.
13. Finalizar el algoritmo.

---

## Variables utilizadas

| Variable  | Tipo   | Descripción                     |
| --------- | ------ | ------------------------------- |
| num       | Entero | Número ingresado por el usuario |
| aux       | Entero | Copia del número original       |
| invertido | Entero | Número invertido                |
| digito    | Entero | Último dígito extraído          |

---

## Operadores utilizados

| Operador | Tipo       | Uso                           |
| -------- | ---------- | ----------------------------- |
| =        | Asignación | Asignar valores               |
| %        | Aritmético | Obtener el último dígito      |
| *        | Aritmético | Desplazar el número invertido |
| +        | Aritmético | Construir el número invertido |
| /        | Aritmético | Eliminar el último dígito     |
| ==       | Relacional | Verificar si es capicúa       |
| !=       | Relacional | Verificar si no es capicúa    |
| >        | Relacional | Controlar el ciclo            |

---

## Estructuras utilizadas

| Estructura              | Uso                            |
| ----------------------- | ------------------------------ |
| Secuencial              | Leer datos y realizar cálculos |
| Condicional (if - else) | Determinar si es capicúa       |
| Repetitiva (while)      | Invertir el número             |

---

## Fórmulas utilizadas

### Obtener último dígito

```text
digito = num % 10
```

### Construir el número invertido

```text
invertido = invertido * 10 + digito
```

### Eliminar último dígito

```text
num = num / 10
```

### Verificar si es capicúa

```text
aux == invertido
```

---

# Pseudocódigo

```text
INICIO

    Definir num, aux, invertido, digito Como Entero

    Escribir "Ingrese un numero: "
    Leer num

    aux = num

    invertido = 0

    While num > 0

        digito = num % 10

        invertido = invertido * 10 + digito

        num = num / 10

    EndWhile

    Escribir "El numero invertido es: ", invertido

    If aux == invertido

        Escribir "El numero es capicua"

    Else

        Escribir "El numero no es capicua"

    EndIf

FIN
```

---

# Prueba de Escritorio

## Caso 1

### Datos de entrada

```text
num = 123
```

### Seguimiento

| Vuelta  | num | digito | invertido |
| ------- | --- | ------ | --------- |
| Inicial | 123 | -      | 0         |
| 1       | 12  | 3      | 3         |
| 2       | 1   | 2      | 32        |
| 3       | 0   | 1      | 321       |

### Comparación

```text
123 == 321
```

Resultado:

```text
No es capicua
```

### Salida

```text
El numero invertido es: 321
El numero no es capicua
```

---

## Caso 2

### Datos de entrada

```text
num = 121
```

### Seguimiento

| Vuelta  | num | digito | invertido |
| ------- | --- | ------ | --------- |
| Inicial | 121 | -      | 0         |
| 1       | 12  | 1      | 1         |
| 2       | 1   | 2      | 12        |
| 3       | 0   | 1      | 121       |

### Comparación

```text
121 == 121
```

Resultado:

```text
Es capicua
```

### Salida

```text
El numero invertido es: 121
El numero es capicua
```

---

# Implementación en C++

```cpp
#include <iostream>

using namespace std;

int main() {
    int num, aux, invertido, digito;

    cout << "Ingrese un numero: ";
    cin >> num;

    aux = num;

    invertido = 0;

    while (num > 0) {
        digito = num % 10;
        invertido = invertido * 10 + digito;
        num = num / 10;
    }

    cout << "El numero invertido es: " << invertido << endl;

    if (aux == invertido) {
        cout << "El numero es capicua" << endl;
    } else {
        cout << "El numero no es capicua" << endl;
    }

    return 0;
}
```
