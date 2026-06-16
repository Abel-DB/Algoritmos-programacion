# Retorno de Funciones

## ¿Qué es el retorno de una función?

El retorno es el valor que una función devuelve al programa que la invocó una vez que ha finalizado su ejecución.

Gracias al retorno, una función puede entregar el resultado de un procesamiento para que sea utilizado en otras partes del programa.

---

## Instrucción de retorno

La devolución de un valor se realiza mediante la instrucción:

```text
Retornar
```

Su sintaxis general es:

```text
Retornar valor
```

---

## Estructura general

```text
Funcion NombreFuncion(parametros)

    instrucciones

    Retornar resultado

FinFuncion
```

Cuando se ejecuta la instrucción `Retornar`, la función finaliza y envía el valor indicado al programa que realizó la llamada.

---

## Ejemplo

```text
Funcion Sumar(a, b)

    resultado <- a + b

    Retornar resultado

FinFuncion
```

Si:

```text
Sumar(6, 8)
```

La función devolverá:

```text
14
```

---

## Retorno de una expresión

No siempre es necesario almacenar el resultado en una variable.

También es posible retornar directamente una expresión.

### Ejemplo

```text
Funcion Sumar(a, b)

    Retornar a + b

FinFuncion
```

Si:

```text
Sumar(6, 8)
```

La función devolverá:

```text
14
```

---

## Uso del valor retornado

El valor devuelto por una función puede almacenarse en una variable.

### Ejemplo

```text
resultado <- Sumar(6, 8)
```

Después de la ejecución:

```text
resultado = 14
```

---

## Importancia del retorno

El retorno permite:

- Obtener resultados de una función.
- Reutilizar cálculos en diferentes partes del programa.
- Evitar la repetición de código.
- Facilitar la organización del programa.

---

## Consideraciones

- Una función devuelve un único valor.
- La instrucción `Retornar` finaliza la ejecución de la función.
- El valor retornado puede ser almacenado o utilizado directamente.
- No todas las funciones necesitan recibir parámetros para retornar un resultado.

### Ejemplo

```text
Funcion ObtenerPI()

    Retornar 3.1416

FinFuncion
```

La función no recibe parámetros, pero devuelve un valor.

---

## Resumen

El retorno es el mecanismo mediante el cual una función devuelve un valor al programa que la invocó.

La instrucción `Retornar` permite entregar el resultado de un procesamiento para que pueda utilizarse posteriormente en otras partes del programa.
