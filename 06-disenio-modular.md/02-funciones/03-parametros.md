# Parámetros en las Funciones

## ¿Qué son los parámetros?

Los parámetros son datos que una función recibe para poder realizar una tarea específica.

Permiten que una misma función pueda trabajar con diferentes valores sin necesidad de modificar su código.

---

## ¿Para qué sirven?

Los parámetros permiten:

- Enviar información a una función.
- Reutilizar una función con distintos datos.
- Evitar la repetición de código.
- Hacer que los programas sean más flexibles.

---

## Sintaxis general

```text
Funcion NombreFuncion(parametro1, parametro2, ...)

    instrucciones

    Retornar resultado

FinFuncion
```

Los parámetros se escriben entre paréntesis después del nombre de la función.

---

## Función sin parámetros

Una función no está obligada a recibir parámetros.

### Ejemplo

```text
Funcion MostrarMensaje()

    Retornar "Bienvenido"

FinFuncion
```

En este caso, la función siempre devolverá el mismo resultado.

---

## Función con un parámetro

Una función puede recibir un único dato.

### Ejemplo

```text
Funcion Cuadrado(numero)

    Retornar numero * numero

FinFuncion
```

Si:

```text
Cuadrado(4)
```

La función devolverá:

```text
16
```

---

## Función con varios parámetros

Una función también puede recibir varios datos.

### Ejemplo

```text
Funcion Sumar(a, b)

    Retornar a + b

FinFuncion
```

Si:

```text
Sumar(5, 3)
```

La función devolverá:

```text
8
```

---

## Correspondencia de parámetros

Cuando se invoca una función, los valores enviados deben respetar el orden de los parámetros definidos.

### Declaración

```text
Funcion Restar(a, b)

    Retornar a - b

FinFuncion
```

### Llamada

```text
Restar(10, 4)
```

Resultado:

```text
6
```

En este caso:

- `10` corresponde a `a`.
- `4` corresponde a `b`.

---

## Importancia de los parámetros

Los parámetros permiten que una misma función pueda utilizarse en múltiples situaciones.

Por ejemplo, la función:

```text
Funcion Sumar(a, b)
```

puede utilizarse para sumar cualquier par de números sin necesidad de crear una función diferente para cada caso.

---

## Resumen

Los parámetros son datos que una función recibe para realizar una tarea específica.

Gracias a ellos, las funciones pueden reutilizarse con distintos valores, haciendo que los programas sean más flexibles y fáciles de mantener.
