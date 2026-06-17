# Calculadora Básica

## Enunciado

Construir un algoritmo que utilice funciones para realizar operaciones matemáticas básicas.

El programa deberá mostrar un menú de opciones, permitir al usuario seleccionar una operación y ejecutar el cálculo correspondiente mediante funciones.

El proceso se repetirá hasta que el usuario seleccione la opción de salir.

### Operaciones disponibles

1. Suma
2. Resta
3. Multiplicación
4. División
5. Salir

---

# Análisis

## Entradas

| Dato | Tipo |
|--------|--------|
| num1 | Real |
| num2 | Real |
| opcion | Entero |

---

## Proceso

1. Mostrar un menú de operaciones.
2. Permitir al usuario seleccionar una opción.
3. Solicitar los números necesarios.
4. Ejecutar la función correspondiente.
5. Mostrar el resultado.
6. Repetir el proceso hasta seleccionar salir.

---

## Salidas

| Salida |
|---------|
| Resultado de la operación |
| Mensajes de validación |
| Mensaje de salida |

---

## Restricciones

* No se puede dividir entre cero.
* La opción debe estar entre 1 y 5.

---

# Casos de Prueba

| Opción | num1 | num2 | Resultado |
|---------|---------|---------|---------|
| 1 | 10 | 5 | 15 |
| 2 | 10 | 5 | 5 |
| 3 | 10 | 5 | 50 |
| 4 | 10 | 5 | 2 |
| 4 | 10 | 0 | Error |

---

# Estrategia de Solución

Se utilizarán funciones independientes para cada operación matemática.

El programa mostrará un menú dentro de un ciclo repetitivo que permanecerá activo hasta que el usuario seleccione la opción salir.

Dependiendo de la opción seleccionada se llamará a la función correspondiente y se mostrará el resultado.

---

# Variables

| Variable | Tipo | Descripción |
|-----------|-----------|-----------|
| num1 | Real | Primer número ingresado |
| num2 | Real | Segundo número ingresado |
| resultado | Real | Resultado de la operación |
| opcion | Entero | Opción seleccionada |

---

# Operadores

| Operador | Tipo | Uso |
|-----------|-----------|-----------|
| + | Aritmético | Sumar |
| - | Aritmético | Restar |
| * | Aritmético | Multiplicar |
| / | Aritmético | Dividir |
| = | Asignación | Asignar valores |
| != | Relacional | Validar división |
| < | Relacional | Validar opciones |
| > | Relacional | Validar opciones |
| \|\| | Lógico | Verificar rango de opciones |

---

# Estructuras Utilizadas

```text
While
```

Permite mantener activo el menú hasta que el usuario decida salir.

```text
Switch
```

Permite seleccionar la operación matemática.

```text
If
```

Permite validar opciones y evitar divisiones entre cero.

```text
Funciones
```

Permiten modularizar el programa separando cada operación matemática en una función independiente.

---

# Fórmulas

### Suma

```text
resultado = a + b
```

### Resta

```text
resultado = a - b
```

### Multiplicación

```text
resultado = a * b
```

### División

```text
resultado = a / b
```

---

# Secuencia Lógica

1. Inicio.
2. Definir las funciones sumar, restar, multiplicar y dividir.
3. Definir las variables necesarias.
4. Mostrar el menú de opciones.
5. Leer la opción seleccionada.
6. Verificar si la opción es igual a 5.
7. Si la opción es 5, mostrar mensaje de salida y finalizar.
8. Verificar si la opción es válida.
9. Si la opción es inválida, mostrar mensaje de error.
10. Volver a mostrar el menú.
11. Solicitar el primer número.
12. Leer el primer número.
13. Solicitar el segundo número.
14. Leer el segundo número.
15. Evaluar la opción seleccionada.
16. Si la opción es 1, llamar a la función sumar.
17. Mostrar el resultado de la suma.
18. Si la opción es 2, llamar a la función restar.
19. Mostrar el resultado de la resta.
20. Si la opción es 3, llamar a la función multiplicar.
21. Mostrar el resultado de la multiplicación.
22. Si la opción es 4, verificar que el segundo número sea diferente de cero.
23. Si la división es válida, llamar a la función dividir.
24. Mostrar el resultado de la división.
25. Si el segundo número es cero, mostrar mensaje de error.
26. Volver al menú principal.
27. Repetir el proceso mientras el usuario no seleccione salir.
28. Fin.

