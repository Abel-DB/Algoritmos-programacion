# Tablas

## ¿Qué es una tabla?

Una **tabla** es una estructura de datos que permite almacenar varios elementos del mismo tipo bajo un único nombre.

Cada elemento se identifica mediante una posición denominada **índice**.

En programación, una tabla también es conocida como **arreglo**.

---

# Importancia

Las tablas permiten:

* Almacenar múltiples datos relacionados.
* Organizar información de forma eficiente.
* Evitar la creación de muchas variables independientes.
* Facilitar el procesamiento de conjuntos de datos.

---

# Conceptos fundamentales

| Concepto | Descripción                                      |
| -------- | ------------------------------------------------ |
| Tabla    | Conjunto de elementos del mismo tipo.            |
| Elemento | Dato almacenado dentro de la tabla.              |
| Índice   | Posición utilizada para acceder a un elemento.   |
| Tamaño   | Cantidad total de elementos que puede almacenar. |

---

# Representación de una tabla

## Ejemplo

```text
Índice:   0   1   2   3   4
Valor :  10  20  30  40  50
```

En este ejemplo:

* El primer elemento se encuentra en la posición 0.
* El último elemento se encuentra en la posición 4.

---

# Características

| Característica          | Descripción                                          |
| ----------------------- | ---------------------------------------------------- |
| Homogénea               | Todos los elementos son del mismo tipo.              |
| Tamaño fijo             | Se define al momento de su creación.                 |
| Acceso directo          | Los elementos pueden localizarse mediante su índice. |
| Organización secuencial | Los datos mantienen un orden definido.               |

---

# Acceso conceptual a los elementos

Cada elemento de una tabla puede identificarse mediante su índice.

Por ejemplo:

```text
Índice:   0   1   2   3   4
Valor :  10  20  30  40  50
```

Para obtener el valor 30 se utiliza el índice 2.

---

# Ventajas

| Ventaja       | Descripción                                 |
| ------------- | ------------------------------------------- |
| Organización  | Agrupa datos relacionados.                  |
| Eficiencia    | Facilita la localización de elementos.      |
| Reutilización | Reduce la cantidad de variables necesarias. |
| Escalabilidad | Permite trabajar con conjuntos de datos.    |

---

# Desventajas

| Desventaja             | Descripción                                    |
| ---------------------- | ---------------------------------------------- |
| Tamaño fijo            | No puede cambiar fácilmente su capacidad.      |
| Homogeneidad           | Solo almacena un tipo de dato.                 |
| Dependencia del índice | Requiere conocer la posición de los elementos. |

---

# Aplicaciones

Las tablas se utilizan en:

* Almacenamiento de calificaciones.
* Listas de productos.
* Inventarios.
* Estadísticas.
* Registros de información.
* Procesamiento de datos.

---

# Representación conceptual en memoria

Una tabla almacena varios elementos relacionados bajo una misma estructura.

```text
Calificaciones

[85] [90] [78] [95] [88]
```

Cada elemento ocupa una posición específica dentro de la tabla.

---

# Errores comunes

| Error                                | Descripción                                        |
| ------------------------------------ | -------------------------------------------------- |
| Confundir índice con posición humana | El primer índice suele ser 0.                      |
| Utilizar índices inexistentes        | Impide acceder correctamente a los datos.          |
| Exceder el tamaño de la tabla        | Produce errores en el manejo de la información.    |
| Mezclar tipos de datos               | Una tabla debe almacenar elementos del mismo tipo. |

---

# Conclusión

Las tablas permiten almacenar y organizar múltiples elementos del mismo tipo mediante una única estructura. Constituyen una herramienta fundamental para trabajar con conjuntos de información y representan una de las estructuras de datos más utilizadas en programación.

---

# Resumen

| Concepto          | Idea principal                                     |
| ----------------- | -------------------------------------------------- |
| Tabla             | Conjunto de elementos del mismo tipo.              |
| Elemento          | Dato almacenado dentro de la tabla.                |
| Índice            | Posición utilizada para acceder a los datos.       |
| Tamaño            | Cantidad máxima de elementos.                      |
| Ventaja principal | Organización eficiente de información relacionada. |
| Uso común         | Manejo de listas y colecciones de datos.           |
