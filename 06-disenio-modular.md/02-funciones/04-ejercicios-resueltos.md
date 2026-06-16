# Suma de dos números

### Problema

Desarrollar una función que reciba dos números y devuelva su suma.

---

### Declaración

```text
Funcion Sumar(a, b)

    resultado <- a + b

    Retornar resultado

FinFuncion
```

### Llamada

```text
r <- Sumar(6, 8)
```

### Resultado

```text
r = 14
```

---

# Calculadora Modular

### Problema

Desarrollar una calculadora capaz de:

1. Sumar dos números.
2. Restar dos números.
3. Multiplicar dos números.

---

## Análisis

### Entrada

```text
opcion
a
b
```

### Proceso

```text
Si opcion = 1 → Sumar
Si opcion = 2 → Restar
Si opcion = 3 → Multiplicar
```

### Salida

```text
resultado
```

---

## Funciones

### Función Sumar

```text
Funcion SumarN(x, y)

    s <- x + y

    Retornar s

FinFuncion
```

### Función Restar

```text
Funcion RestarN(x, y)

    r <- x - y

    Retornar r

FinFuncion
```

### Función Multiplicar

```text
Funcion MultiplicarN(x, y)

    m <- x * y

    Retornar m

FinFuncion
```

---

## Programa Principal

```text
Inicio

    Leer opcion
    Leer a
    Leer b

    Segun opcion Hacer

        1:
            resultado <- SumarN(a, b)

        2:
            resultado <- RestarN(a, b)

        3:
            resultado <- MultiplicarN(a, b)

        De Otro Modo:
            Mostrar "Opcion invalida"

    FinSegun

    Mostrar resultado

Fin
```

---

## Diagrama de flujo

```text
┌─────────────┐
│   Inicio    │
└──────┬──────┘
       │
       ▼
┌─────────────────┐
│ Leer opcion     │
│ Leer a          │
│ Leer b          │
└──────┬──────────┘
       │
       ▼
┌─────────────────┐
│ ¿opcion = 1?    │
└───┬─────────┬───┘
   Sí         No
    │          │
    ▼          ▼
SumarN()   ¿opcion = 2?
               │
          ┌────┴────┐
         Sí         No
          │          │
          ▼          ▼
      RestarN() MultiplicarN()
               │
               ▼
┌─────────────────┐
│ Mostrar resultado│
└──────┬──────────┘
       │
       ▼
┌─────────────┐
│    Fin      │
└─────────────┘
```

---

## Prueba de escritorio

### Datos de entrada

```text
opcion = 1
a = 6
b = 8
```

### Ejecución

```text
resultado <- SumarN(6, 8)
```

Dentro de la función:

```text
s <- 6 + 8
s <- 14
```

Retorno:

```text
14
```

### Salida

```text
resultado = 14
```

---

## Beneficios observados

- Cada operación se encuentra en una función independiente.
- El código es más organizado.
- Las funciones pueden reutilizarse en otros programas.
- El mantenimiento es más sencillo.
- Se evita repetir instrucciones.

---

## Resumen

Las funciones permiten dividir un problema en tareas más pequeñas y reutilizables. En este ejemplo, cada operación matemática se implementa mediante una función independiente, logrando una solución modular, organizada y fácil de mantener.
