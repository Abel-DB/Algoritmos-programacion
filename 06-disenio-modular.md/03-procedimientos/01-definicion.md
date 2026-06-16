# Procedimientos

## Definición

Un procedimiento es un subprograma que realiza una tarea específica dentro de un programa.

Al igual que las funciones, los procedimientos permiten dividir un problema en partes más pequeñas y reutilizables.

La principal diferencia es que un procedimiento no necesariamente devuelve un único valor como resultado.

---

## Características

- Poseen un nombre único.
- Pueden recibir parámetros.
- Ejecutan una tarea específica.
- Pueden devolver cero, uno o varios resultados.
- Pueden modificar variables recibidas como parámetros.
- Pueden ser llamados desde cualquier parte del programa.

---

## ¿Cuándo utilizar un procedimiento?

Los procedimientos son útiles cuando se desea realizar una acción o conjunto de acciones sin necesidad de obtener un único valor de retorno.

### Ejemplos

- Mostrar un menú.
- Imprimir información en pantalla.
- Leer datos de entrada.
- Actualizar registros.
- Generar reportes.

---

## Diferencia entre función y procedimiento

| Función | Procedimiento |
|----------|-------------|
| Devuelve un único valor. | No necesariamente devuelve un valor. |
| Se utiliza dentro de expresiones. | Se ejecuta como una instrucción. |
| Utiliza `Retornar`. | Puede no utilizar `Retornar`. |
| Generalmente realiza cálculos. | Generalmente realiza acciones o procesos. |

### Función

```text
resultado <- Sumar(5, 3)
```

La función devuelve un valor que se almacena en una variable.

### Procedimiento

```text
MostrarMenu()
```

El procedimiento ejecuta una acción.

---

## Estructura general

```text
Procedimiento NombreProcedimiento(parametros)

    instrucciones

FinProcedimiento
```

---

## Ejemplo conceptual

```text
Procedimiento Saludar()

    Mostrar "Hola Mundo"

FinProcedimiento
```

Al ejecutarse, el procedimiento muestra un mensaje en pantalla.

---

## Ventajas

- Favorecen la reutilización de código.
- Facilitan el mantenimiento.
- Mejoran la organización del programa.
- Permiten dividir tareas complejas.
- Hacen el código más legible.

---

## Resumen

Un procedimiento es un subprograma que realiza una tarea específica dentro de un programa. A diferencia de una función, no está obligado a devolver un único valor y suele utilizarse para ejecutar acciones o procesos.
