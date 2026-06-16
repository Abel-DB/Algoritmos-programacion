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

### Ejemplo

Si:

```text
num1 = 10
num2 = 5
opcion = 1
```

Mostrar:

```text
Resultado: 15
```

---

# Análisis del Problema

## Entradas

| Dato   | Tipo   |
| ------ | ------ |
| num1   | Real   |
| num2   | Real   |
| opcion | Entero |

## Proceso

1. Mostrar un menú de operaciones.
2. Permitir al usuario seleccionar una opción.
3. Solicitar los números necesarios para realizar la operación.
4. Ejecutar la operación seleccionada mediante una función.
5. Mostrar el resultado obtenido.
6. Repetir el proceso hasta que el usuario decida salir.

## Salidas

| Salida                                 |
| -------------------------------------- |
| Resultado de la operación seleccionada |
| Mensajes de validación                 |
| Mensaje de salida                      |

---

# Diseño de la Solución

## Secuencia lógica

1. Declarar las funciones Sumar, Restar, Multiplicar y Dividir.
2. Mostrar el menú de opciones.
3. Leer la opción seleccionada.
4. Si la opción es 5, finalizar el programa.
5. Verificar que la opción ingresada sea válida.
6. Solicitar el primer número.
7. Solicitar el segundo número.
8. Evaluar la opción mediante una estructura switch.
9. Si la opción es 1, llamar a la función Sumar.
10. Si la opción es 2, llamar a la función Restar.
11. Si la opción es 3, llamar a la función Multiplicar.
12. Si la opción es 4, verificar que el segundo número sea diferente de cero.
13. Si la división es válida, llamar a la función Dividir.
14. Mostrar el resultado obtenido.
15. Regresar al menú principal.
16. Repetir el proceso hasta que el usuario seleccione la opción Salir.

---

## Variables utilizadas

| Variable  | Tipo   | Descripción                              |
| --------- | ------ | ---------------------------------------- |
| num1      | Real   | Primer número ingresado                  |
| num2      | Real   | Segundo número ingresado                 |
| resultado | Real   | Resultado de la operación                |
| opcion    | Entero | Opción seleccionada en el menú principal |

---

## Operadores utilizados

| Operador | Tipo       | Uso                         |
| -------- | ---------- | --------------------------- |
| +        | Aritmético | Suma                        |
| -        | Aritmético | Resta                       |
| *        | Aritmético | Multiplicación              |
| /        | Aritmético | División                    |
| =        | Asignación | Asignar valores             |
| !=       | Relacional | Validar división            |
| <        | Relacional | Validar opciones            |
| >        | Relacional | Validar opciones            |
| ||       | Lógico     | Verificar rango de opciones |

---

## Estructuras utilizadas

| Estructura         | Uso                                    |
| ------------------ | -------------------------------------- |
| Secuencial         | Lectura y visualización de datos       |
| Repetitiva (while) | Mantener activo el menú                |
| Selectiva (switch) | Seleccionar la operación               |
| Condicional (if)   | Validar opciones y división entre cero |
| Funciones          | Realizar los cálculos                  |

---

## Fórmulas utilizadas

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

# Pseudocódigo

```text
Funcion Sumar(a, b)

    resultado = a + b

    Return resultado

FinFuncion


Funcion Restar(a, b)

    resultado = a - b

    Return resultado

FinFuncion


Funcion Multiplicar(a, b)

    resultado = a * b

    Return resultado

FinFuncion


Funcion Dividir(a, b)

    resultado = a / b

    Return resultado

FinFuncion


Algoritmo Calculadora

    Definir num1, num2, resultado Como Real
    Definir opcion Como Entero

    While (Verdadero)

        Escribir "===== MENU ====="
        Escribir "1. Sumar"
        Escribir "2. Restar"
        Escribir "3. Multiplicar"
        Escribir "4. Dividir"
        Escribir "5. Salir"

        Escribir "Ingrese la opcion:"
        Leer opcion

        If (opcion == 5) Then

            Escribir "Saliendo del programa..."

            Break

        EndIf

        If (opcion < 1 || opcion > 5) Then

            Escribir "Opcion invalida."

            Continue

        EndIf

        Escribir "Ingrese el primer numero:"
        Leer num1

        Escribir "Ingrese el segundo numero:"
        Leer num2

        Switch(opcion)

            Case 1:

                resultado = Sumar(num1, num2)

                Escribir "Resultado: ", resultado

            Case 2:

                resultado = Restar(num1, num2)

                Escribir "Resultado: ", resultado

            Case 3:

                resultado = Multiplicar(num1, num2)

                Escribir "Resultado: ", resultado

            Case 4:

                If (num2 != 0) Then

                    resultado = Dividir(num1, num2)

                    Escribir "Resultado: ", resultado

                Else

                    Escribir "No se puede dividir entre 0."

                EndIf

        EndSwitch

    EndWhile

FinAlgoritmo
```

---

# Prueba de Escritorio

## Caso 1: Suma

### Datos de entrada

```text
num1 = 10
num2 = 5
opcion = 1
```

### Resultado

```text
Resultado: 15
```

---

## Caso 2: División

### Datos de entrada

```text
num1 = 20
num2 = 4
opcion = 4
```

### Resultado

```text
Resultado: 5
```

---

## Caso 3: División entre cero

### Datos de entrada

```text
num1 = 10
num2 = 0
opcion = 4
```

### Resultado

```text
No se puede dividir entre 0.
```

---

## Caso 4: Opción inválida

### Datos de entrada

```text
opcion = 8
```

### Resultado

```text
Opcion invalida.
```

---

## Caso 5: Salir del programa

### Datos de entrada

```text
opcion = 5
```

### Resultado

```text
Saliendo del programa...
```

---

# Implementación en C++

```cpp
#include <iostream>

using namespace std;

double Sumar(double a, double b) {
  double resultado = a + b;
  return resultado;
}

double Restar(double a, double b) {
  double resultado = a - b;
  return resultado;
}

double Multiplicar(double a, double b) {
  double resultado = a * b;
  return resultado;
}

double Dividir(double a, double b) {
  double resultado = a / b;
  return resultado;
}

int main() {
  double num1, num2, resultado;
  int opcion;

  while (true) {
    cout << "\n===== MENU =====" << endl;
    cout << "1. Sumar" << endl;
    cout << "2. Restar" << endl;
    cout << "3. Multiplicar" << endl;
    cout << "4. Dividir" << endl;
    cout << "5. Salir" << endl;

    cout << "\nIngrese la opcion: ";
    cin >> opcion;

    if (opcion == 5) {
      cout << "\nSaliendo del programa..." << endl;
      break;
    }

    if (opcion < 1 || opcion > 5) {
      cout << "\nOpcion invalida." << endl;
      continue;
    }

    cout << "\nIngrese el primer numero: ";
    cin >> num1;

    cout << "Ingrese el segundo numero: ";
    cin >> num2;

    switch (opcion) {
      case 1:
        resultado = Sumar(num1, num2);
        cout << "\nResultado: " << resultado << endl;
        break;
      case 2:
        resultado = Restar(num1, num2);
        cout << "\nResultado: " << resultado << endl;
        break;
      case 3:
        resultado = Multiplicar(num1, num2);
        cout << "\nResultado: " << resultado << endl;
        break;
      case 4:
        if (num2 != 0) {
          resultado = Dividir(num1, num2);
          cout << "\nResultado: " << resultado << endl;
        } else {
          cout << "\nNo se puede dividir entre 0." << endl;
        }
        break;
    }
  }
}
```