---

# Pseudocódigo

```text
Funcion sumar(a, b)

    Retornar a + b

FinFuncion


Funcion restar(a, b)

    Retornar a - b

FinFuncion


Funcion multiplicar(a, b)

    Retornar a * b

FinFuncion


Funcion dividir(a, b)

    Retornar a / b

FinFuncion


Inicio

    Definir num1 Como Real
    Definir num2 Como Real
    Definir resultado Como Real

    Definir opcion Como Entero

    while (Verdadero)

        Escribir "===== MENU ====="
        Escribir "1. Sumar"
        Escribir "2. Restar"
        Escribir "3. Multiplicar"
        Escribir "4. Dividir"
        Escribir "5. Salir"

        Escribir "Ingrese una opcion: "
        Leer opcion

        if (opcion == 5) then
            Escribir "Saliendo del programa..."
            break
        endif

        if (opcion < 1 || opcion > 5) then
            Escribir "Opcion invalida"
            continue
        endif

        Escribir "Ingrese el primer numero: "
        Leer num1

        Escribir "Ingrese el segundo numero: "
        Leer num2

        switch (opcion)
            case 1:
                resultado = sumar(num1, num2)
                Escribir "Resultado: ", resultado
                break

            case 2:
                resultado = restar(num1, num2)
                Escribir "Resultado: ", resultado
                break

            case 3:
                resultado = multiplicar(num1, num2)
                Escribir "Resultado: ", resultado
                break

            case 4:
                if (num2 != 0) then
                    resultado = dividir(num1, num2)
                    Escribir "Resultado: ", resultado
                else
                    Escribir "No se puede dividir entre 0"
                endif
                break
        endswitch
    endwhile

Fin
```

---

# Prueba de Escritorio

## Caso 1

### Entrada

```text
num1 = 10
num2 = 5
opcion = 1
```

### Salida

```text
Resultado: 15
```

---

## Caso 2

### Entrada

```text
num1 = 20
num2 = 4
opcion = 4
```

### Salida

```text
Resultado: 5
```

---

## Caso 3

### Entrada

```text
num1 = 10
num2 = 0
opcion = 4
```

### Salida

```text
No se puede dividir entre 0
```

---

## Caso 4

### Entrada

```text
opcion = 8
```

### Salida

```text
Opcion invalida
```

---

## Caso 5

### Entrada

```text
opcion = 5
```

### Salida

```text
Saliendo del programa...
```

---

# Implementación

```cpp
#include <iostream>

using namespace std;

double sumar(double a, double b) {

    return a + b;

}

double restar(double a, double b) {

    return a - b;

}

double multiplicar(double a, double b) {

    return a * b;

}

double dividir(double a, double b) {

    return a / b;

}

int main() {

    double num1;
    double num2;
    double resultado;

    int opcion;

    while (true) {

        cout << "\n===== MENU =====" << endl;

        cout << "1. Sumar" << endl;
        cout << "2. Restar" << endl;
        cout << "3. Multiplicar" << endl;
        cout << "4. Dividir" << endl;
        cout << "5. Salir" << endl;

        cout << "\nIngrese una opcion: ";
        cin >> opcion;

        if (opcion == 5) {
            cout << "\nSaliendo del programa..." << endl;
            break;
        }

        if (opcion < 1 || opcion > 5) {
            cout << "\nOpcion invalida" << endl;
            continue;
        }

        cout << "\nIngrese el primer numero: ";
        cin >> num1;

        cout << "Ingrese el segundo numero: ";
        cin >> num2;

        switch (opcion) {
            case 1:
                resultado = sumar(num1, num2);
                cout << "\nResultado: " << resultado << endl;
                break;

            case 2:
                resultado = restar(num1, num2);
                cout << "\nResultado: " << resultado << endl;
                break;

            case 3:
                resultado = multiplicar(num1, num2);
                cout << "\nResultado: " << resultado << endl;
                break;

            case 4:
                if (num2 != 0) {
                    resultado = dividir(num1, num2);
                    cout << "\nResultado: " << resultado << endl;
                } else {
                    cout << "\nNo se puede dividir entre 0" << endl;
                }
                break;
        }
    }

    return 0;
}
```
