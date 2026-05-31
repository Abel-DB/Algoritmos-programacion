# Variables y Tipos de Datos

## ¿Qué es una variable?

Una **variable** es un espacio de memoria utilizado para almacenar información que puede cambiar durante la ejecución de un programa.

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
* Interactuar con el usuario.
* Construir algoritmos y programas.

Sin variables sería imposible guardar información temporal durante la ejecución de un programa.

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
Tipo   : int
Valor  : 20
```

---

# Reglas para nombrar variables

| Regla                             | Ejemplo            |
| --------------------------------- | ------------------ |
| Debe comenzar con una letra o `_` | edad, _contador    |
| No puede contener espacios        | nombre_usuario     |
| No puede usar palabras reservadas | int, while, if     |
| Debe ser descriptiva              | promedio, cantidad |

---

## Ejemplos correctos

```text
edad
nombre
promedio
cantidadEstudiantes
```

---

## Ejemplos incorrectos

```text
2edad
mi nombre
while
int
```

---

# Buenas prácticas

| Recomendación                        | Ejemplo                            |
| ------------------------------------ | ---------------------------------- |
| Utilizar nombres descriptivos        | promedioFinal                      |
| Evitar abreviaturas confusas         | cantidadEstudiantes                |
| Mantener un estilo consistente       | utilizar siempre el mismo criterio |
| Relacionar el nombre con el problema | salario, nota, totalVentas         |

## Información complementaria

Para conocer las convenciones de nombres utilizadas en proyectos de C++, consulte:

- [Convenciones de nombres](../Anexos/convensiones_nombres.md)

---

# ¿Qué es un tipo de dato?

Un **tipo de dato** define la clase de información que una variable puede almacenar.

Determina:

* El espacio utilizado en memoria.
* El rango de valores permitidos.
* Las operaciones que pueden realizarse.

---

# Clasificación de tipos de datos

## Tipos enteros

Se utilizan para almacenar números sin decimales.

| Tipo      | Tamaño aproximado | Rango aproximado    | Uso principal       |
| --------- | ----------------- | ------------------- | ------------------- |
| short     | 2 bytes           | -32,768 a 32,767    | Valores pequeños    |
| int       | 4 bytes           | ±2 mil millones     | Uso general         |
| long      | 4 u 8 bytes       | Depende del sistema | Valores grandes     |
| long long | 8 bytes           | Muy amplio          | Valores muy grandes |

---

## Tipos reales

Se utilizan para almacenar números con decimales.

| Tipo        | Tamaño aproximado | Precisión                  |
| ----------- | ----------------- | -------------------------- |
| float       | 4 bytes           | ~7 dígitos significativos  |
| double      | 8 bytes           | ~15 dígitos significativos |
| long double | 8 a 16 bytes      | Mayor precisión            |

---

## Tipos de caracteres

Se utilizan para almacenar un único carácter.

| Tipo | Tamaño aproximado | Ejemplo       |
| ---- | ----------------- | ------------- |
| char | 1 byte            | 'A', 'b', '9' |

---

## Tipos de texto

Se utilizan para almacenar cadenas de caracteres.

| Tipo   | Descripción             | Ejemplo      |
| ------ | ----------------------- | ------------ |
| string | Secuencia de caracteres | "Hola Mundo" |

---

## Tipos lógicos

Se utilizan para representar condiciones verdaderas o falsas.

| Tipo | Tamaño aproximado | Valores posibles |
| ---- | ----------------- | ---------------- |
| bool | 1 byte            | true, false      |

> **Nota:** Los tamaños y rangos pueden variar según el compilador y la arquitectura del sistema.

---

# Declaración de variables en C++

## Sintaxis general

```cpp
tipo nombre;
```

### Ejemplos

```cpp
int edad;
float promedio;
char inicial;
bool activo;
string nombre;
```

---

# Inicialización de variables

Consiste en asignar un valor inicial al momento de declararlas.

### Ejemplos

```cpp
int edad = 20;
float promedio = 85.5;
char letra = 'A';
bool activo = true;
string nombre = "Juan";
```

---

# Relación entre variable y memoria

Cuando se declara una variable, el sistema reserva un espacio de memoria para almacenar su valor.

```text
Variable      Valor
edad          20
promedio      85.5
activo        true
```

---

# Errores comunes

| Error                    | Descripción                           |
| ------------------------ | ------------------------------------- |
| Nombre poco descriptivo  | Dificulta la comprensión del código.  |
| Usar palabras reservadas | Genera errores de compilación.        |
| Tipo incorrecto          | Produce resultados inesperados.       |
| No inicializar variables | Puede generar valores indeterminados. |

---

# Aplicaciones

Las variables se utilizan en:

* Sistemas bancarios.
* Videojuegos.
* Aplicaciones móviles.
* Sistemas empresariales.
* Programas científicos.
* Bases de datos.

---

# Conclusión

Las variables permiten almacenar y manipular información dentro de un programa. Su correcto uso, junto con la elección adecuada de tipos de datos, constituye una de las bases fundamentales de la programación.

---

# Resumen

| Concepto       | Idea principal                                |
| -------------- | --------------------------------------------- |
| Variable       | Espacio de memoria para almacenar datos.      |
| Componentes    | Nombre, tipo y valor.                         |
| Tipos de datos | Enteros, reales, caracteres, texto y lógicos. |
| Declaración    | Define una variable dentro del programa.      |
| Inicialización | Asigna un valor inicial.                      |
| Importancia    | Permite almacenar y manipular información.    |
