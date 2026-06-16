# Funciones

## Definición

Una función es un subprograma que realiza una tarea específica dentro de un programa.

Recibe datos mediante parámetros, ejecuta un conjunto de instrucciones y devuelve un único resultado al programa que la invocó.

Las funciones permiten reutilizar código y dividir problemas complejos en tareas más pequeñas y fáciles de mantener.

---

## Características

- Poseen un nombre único.
- Pueden recibir uno o varios parámetros.
- Realizan una tarea específica.
- Devuelven un único valor mediante una instrucción de retorno.
- Pueden ser invocadas desde cualquier parte del programa.

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

Son los datos que recibe la función para realizar su tarea.

```text
Funcion Sumar(a, b)
```

### Cuerpo

Conjunto de instrucciones que ejecuta la función.

```text
resultado <- a + b
```

### Valor de retorno

Resultado que devuelve la función al finalizar su ejecución.

```text
Retornar resultado
```

---

## Ejemplo

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

## Ventajas de utilizar funciones

- Evitan la repetición de código.
- Facilitan el mantenimiento.
- Mejoran la organización del programa.
- Permiten reutilizar soluciones.
- Hacen más legible el código.

---

## Resumen

Una función es un subprograma que recibe datos, realiza un procesamiento y devuelve un único resultado. Su principal objetivo es reutilizar código y dividir problemas complejos en tareas más pequeñas.
