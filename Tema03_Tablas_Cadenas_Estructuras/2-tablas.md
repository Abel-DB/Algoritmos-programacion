# Arreglos (Tablas)

---

## ¿Qué es un arreglo?

Un **arreglo** (también llamado **vector o tabla**) es una estructura que permite almacenar **varios datos del mismo tipo** en una sola variable.

Permite organizar información sin necesidad de crear muchas variables individuales.

Ejemplo conceptual:

* Sin arreglo: nota1, nota2, nota3
* Con arreglo: notas[ ]

---

## ¿Cómo funciona un arreglo?

Un arreglo funciona como una **lista ordenada de posiciones**.

Cada posición tiene:

* Un **índice** (posición)
* Un **valor almacenado**

---

## Índices (Importante)

Los arreglos comienzan en la posición **0**.

Ejemplo:

```
Posición:   0   1   2   3
Valores:   10  20  30  40
```

* notas[0] → 10
* notas[3] → 40

---

## Error común

* Pensar que el índice inicia en 1
* En la mayoría de los lenguajes inicia en 0

---

## Tipos de arreglos

---

### 1. Arreglo unidimensional (Vector)

Es una lista simple de elementos.

Ejemplo:

```
Edades = [18, 20, 22, 25]
```

---

### 2. Arreglo bidimensional (Matriz o tabla)

Organiza los datos en filas y columnas.

Ejemplo:

```
        Col0  Col1  Col2
       ┌────┬────┬────┐
Fila0  │ 10 │ 20 │ 30 │
       ├────┼────┼────┤
Fila1  │ 40 │ 50 │ 60 │
       └────┴────┴────┘
```

* [0][1] → 20
* [1][2] → 60

---

## Operaciones básicas (concepto)

En los arreglos se pueden realizar acciones como:

* Recorrer todos los elementos
* Leer o ingresar datos
* Buscar un valor
* Modificar información

---

## Ventajas de los arreglos

* Permiten organizar grandes cantidades de datos
* Evitan repetir variables
* Facilitan el manejo de información
* Hacen más eficiente el trabajo con datos

---

## Errores comunes

* Usar índices incorrectos
* Acceder a posiciones que no existen
* Confundir el índice con el valor
* No controlar el tamaño del arreglo

---

## Aplicaciones

* Notas de estudiantes
* Listas de productos
* Datos estadísticos
* Tablas de información

---

## Conclusión

Los arreglos son estructuras fundamentales que permiten organizar y manejar múltiples datos de forma eficiente.

---

## Resumen

* Un arreglo almacena varios datos del mismo tipo
* Se accede mediante índices (desde 0)
* Puede ser unidimensional o bidimensional
* Permite organizar y manipular información

---
