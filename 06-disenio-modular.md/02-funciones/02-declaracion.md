# Declaración de Funciones

## ¿Qué es la declaración de una función?

La declaración es la forma en que se define una función dentro de un programa.

En ella se especifican:

- El nombre de la función.
- Los parámetros que recibirá.
- Las instrucciones que ejecutará.
- El valor que devolverá.

Una función debe ser declarada antes de ser utilizada.

---

## Estructura general

```text
Funcion NombreFuncion(lista_parametros)

    instrucciones

    Retornar resultado

FinFuncion
```

---

## Partes de la declaración

### Palabra reservada `Funcion`

Indica el inicio de la definición de una función.

```text
Funcion
```

---

### Nombre de la función

Identifica la función dentro del programa.

```text
Funcion Sumar()
```

Se recomienda utilizar nombres descriptivos.

### Correcto

```text
Funcion CalcularPromedio()
```

### Incorrecto

```text
Funcion F1()
```

---

### Lista de parámetros

Son los datos que recibe la función para realizar su tarea.

```text
Funcion Sumar(a, b)
```

En este caso:

- `a` es un parámetro.
- `b` es un parámetro.

---

### Cuerpo de la función

Contiene las instrucciones que ejecutará la función.

```text
resultado <- a + b
```

---

### Retorno

Permite devolver un resultado al programa que llamó a la función.

```text
Retornar resultado
```

Una función devuelve un único valor.

---

### Fin de la función

Indica que la definición ha terminado.

```text
FinFuncion
```

---

## Ejemplo completo

```text
Funcion Sumar(a, b)

    resultado <- a + b

    Retornar resultado

FinFuncion
```

### Funcionamiento

Si:

```text
a = 6
b = 8
```

Entonces:

```text
resultado <- 6 + 8
```

La función devolverá:

```text
14
```

---

## Diagrama de la estructura de una función

```text
┌───────────────────────────┐
│ Funcion Sumar(a, b)       │
├───────────────────────────┤
│ resultado <- a + b        │
├───────────────────────────┤
│ Retornar resultado        │
└───────────────────────────┘
```

---

## Resumen

La declaración de una función consiste en definir su nombre, parámetros, instrucciones y valor de retorno. Una vez declarada, podrá ser utilizada desde cualquier parte del programa mediante una llamada.
