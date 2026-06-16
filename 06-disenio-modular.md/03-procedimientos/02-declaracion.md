# Declaración de Procedimientos

## ¿Qué es la declaración de un procedimiento?

La declaración es la definición formal de un procedimiento dentro de un programa.

En ella se especifican:

- El nombre del procedimiento.
- Los parámetros que recibirá.
- Las instrucciones que ejecutará.

Una vez declarado, el procedimiento puede ser invocado desde cualquier parte del programa.

---

## Estructura general

```text
Procedimiento NombreProcedimiento(lista_parametros)

    instrucciones

FinProcedimiento
```

---

## Partes de la declaración

### Palabra reservada `Procedimiento`

Indica el inicio de la definición del procedimiento.

```text
Procedimiento
```

---

### Nombre del procedimiento

Permite identificar al procedimiento dentro del programa.

```text
Procedimiento MostrarMenu()
```

Se recomienda utilizar nombres descriptivos.

### Correcto

```text
Procedimiento MostrarMenu()
```

### Incorrecto

```text
Procedimiento P1()
```

---

### Lista de parámetros

Los parámetros son datos que el procedimiento recibe para realizar una tarea.

```text
Procedimiento MostrarSuma(a, b)
```

En este caso:

- `a` es un parámetro.
- `b` es un parámetro.

---

### Cuerpo del procedimiento

Contiene las instrucciones que serán ejecutadas.

```text
suma <- a + b
Mostrar suma
```

---

### Fin del procedimiento

Indica que la definición ha terminado.

```text
FinProcedimiento
```

---

## Ejemplo 1

```text
Procedimiento Saludar()

    Mostrar "Hola Mundo"

FinProcedimiento
```

Este procedimiento muestra un mensaje en pantalla.

---

## Ejemplo 2

```text
Procedimiento MostrarSuma(a, b)

    suma <- a + b

    Mostrar suma

FinProcedimiento
```

Si:

```text
a = 6
b = 8
```

La salida será:

```text
14
```

---

## Diagrama de la estructura de un procedimiento

```text
┌───────────────────────────┐
│ Procedimiento MostrarSuma │
├───────────────────────────┤
│ suma <- a + b             │
│ Mostrar suma              │
└───────────────────────────┘
```

---

## Diferencia con una función

### Función

```text
Funcion Sumar(a, b)

    Retornar a + b

FinFuncion
```

Devuelve un valor mediante `Retornar`.

### Procedimiento

```text
Procedimiento MostrarSuma(a, b)

    Mostrar a + b

FinProcedimiento
```

Realiza una acción sin necesidad de devolver un valor.

---

## Resumen

La declaración de un procedimiento consiste en definir su nombre, parámetros e instrucciones. A diferencia de las funciones, los procedimientos no están obligados a devolver un valor y suelen utilizarse para ejecutar acciones dentro del programa.
