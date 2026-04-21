# Estructuras (Registros)

---

## ¿Qué es una estructura?

Una **estructura** (también llamada **registro**) es un tipo de dato compuesto que permite **agrupar varios datos relacionados** bajo un mismo nombre.

Sirve para representar información formada por varios elementos.

---

## Idea principal

Una estructura reúne datos de una misma entidad.

Ejemplos:

* Persona
* Estudiante
* Producto
* Vehículo
* Empleado

---

## Ejemplo conceptual

```text
Estudiante

Nombre    : Ana
Edad      : 21
Promedio  : 8.5
Carrera   : Sistemas
```

Todos esos datos pertenecen al mismo estudiante.

---

## ¿Por qué se usan?

Sin estructuras habría que manejar muchas variables separadas:

```text
nombre
edad
promedio
carrera
```

Con estructura, todo queda agrupado en una sola unidad lógica.

---

## Componentes de una estructura

### 1. Nombre

Identifica la estructura.

Ejemplo:

```text
Estudiante
```

---

### 2. Campos o atributos

Son los datos internos.

Ejemplo:

* nombre
* edad
* promedio
* carrera

---

### 3. Tipo de cada campo

Cada campo puede guardar un tipo distinto de dato.

| Campo    | Tipo   |
| -------- | ------ |
| nombre   | cadena |
| edad     | entero |
| promedio | real   |
| activo   | lógico |

---

## Características principales

* Agrupan datos relacionados
* Admiten distintos tipos de datos
* Mejoran el orden de la información
* Facilitan mantenimiento
* Representan objetos reales

---

## Tipos de estructuras

### 1. Estructura simple

Contiene un solo registro.

```text
Producto:
Nombre = Mouse
Precio = 45
Stock = 20
```

---

### 2. Conjunto de estructuras

Varios registros del mismo tipo.

```text
Alumnos
Productos
Empleados
Clientes
```

---

### 3. Estructuras anidadas

Una estructura dentro de otra.

```text
Persona
 ├─ Nombre
 ├─ Edad
 └─ Dirección
      ├─ Ciudad
      └─ Zona
```

---

## Operaciones comunes

### Crear

Definir una estructura.

### Guardar datos

Asignar información a sus campos.

### Consultar

Leer datos almacenados.

### Modificar

Cambiar información existente.

### Mostrar

Presentar todos los datos.

---

## Ejemplo práctico

### Registro de estudiante

```text
Nombre   : Carlos
Edad     : 20
Nota     : 87
Carrera  : Informática
```

---

## Diferencia con otros temas

### Estructura vs Variable simple

| Variable simple | Estructura          |
| --------------- | ------------------- |
| Guarda un dato  | Guarda varios datos |
| edad            | persona             |

---

### Estructura vs Arreglo

| Arreglo              | Estructura                   |
| -------------------- | ---------------------------- |
| Muchos datos iguales | Datos distintos relacionados |
| notas                | alumno                       |

---

## Ventajas

* Organizan información compleja
* Reducen variables separadas
* Facilitan comprensión
* Mejoran diseño de programas
* Representan mejor la realidad

---

## Desventajas

* Más complejas que una variable simple
* Requieren planificación
* Si se diseñan mal, desordenan el sistema

---

## Aplicaciones reales

* Sistema de alumnos
* Inventario de productos
* Registro de clientes
* Nómina de empleados
* Hospitales (pacientes)
* Juegos (personajes, objetos)

---

## Errores comunes

* Confundir estructura con arreglo
* Definir campos innecesarios
* Elegir tipos incorrectos
* No organizar los datos
* Usar nombres poco claros

---

## Buenas prácticas

* Usar nombres descriptivos
* Guardar solo datos necesarios
* Agrupar información relacionada
* Mantener orden lógico
* Evitar estructuras demasiado grandes

---

## Concepto importante

Las estructuras permiten **modelar objetos reales** mediante datos organizados.

Ejemplo:

```text
Persona  → nombre, edad, dirección
Producto → código, precio, stock
```

---

## Resumen

* Una estructura agrupa varios datos en una sola unidad
* Puede contener distintos tipos de datos
* Representa entidades reales
* Mejora organización de la información
* Es fundamental en programas medianos y grandes

---
