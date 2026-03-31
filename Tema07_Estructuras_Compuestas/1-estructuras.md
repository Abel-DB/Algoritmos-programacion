# Estructuras (Registros)

---

## ¿Qué es una estructura?

Una **estructura** es un tipo de dato compuesto que permite **agrupar múltiples datos de diferentes tipos** bajo un mismo nombre.

Se utiliza cuando un solo dato no es suficiente para representar una entidad.

---

## Idea clave

Una estructura representa un **objeto del mundo real**.

Ejemplos:

* Persona
* Estudiante
* Producto
* Vehículo

---

## Ejemplo conceptual

```id="h2s8dk"
Estudiante
┌────────────────────┐
│ Nombre   → "Ana"   │ (cadena)
│ Edad     → 21      │ (entero)
│ Promedio → 8.5     │ (decimal)
└────────────────────┘
```

---

## Componentes de una estructura

Una estructura está formada por:

### 1. Campos (atributos)

Son las variables internas.

Ejemplo:

* nombre
* edad
* promedio

---

### 2. Tipos de datos

Cada campo tiene su tipo:

| Campo    | Tipo   |
| -------- | ------ |
| nombre   | cadena |
| edad     | entero |
| promedio | real   |

---

### 3. Identificador

Es el nombre de la estructura.

Ejemplo:

```id="u4x0pl"
Estudiante
```

---

# Tipos de estructuras

---

## 1. Estructura simple

Contiene un solo registro.

```id="7f1k9m"
Persona → Juan, 20
```

---

## 2. Arreglo de estructuras

Contiene múltiples registros.

```id="jv93la"
Personas[3]
```

---

## 3. Estructuras anidadas

Una estructura dentro de otra.

---

### Ejemplo

```id="k9dm21"
Dirección
┌──────────────┐
│ Ciudad       │
│ Calle        │
└──────────────┘

Persona
┌────────────────────┐
│ Nombre             │
│ Edad               │
│ Dirección          │ ← estructura
└────────────────────┘
```

---

# Operaciones con estructuras

---

## 1. Declarar

Definir la estructura.

---

## 2. Crear (instanciar)

Crear una variable de ese tipo.

---

## 3. Asignar valores

Guardar datos en los campos.

---

## 4. Acceder a los campos

Ejemplo:

```id="u9d2sx"
Persona.nombre
Persona.edad
```

---

## 5. Modificar datos

Cambiar valores existentes.

---

## 6. Mostrar información

Imprimir todos los campos.

---

# Diagrama de flujo (completo)

```id="z8p1wq"
   ┌───────────┐
   │  INICIO   │
   └─────┬─────┘
         │
   ┌──────────────────────┐
   │ Leer Nombre, Edad    │ ← Entrada (paralelogramo)
   └─────┬────────────────┘
         │
   ┌──────────────────────┐
   │ Guardar en estructura│ ← Proceso (rectángulo)
   └─────┬────────────────┘
         │
   ┌──────────────────────┐
   │ Mostrar datos        │ ← Salida (documento)
   └─────┬────────────────┘
         │
   ┌───────────┐
   │   FIN     │
   └───────────┘
```

---

# Prueba de escritorio

| Paso    | Nombre | Edad | Acción  |
| ------- | ------ | ---- | ------- |
| Leer    | Ana    | 21   | Entrada |
| Guardar | Ana    | 21   | Proceso |
| Mostrar | Ana    | 21   | Salida  |

---

# Diferencias importantes

---

## Estructura vs Arreglo

| Característica | Estructura | Arreglo |
| -------------- | ---------- | ------- |
| Tipos          | Diferentes | Igual   |
| Uso            | Complejo   | Simple  |
| Ejemplo        | Persona    | Lista   |

---

## Estructura vs Variable simple

| Variable | Estructura   |
| -------- | ------------ |
| Un dato  | Varios datos |
| Simple   | Compuesta    |

---

# Conceptos clave importantes

---

## 1. Abstracción

Las estructuras permiten representar entidades reales de forma simplificada.

---

## 2. Modularidad

Permiten organizar mejor el programa.

---

## 3. Reutilización

Se pueden usar varias veces.

---

## 4. Organización de datos

Evitan tener muchas variables sueltas.

---

# Ventajas

- Ordenan la información
- Facilitan el mantenimiento
- Representan mejor la realidad
- Escalan a programas grandes

---

# Desventajas

- Más complejas que variables simples
- Requieren planificación

---

# Aplicaciones reales

* Sistemas de alumnos
* Inventarios
* Registros de usuarios
* Bases de datos simples
* Videojuegos (personajes, objetos)

---

# Errores comunes

* Confundir con arreglos
* No definir bien los campos
* Usar tipos incorrectos
* No organizar la información

---

# Relación con otros temas

Las estructuras se combinan con:

* Arreglos → listas de registros
* Cadenas → nombres, textos
* Funciones → manipulación de datos

---

# Nivel avanzado (importante)

---

## Colecciones de estructuras

Ejemplo:

```id="r2k8tx"
Estudiantes[100]
```

Base de sistemas reales.

---

## Paso de estructuras

Se pueden pasar a funciones para trabajar con ellas.

---

## Modelado de problemas

Este es el uso MÁS importante:

Transformar un problema real en datos organizados.

---

# Conclusión

Las estructuras son fundamentales para representar información compleja.

Son el puente entre:

* Problema real
* Solución en programación

---

# Resumen

* Agrupan datos diferentes
* Representan objetos reales
* Se componen de campos
* Pueden combinarse con arreglos
* Son base de sistemas grandes

---
