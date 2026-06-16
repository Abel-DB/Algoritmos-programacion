# Procedimientos

## Definición

Un procedimiento es un subprograma que realiza una tarea específica dentro de un programa.

Al igual que las funciones, los procedimientos permiten dividir un problema en partes más pequeñas, organizadas y reutilizables.

La principal diferencia es que un procedimiento no devuelve un valor mediante una instrucción de retorno. Su propósito principal es ejecutar acciones o procesos dentro del programa.

---

## Características

* Poseen un nombre único.
* Pueden recibir parámetros.
* Ejecutan una tarea específica.
* No devuelven un valor mediante una instrucción de retorno.
* Pueden modificar variables recibidas como parámetros.
* Pueden ser llamados desde diferentes partes del programa.
* Facilitan la organización del código.

---

## ¿Cuándo utilizar un procedimiento?

Los procedimientos son útiles cuando se desea realizar una acción o conjunto de acciones sin necesidad de obtener un valor de retorno.

### Ejemplos

* Mostrar un menú.
* Imprimir información en pantalla.
* Leer datos de entrada.
* Actualizar información.
* Generar reportes.
* Mostrar resultados de cálculos.

---

## Diferencia entre función y procedimiento

| Función                                 | Procedimiento                                  |
| --------------------------------------- | ---------------------------------------------- |
| Devuelve un valor mediante `Retornar`.  | No devuelve valores mediante `Retornar`.       |
| Puede utilizarse dentro de expresiones. | Se ejecuta como una instrucción independiente. |
| Utiliza `Retornar`.                     | Normalmente no utiliza `Retornar`.             |
| Generalmente realiza cálculos.          | Generalmente realiza acciones o procesos.      |

### Función

```text
resultado <- Sumar(5, 3)
```

La función devuelve un valor que puede almacenarse en una variable.

### Procedimiento

```text
MostrarMenu()
```

El procedimiento ejecuta una acción y continúa con la ejecución del programa.

---

## Estructura general

```text
Procedimiento NombreProcedimiento(parametros)

    instrucciones

FinProcedimiento
```

### Componentes

* **Procedimiento:** indica el inicio de la definición.
* **NombreProcedimiento:** identifica al procedimiento.
* **Parámetros:** datos que puede recibir para realizar su tarea.
* **Instrucciones:** acciones que ejecutará el procedimiento.
* **FinProcedimiento:** indica el final de la definición.

---

## Ejemplo conceptual

```text
Procedimiento Saludar()

    Mostrar "Hola Mundo"

FinProcedimiento
```

Al ejecutarse, el procedimiento muestra un mensaje en pantalla.

### Resultado

```text
Hola Mundo
```

---

## Ventajas

* Favorecen la reutilización de código.
* Facilitan el mantenimiento de los programas.
* Mejoran la organización del software.
* Permiten dividir tareas complejas en tareas más simples.
* Hacen el código más legible y comprensible.
* Facilitan el trabajo en equipo.

---

## Resumen

Un procedimiento es un subprograma que ejecuta una tarea específica dentro de un programa.

A diferencia de una función, no devuelve un valor mediante una instrucción de retorno y se utiliza principalmente para realizar acciones o procesos como mostrar información, leer datos o ejecutar operaciones determinadas.

Los procedimientos son una herramienta fundamental de la programación modular porque permiten organizar mejor el código y reutilizar soluciones en diferentes partes de un programa.
