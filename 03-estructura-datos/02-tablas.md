# Tablas

## ¿Qué es una tabla?

Una **tabla** es una estructura de datos que permite almacenar varios elementos del mismo tipo bajo un único nombre.

Cada elemento se identifica mediante una posición denominada **índice**.

En programación, una tabla también es conocida como **arreglo** (*array*).

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

### Ejemplo

```text
Índice:   0   1   2   3   4
Valor :  10  20  30  40  50
```

En este ejemplo:

* El primer elemento se encuentra en la posición `0`.
* El último elemento se encuentra en la posición `4`.

---

# Características

| Característica          | Descripción                                        |
| ----------------------- | -------------------------------------------------- |
| Homogénea               | Todos los elementos son del mismo tipo.            |
| Tamaño fijo             | Se define al momento de su creación.               |
| Acceso directo          | Los elementos pueden accederse mediante su índice. |
| Almacenamiento contiguo | Los datos se guardan consecutivamente en memoria.  |

---

# Declaración en C++

## Sintaxis

```cpp
tipo nombre[tamaño];
```

### Ejemplo

```cpp
int notas[5];
```

La tabla puede almacenar cinco números enteros.

---

# Inicialización

### Ejemplo

```cpp
int numeros[5] = {10, 20, 30, 40, 50};
```

Representación:

```text
Índice:   0   1   2   3   4
Valor :  10  20  30  40  50
```

---

# Acceso a elementos

Para acceder a un elemento se utiliza su índice.

### Ejemplo

```cpp
cout << numeros[0];
```

Resultado:

```text
10
```

---

# Modificación de elementos

### Ejemplo

```cpp
numeros[2] = 100;
```

Resultado:

```text
Índice:   0   1    2   3   4
Valor :  10  20  100  40  50
```

---

# Recorrido de una tabla

Una tabla suele recorrerse utilizando estructuras repetitivas.

### Ejemplo

```cpp
for (int i = 0; i < 5; i++) {
    cout << numeros[i] << endl;
}
```

> **Nota:** Las estructuras repetitivas se estudiarán con mayor profundidad en el tema de instrucciones de control.

---

# Ventajas

| Ventaja       | Descripción                                 |
| ------------- | ------------------------------------------- |
| Organización  | Agrupa datos relacionados.                  |
| Eficiencia    | Facilita el acceso a los elementos.         |
| Reutilización | Reduce la cantidad de variables necesarias. |
| Escalabilidad | Permite trabajar con conjuntos de datos.    |

---

# Desventajas

| Desventaja             | Descripción                               |
| ---------------------- | ----------------------------------------- |
| Tamaño fijo            | No puede crecer dinámicamente.            |
| Homogeneidad           | Solo almacena un tipo de dato.            |
| Desperdicio de memoria | Puede reservar más espacio del necesario. |

---

# Aplicaciones

Las tablas se utilizan en:

* Almacenamiento de calificaciones.
* Listas de productos.
* Inventarios.
* Estadísticas.
* Procesamiento de datos.

---

# Relación con la memoria

Una tabla almacena sus elementos de forma consecutiva.

```text
Dirección → [10][20][30][40][50]
Índice       0   1   2   3   4
```

Esto permite acceder rápidamente a cualquier elemento.

---

# Errores comunes

| Error                                | Descripción                          |
| ------------------------------------ | ------------------------------------ |
| Acceder a índices inexistentes       | Produce comportamientos inesperados. |
| Confundir índice con posición humana | El primer índice es 0.               |
| Exceder el tamaño de la tabla        | Puede generar errores de ejecución.  |
| Utilizar índices negativos           | No están permitidos.                 |

---

# Información complementaria

Para comprender cómo recorrer tablas mediante estructuras repetitivas, consulte:

* [Instrucciones de control](../Tema05_instrucciones_control/repetitivas/)

---

# Conclusión

Las tablas permiten almacenar y organizar múltiples datos del mismo tipo mediante una única estructura. Constituyen una herramienta fundamental para trabajar con conjuntos de información dentro de un programa.

---

# Resumen

| Concepto          | Idea principal                                 |
| ----------------- | ---------------------------------------------- |
| Tabla             | Conjunto de elementos del mismo tipo.          |
| Índice            | Posición utilizada para acceder a los datos.   |
| Tamaño            | Cantidad máxima de elementos.                  |
| Ventaja principal | Organización eficiente de datos.               |
| Uso común         | Manejo de listas y colecciones de información. |
