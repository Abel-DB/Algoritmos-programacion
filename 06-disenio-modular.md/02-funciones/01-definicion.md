# Funciones

## Definición

Una función es un subprograma que realiza una tarea específica dentro de un programa.

Puede recibir datos mediante parámetros, ejecutar un conjunto de instrucciones y devolver un valor al programa que la invocó.

Las funciones permiten reutilizar código y dividir problemas complejos en tareas más pequeñas y fáciles de mantener.

---

## Características

Las funciones poseen las siguientes características:

- Poseen un nombre único.
- Pueden recibir uno o varios parámetros.
- Realizan una tarea específica.
- Devuelven un valor mediante una instrucción de retorno.
- Pueden ser invocadas desde diferentes partes del programa.

---

## Estructura general

```text
Funcion NombreFuncion(parametros)

    instrucciones

    Retornar resultado

FinFuncion
```

---

## Elementos de una función

### Nombre

Identifica a la función dentro del programa.

```text
Funcion Sumar()
```

### Parámetros

Son los datos que recibe la función para realizar una tarea.

```text
Funcion Sumar(a, b)
```

### Cuerpo

Es el conjunto de instrucciones que ejecuta la función.

```text
resultado <- a + b
```

### Valor de retorno

Es el resultado que la función devuelve al finalizar su ejecución.

```text
Retornar resultado
```

---

## Ejemplo

La siguiente función recibe dos números, realiza una suma y devuelve el resultado.

```text
Funcion Sumar(a, b)

    resultado <- a + b

    Retornar resultado

FinFuncion
```

Si la función recibe:

```text
a = 6
b = 8
```

entonces devolverá:

```text
14
```

---

## Importante

Una función se diferencia de un procedimiento porque devuelve un valor como resultado de su ejecución.

```text
edad <- CalcularEdad(fechaNacimiento)
```

En este caso, la función `CalcularEdad()` devuelve un valor que se almacena en la variable `edad`.

---

## Resumen

Una función es un subprograma que puede recibir datos, realizar un procesamiento y devolver un valor como resultado.

Las funciones favorecen la reutilización del código, mejoran la organización de los programas y facilitan su mantenimiento.
