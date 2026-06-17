# Estructuras

## ¿Qué es una estructura?

Una **estructura** es una estructura de datos que permite agrupar varios datos relacionados bajo una misma entidad.

A diferencia de una tabla, cuyos elementos son del mismo tipo, una estructura puede contener datos de diferentes tipos.

Las estructuras permiten representar objetos o entidades del mundo real.

---

# Importancia

Las estructuras permiten:

* Organizar información relacionada.
* Agrupar datos bajo una única entidad.
* Facilitar la representación de objetos reales.
* Mejorar la comprensión de los algoritmos.
* Reducir la cantidad de variables independientes.

---

# Conceptos fundamentales

| Concepto       | Descripción                                            |
| -------------- | ------------------------------------------------------ |
| Estructura     | Agrupación de datos relacionados.                      |
| Campo          | Dato individual que forma parte de la estructura.      |
| Entidad        | Objeto o elemento representado mediante la estructura. |
| Tipo compuesto | Tipo formado por varios datos.                         |

---

# Problema que resuelven

Supongamos que deseamos almacenar información de un estudiante.

Sin estructura:

```text
Nombre
Edad
Promedio
Carrera
```

Cada dato debe manejarse por separado.

Con una estructura:

```text
Estudiante
├── Nombre
├── Edad
├── Promedio
└── Carrera
```

Toda la información queda agrupada bajo una única entidad.

---

# Diferencia entre tablas y estructuras

| Tabla                          | Estructura                                |
| ------------------------------ | ----------------------------------------- |
| Almacena datos del mismo tipo. | Puede almacenar datos de distintos tipos. |
| Se accede mediante índices.    | Se accede mediante campos.                |
| Representa colecciones.        | Representa entidades.                     |

---

# Representación conceptual

## Estudiante

```text
Estudiante
│
├── Nombre   → Juan Pérez
├── Edad     → 20
├── Promedio → 85.5
└── Carrera  → Ingeniería
```

---

## Producto

```text
Producto
│
├── Código      → P001
├── Nombre      → Laptop
├── Precio      → 850.00
└── Existencias → 12
```

---

# Características

| Característica | Descripción                                 |
| -------------- | ------------------------------------------- |
| Agrupación     | Reúne datos relacionados.                   |
| Organización   | Facilita el manejo de información compleja. |
| Flexibilidad   | Puede combinar diferentes tipos de datos.   |
| Representación | Modela entidades del mundo real.            |

---

# Ventajas

| Ventaja       | Descripción                                          |
| ------------- | ---------------------------------------------------- |
| Organización  | Mantiene los datos relacionados en un solo lugar.    |
| Claridad      | Facilita la lectura y comprensión de la información. |
| Reutilización | Permite representar múltiples entidades similares.   |
| Escalabilidad | Facilita el crecimiento de los sistemas.             |

---

# Limitaciones

| Limitación        | Descripción                                        |
| ----------------- | -------------------------------------------------- |
| Mayor complejidad | Requiere definir la estructura de los datos.       |
| Diseño previo     | Es necesario identificar correctamente los campos. |

---

# Aplicaciones

Las estructuras se utilizan para representar:

* Estudiantes.
* Empleados.
* Clientes.
* Productos.
* Vehículos.
* Inventarios.
* Registros de información.

---

# Relación con la memoria

Cada estructura almacena todos los datos que forman parte de la entidad representada.

```text
Estudiante

Nombre   → Juan Pérez
Edad     → 20
Promedio → 85.5
Carrera  → Ingeniería
```

Los datos permanecen agrupados y relacionados entre sí.

---

# Errores comunes

| Error                           | Descripción                                   |
| ------------------------------- | --------------------------------------------- |
| Confundir estructura con tabla  | Cumplen funciones diferentes.                 |
| Definir campos innecesarios     | Incrementa la complejidad.                    |
| Omitir información importante   | La entidad queda incompleta.                  |
| Diseñar estructuras poco claras | Dificulta el mantenimiento de la información. |

---

# Relación con la programación

Las estructuras sirven como base para representar entidades complejas dentro de los algoritmos.

Posteriormente, los lenguajes de programación proporcionan mecanismos específicos para implementar estas estructuras de datos.

---

# Conclusión

Las estructuras permiten agrupar información relacionada bajo una misma entidad, facilitando la organización y representación de datos complejos. Constituyen una herramienta fundamental para modelar objetos del mundo real dentro de los algoritmos y sistemas informáticos.

---

# Resumen

| Concepto             | Idea principal                              |
| -------------------- | ------------------------------------------- |
| Estructura           | Agrupa datos relacionados.                  |
| Campo                | Dato individual de la estructura.           |
| Entidad              | Objeto representado mediante la estructura. |
| Tipo compuesto       | Formado por varios datos.                   |
| Ventaja principal    | Organización de información compleja.       |
| Aplicación principal | Representación de entidades del mundo real. |
