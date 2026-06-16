# Mostrar un mensaje

### Problema

Crear un procedimiento que muestre un mensaje de bienvenida.

---

### Declaración

```text
Procedimiento Saludar()

    Mostrar "Bienvenido al sistema"

FinProcedimiento
```

### Llamada

```text
Saludar()
```

### Salida

```text
Bienvenido al sistema
```

---

## Mostrar la suma de dos números

### Problema

Crear un procedimiento que reciba dos números y muestre su suma.

---

### Declaración

```text
Procedimiento MostrarSuma(a, b)

    suma <- a + b

    Mostrar suma

FinProcedimiento
```

### Llamada

```text
MostrarSuma(6, 8)
```

### Salida

```text
14
```

---

## Menú de opciones

### Problema

Crear un procedimiento que muestre un menú de opciones para una calculadora.

---

### Declaración

```text
Procedimiento MostrarMenu()

    Mostrar "1. Sumar"
    Mostrar "2. Restar"
    Mostrar "3. Multiplicar"
    Mostrar "4. Salir"

FinProcedimiento
```

### Llamada

```text
MostrarMenu()
```

### Salida

```text
1. Sumar
2. Restar
3. Multiplicar
4. Salir
```

---

## Programa Principal utilizando procedimientos

```text
Procedimiento MostrarMenu()

    Mostrar "1. Sumar"
    Mostrar "2. Restar"
    Mostrar "3. Multiplicar"

FinProcedimiento


Inicio

    MostrarMenu()

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
│ MostrarMenu()   │
└──────┬──────────┘
       │
       ▼
┌─────────────────┐
│ Mostrar opciones│
└──────┬──────────┘
       │
       ▼
┌─────────────────┐
│ Regresar al     │
│ programa        │
└──────┬──────────┘
       │
       ▼
┌─────────────┐
│    Fin      │
└─────────────┘
```

---

## Prueba de escritorio

### Entrada

```text
MostrarMenu()
```

### Ejecución

```text
Mostrar "1. Sumar"
Mostrar "2. Restar"
Mostrar "3. Multiplicar"
```

### Salida

```text
1. Sumar
2. Restar
3. Multiplicar
```

---

## Funciones vs Procedimientos

### Función

```text
Funcion Sumar(a, b)

    Retornar a + b

FinFuncion
```

Uso:

```text
resultado <- Sumar(6, 8)
```

La función devuelve un valor.

---

### Procedimiento

```text
Procedimiento MostrarSuma(a, b)

    Mostrar a + b

FinProcedimiento
```

Uso:

```text
MostrarSuma(6, 8)
```

El procedimiento realiza una acción.

---

## Resumen

Los procedimientos permiten ejecutar tareas específicas dentro de un programa. Son especialmente útiles para mostrar información, leer datos, generar reportes o realizar acciones que no requieren devolver un único valor como resultado.
