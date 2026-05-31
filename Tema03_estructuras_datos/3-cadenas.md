# Cadenas

## ¿Qué es una cadena?

Una **cadena** es una secuencia de caracteres almacenados y tratados como una única unidad de información.

Las cadenas permiten representar texto dentro de un programa.

### Ejemplos

```text
"Hola"
"Programación"
"Juan Pérez"
"2025"
```

---

# Importancia

Las cadenas permiten:

* Almacenar texto.
* Mostrar mensajes al usuario.
* Procesar información textual.
* Validar datos ingresados.
* Manipular palabras y frases.

---

# Conceptos fundamentales

| Concepto | Descripción                                    |
| -------- | ---------------------------------------------- |
| Cadena   | Conjunto de caracteres.                        |
| Carácter | Unidad individual representada por `char`.     |
| Longitud | Cantidad de caracteres que posee una cadena.   |
| Índice   | Posición de cada carácter dentro de la cadena. |

---

# Relación con ASCII

Cada carácter de una cadena se almacena internamente utilizando su código ASCII.

### Ejemplo

```text
Cadena: "ABC"

A → 65
B → 66
C → 67
```

Por este motivo, las computadoras pueden almacenar y procesar texto.

---

# Relación con las tablas

Conceptualmente, una cadena puede verse como una colección ordenada de caracteres.

### Ejemplo

```text
Cadena: "Hola"

Índice:     0   1   2   3
Caracter:   H   o   l   a
```

Cada carácter ocupa una posición específica dentro de la cadena.

---

# Cadenas en C++

En C++ existen dos formas comunes de trabajar con texto:

| Tipo     | Descripción                             |
| -------- | --------------------------------------- |
| `char[]` | Arreglo de caracteres.                  |
| `string` | Clase especializada para manejar texto. |

---

# Uso de string

Para utilizar cadenas mediante `string` se requiere:

```cpp
#include <string>
```

### Declaración

```cpp
string nombre;
```

### Inicialización

```cpp
string nombre = "Juan";
```

---

# Entrada y salida de cadenas

### Lectura

```cpp
string nombre;
cin >> nombre;
```

### Escritura

```cpp
cout << nombre;
```

---

# Ejemplo completo

```cpp
#include <iostream>
#include <string>

using namespace std;

int main() {
    string nombre;

    cout << "Ingrese su nombre: ";
    cin >> nombre;

    cout << "Hola " << nombre << endl;

    return 0;
}
```

---

# Operaciones básicas

## Concatenación

Permite unir cadenas.

### Ejemplo

```cpp
string nombre = "Juan";
string apellido = "Perez";

string completo = nombre + " " + apellido;
```

Resultado:

```text
Juan Perez
```

---

## Longitud

Permite conocer la cantidad de caracteres.

### Ejemplo

```cpp
string palabra = "Hola";

cout << palabra.length();
```

Resultado:

```text
4
```

---

## Acceso a caracteres

Cada carácter puede accederse mediante un índice.

### Ejemplo

```cpp
string palabra = "Hola";

cout << palabra[0];
```

Resultado:

```text
H
```

---

# Ventajas de string

| Ventaja                    | Descripción                          |
| -------------------------- | ------------------------------------ |
| Facilidad de uso           | Simplifica el manejo de texto.       |
| Seguridad                  | Reduce errores comunes.              |
| Funcionalidades integradas | Permite realizar operaciones útiles. |
| Legibilidad                | Hace el código más claro.            |

---

# Aplicaciones

Las cadenas se utilizan en:

* Nombres de usuarios.
* Direcciones.
* Mensajes.
* Contraseñas.
* Sistemas de búsqueda.
* Procesamiento de texto.

---

# Errores comunes

| Error                                       | Descripción                                  |
| ------------------------------------------- | -------------------------------------------- |
| Confundir `char` con `string`               | No representan lo mismo.                     |
| Acceder a índices inexistentes              | Puede producir errores.                      |
| Olvidar incluir `<string>`                  | Impide utilizar `string`.                    |
| Suponer que una cadena es un único carácter | Una cadena puede contener muchos caracteres. |

---

# Información complementaria

Para comprender mejor los conceptos relacionados, consulte:

* [Código ASCII](../Tema02_Datos/02-codigo_ascii.md)
* [Tablas](02-tablas.md)

---

# Conclusión

Las cadenas permiten almacenar y manipular texto dentro de los programas. Constituyen una herramienta fundamental para la interacción con usuarios y el procesamiento de información textual.

---

# Resumen

| Concepto             | Idea principal                                 |
| -------------------- | ---------------------------------------------- |
| Cadena               | Secuencia de caracteres.                       |
| Carácter             | Unidad individual representada por `char`.     |
| string               | Tipo utilizado para trabajar con texto en C++. |
| Índice               | Posición de un carácter dentro de la cadena.   |
| Aplicación principal | Almacenamiento y procesamiento de texto.       |
