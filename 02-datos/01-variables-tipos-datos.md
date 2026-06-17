# Variables y Tipos de Datos

## ¿Qué es una variable?

Una **variable** es un espacio utilizado para almacenar información que puede cambiar durante la resolución de un problema o la ejecución de un algoritmo.

Cada variable posee:

* Un nombre.
* Un tipo de dato.
* Un valor.

---

# Importancia

Las variables permiten:

* Almacenar información.
* Realizar cálculos.
* Manipular datos.
* Resolver problemas.
* Construir algoritmos y programas.

Sin variables sería imposible guardar información temporal durante la ejecución de una solución.

---

# Componentes de una variable

| Componente | Descripción                                       |
| ---------- | ------------------------------------------------- |
| Nombre     | Identificador utilizado para acceder al dato.     |
| Tipo       | Define qué clase de información puede almacenar.  |
| Valor      | Información almacenada en un momento determinado. |

### Ejemplo

```text
Nombre : edad
Tipo   : Entero
Valor  : 20
```

---

# Reglas para nombrar variables

| Regla                             | Ejemplo            |
| --------------------------------- | ------------------ |
| Debe comenzar con una letra       | edad               |
| No debe contener espacios         | nombre_usuario     |
| Debe ser descriptiva              | promedio, cantidad |
| Debe relacionarse con el problema | salario, notaFinal |

---

## Ejemplos correctos

```text
edad
nombre
promedio
cantidad_estudiantes
```

---

## Ejemplos incorrectos

```text
2edad
mi nombre
@
#
```

---

# Buenas prácticas

| Recomendación                        | Ejemplo                            |
| ------------------------------------ | ---------------------------------- |
| Utilizar nombres descriptivos        | promedio_final                      |
| Evitar abreviaturas confusas         | cantidad_estudiantes                |
| Mantener un estilo consistente       | utilizar siempre el mismo criterio |
| Relacionar el nombre con el problema | salario, nota, total_ventas         |

---

# Constantes

## ¿Qué es una constante?

Una **constante** es un dato cuyo valor permanece fijo durante la ejecución de un algoritmo o programa.

A diferencia de una variable, una constante no está diseñada para cambiar su valor.

---

# Importancia

Las constantes permiten:

* Representar valores permanentes.
* Mejorar la claridad de los algoritmos.
* Evitar modificaciones accidentales.
* Facilitar el mantenimiento de las soluciones.

---

# Ejemplos de constantes

| Constante   | Significado                    |
| ----------- | ------------------------------ |
| PI          | Valor aproximado de π          |
| DIAS_SEMANA | Cantidad de días de una semana |
| IVA         | Porcentaje de impuesto         |

---

# Diferencia entre variable y constante

| Variable                                | Constante                          |
| --------------------------------------- | ---------------------------------- |
| Su valor puede cambiar.                 | Su valor permanece fijo.           |
| Almacena información variable.          | Representa información permanente. |
| Puede modificarse durante la ejecución. | No debería modificarse.            |

---

# Ejemplo conceptual

## Problema

Calcular el área de un círculo.

### Constante

```text
PI = 3.1416
```

### Variable

```text
radio
```

### Fórmula

```text
Área = PI × radio²
```

---

# ¿Qué es un tipo de dato?

Un **tipo de dato** define la naturaleza de la información que puede almacenarse en una variable o constante.

Los tipos de datos permiten representar distintos tipos de información dentro de una solución.

---

# Clasificación de tipos de datos

## Datos numéricos

Representan cantidades y valores matemáticos.

### Enteros

No poseen parte decimal.

#### Ejemplos

```text
10
25
-8
0
```

### Reales

Poseen parte decimal.

#### Ejemplos

```text
3.14
8.5
-12.75
```

---

## Datos alfanuméricos

Representan caracteres y texto.

### Carácter

Representa un único símbolo.

#### Ejemplos

```text
A
b
7
$
```

### Cadena de caracteres

Representa una secuencia de caracteres.

#### Ejemplos

```text
Hola
Programación
Juan Pérez
```

---

## Datos lógicos

Representan condiciones o estados.

### Valores posibles

```text
Verdadero
Falso
```

---

# Importancia de los tipos de datos

Los tipos de datos permiten:

* Organizar la información.
* Representar distintos tipos de valores.
* Evitar errores conceptuales.
* Facilitar el diseño de algoritmos.

---

# Ejemplo

## Problema

Registrar información de un estudiante.

| Dato     | Tipo   |
| -------- | ------ |
| Nombre   | Cadena |
| Edad     | Entero |
| Promedio | Real   |
| Aprobado | Lógico |

---

# Relación entre variable y valor

Durante la ejecución de un algoritmo, las variables almacenan información que puede cambiar.

```text
Variable      Valor
edad          20
promedio      85.5
aprobado      Verdadero
```

---

# Errores comunes

| Error                              | Descripción                             |
| ---------------------------------- | --------------------------------------- |
| Nombre poco descriptivo            | Dificulta la comprensión del algoritmo. |
| Utilizar un tipo incorrecto        | Produce resultados inesperados.         |
| Confundir variables con constantes | Puede generar errores de diseño.        |
| Representar mal la información     | Dificulta la solución del problema.     |

---

# Aplicaciones

Las variables y tipos de datos se utilizan en prácticamente cualquier algoritmo:

* Sistemas bancarios.
* Videojuegos.
* Aplicaciones móviles.
* Sistemas empresariales.
* Programas científicos.
* Sistemas educativos.

---

# Conclusión

Las variables permiten almacenar información necesaria para resolver problemas, mientras que los tipos de datos permiten representar adecuadamente esa información. El uso correcto de ambos conceptos constituye una de las bases fundamentales de la programación y del diseño de algoritmos.

---

# Resumen

| Concepto            | Idea principal                                                        |
| ------------------- | --------------------------------------------------------------------- |
| Variable            | Almacena información que puede cambiar.                               |
| Constante           | Representa información que permanece fija.                            |
| Tipo de dato        | Define la naturaleza de la información almacenada.                    |
| Datos numéricos     | Enteros y reales.                                                     |
| Datos alfanuméricos | Caracteres y cadenas.                                                 |
| Datos lógicos       | Verdadero o falso.                                                    |
| Importancia         | Permiten representar y manipular información para resolver problemas. |
