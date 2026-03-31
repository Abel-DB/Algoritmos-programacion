# Arreglos (Tablas)

---

## ¿Qué es un arreglo?

Un **arreglo** (también llamado **vector o tabla**) es una estructura que permite almacenar **varios datos del mismo tipo** en una sola variable.

Sirve para evitar crear muchas variables individuales.

### Sin arreglo:

* nota1, nota2, nota3, nota4...

### Con arreglo:

* notas[ ]

---

## ¿Cómo funciona?

Un arreglo funciona como una **lista ordenada de posiciones**.

Cada posición tiene:

* Un número (índice)
* Un valor almacenado

---

## Índices (MUY IMPORTANTE)

Los arreglos comienzan en **posición 0**

```
Posición:   0   1   2   3
Valores:   10  20  30  40
```

- notas[0] → 10
- notas[3] → 40

---

## Error común

- Pensar que empieza en 1
- Siempre empieza en 0

---

## Tipos de arreglos

---

### 1. Arreglo unidimensional (Vector)

Es una lista simple.

```
Edades = [18, 20, 22, 25]
```

---

### 2. Arreglo bidimensional (Matriz / Tabla)

Tiene filas y columnas.

```
        Col0  Col1  Col2
       ┌────┬────┬────┐
Fila0  │ 10 │ 20 │ 30 │
       ├────┼────┼────┤
Fila1  │ 40 │ 50 │ 60 │
       └────┴────┴────┘
```

- [0][1] → 20
- [1][2] → 60

---

## Operaciones con arreglos

---

### 1. Recorrer un arreglo

Se usa una variable (i) para pasar por todas las posiciones.

---

## Diagrama de flujo (recorrido)

```
        ┌───────────┐
        │  INICIO   │
        └─────┬─────┘
              │
        ┌───────────┐
        │ i = 0     │ ← Proceso
        └─────┬─────┘
              │
        ┌──────────────┐
        │ ¿i < 4?      │ ← Decisión
        └───┬────┬─────┘
            │    │
           Sí    No
            │    │
   ┌──────────────────┐
   │ Mostrar A[i]     │ ← Salida
   └─────┬────────────┘
         │
   ┌──────────────┐
   │ i = i + 1    │
   └─────┬────────┘
         │
         └────────────── (regresa)
              │
        ┌───────────┐
        │   FIN     │
        └───────────┘
```

---

## Prueba de escritorio

A = [10, 20, 30, 40]

| Paso        | i | A[i] |
| ----------- | - | ---- |
| Inicializar | 0 | -    |
| Mostrar     | 0 | 10   |
| Incremento  | 1 | -    |
| Mostrar     | 1 | 20   |
| Incremento  | 2 | -    |
| Mostrar     | 2 | 30   |
| Incremento  | 3 | -    |
| Mostrar     | 3 | 40   |
| Incremento  | 4 | -    |

---

### 2. Cargar datos en un arreglo

---

## Diagrama de flujo (carga)

```
        ┌───────────┐
        │  INICIO   │
        └─────┬─────┘
              │
        ┌───────────┐
        │ i = 0     │
        └─────┬─────┘
              │
        ┌──────────────┐
        │ ¿i < 3?      │
        └───┬────┬─────┘
            │    │
           Sí    No
            │    │
   ┌──────────────────┐
   │ Leer A[i]        │ ← Entrada
   └─────┬────────────┘
         │
   ┌──────────────┐
   │ i = i + 1    │
   └─────┬────────┘
         │
         └────────────── (regresa)
              │
        ┌───────────┐
        │   FIN     │
        └───────────┘
```

---

## Prueba de escritorio

| Paso | i | A[i] |
| ---- | - | ---- |
| Leer | 0 | 5    |
| Leer | 1 | 8    |
| Leer | 2 | 3    |

---

### 3. Buscar un valor

---

## Diagrama de flujo (búsqueda)

```
        ┌───────────┐
        │  INICIO   │
        └─────┬─────┘
              │
        ┌───────────┐
        │ i = 0     │
        └─────┬─────┘
              │
        ┌──────────────┐
        │ ¿i < 3?      │
        └───┬────┬─────┘
            │    │
           Sí    No
            │    │
   ┌──────────────────┐
   │ ¿A[i] == valor?  │ ← Decisión
   └───┬────┬─────────┘
       │    │
      Sí    No
       │     │
  "Encontrado" │
       │     │
       │  ┌──────────────┐
       │  │ i = i + 1    │
       │  └─────┬────────┘
       │        │
       └────────┘ (regresa)
            │
        ┌───────────┐
        │   FIN     │
        └───────────┘
```

---

## Prueba de escritorio

Buscar 8 en A = [5, 8, 3]

| Paso | i | A[i] | Resultado |
| ---- | - | ---- | --------- |
| 1    | 0 | 5    | No        |
| 2    | 1 | 8    | Sí        |

---

## Ventajas de los arreglos

* Organizan datos fácilmente
* Evitan repetir variables
* Facilitan cálculos
* Permiten trabajar con grandes cantidades de información

---

## Errores comunes

* Usar índices incorrectos
* Salirse del tamaño del arreglo
* Confundir posición con valor

---

## Aplicaciones

* Notas de estudiantes
* Listas de productos
* Datos estadísticos
* Tablas de información

---

## Símbolos utilizados

* Inicio / Fin → óvalo
* Proceso → rectángulo
* Entrada → paralelogramo
* Salida → documento
* Decisión → rombo

---

## Resumen

* Un arreglo guarda múltiples datos
* Se accede por índice (desde 0)
* Puede ser vector o matriz
* Se usa con ciclos
* Permite buscar, recorrer y almacenar datos

---
