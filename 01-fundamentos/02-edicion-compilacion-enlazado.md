# Edición, Compilación y Enlazado

## ¿Qué es el proceso de desarrollo de un programa?

Antes de que un programa pueda ejecutarse, debe pasar por varias etapas que transforman el código escrito por el programador en un archivo ejecutable.

Estas etapas permiten detectar errores y preparar el programa para su ejecución.

---

# Importancia

Comprender este proceso permite:

* Entender cómo se construye un programa.
* Identificar errores durante el desarrollo.
* Diferenciar las etapas de creación de software.
* Facilitar la corrección de problemas.

---

# Etapas del proceso

| Etapa       | Descripción                                    |
| ----------- | ---------------------------------------------- |
| Edición     | Escritura del código fuente.                   |
| Compilación | Traducción del código a lenguaje máquina.      |
| Enlazado    | Unión del código con las librerías necesarias. |
| Ejecución   | Funcionamiento del programa.                   |

---

# 1. Edición

Es la etapa donde el programador escribe el código fuente utilizando un editor de texto o un entorno de desarrollo integrado (IDE).

Durante esta etapa se crean y modifican los archivos que contienen las instrucciones del programa.

### Herramientas comunes

| Herramienta        | Tipo   |
| ------------------ | ------ |
| Neovim (nvim)      | Editor |
| Vim                | Editor |
| Visual Studio Code | Editor |
| Code::Blocks       | IDE    |
| Dev-C++            | IDE    |
| Visual Studio      | IDE    |
| CLion              | IDE    |

### Nota

La etapa de edición no depende de una herramienta específica. Un programa puede escribirse utilizando editores ligeros como **Neovim** o **Vim**, o mediante entornos de desarrollo completos (IDE) como **Code::Blocks**, **Visual Studio** o **CLion**.

---

# 2. Compilación

Es el proceso mediante el cual el compilador traduce el código fuente a lenguaje máquina.

Su función principal es verificar que las instrucciones estén correctamente escritas y generar un archivo intermedio que posteriormente será enlazado.

### Funciones principales

* Traducir el código fuente.
* Detectar errores de sintaxis.
* Generar código objeto.

### Errores de compilación

| Tipo de error  | Descripción                 |
| -------------- | --------------------------- |
| Sintaxis       | Instrucciones mal escritas. |
| Variables      | Variables no declaradas.    |
| Tipos de datos | Uso incorrecto de tipos.    |

---

# 3. Enlazado

Es la etapa donde se unen los archivos generados durante la compilación con las librerías necesarias para el funcionamiento del programa.

### Funciones principales

* Incorporar librerías.
* Resolver referencias externas.
* Generar el ejecutable final.

### Posibles errores

| Error               | Causa                                  |
| ------------------- | -------------------------------------- |
| Librería faltante   | No se encuentra una dependencia.       |
| Función no definida | Existe una llamada sin implementación. |

---

# 4. Ejecución

Una vez generado el ejecutable, el sistema operativo carga el programa en memoria y comienza su ejecución.

Durante esta etapa pueden aparecer errores de ejecución o errores lógicos.

---

# Flujo general del proceso

```text
Código Fuente
      ↓
    Edición
      ↓
  Compilación
      ↓
   Enlazado
      ↓
 Programa Ejecutable
      ↓
   Ejecución
```

---

# Tipos de errores

| Tipo      | Momento en que aparece                                     |
| --------- | ---------------------------------------------------------- |
| Sintaxis  | Durante la compilación.                                    |
| Enlazado  | Durante el enlazado.                                       |
| Ejecución | Mientras el programa se ejecuta.                           |
| Lógico    | El programa funciona, pero produce resultados incorrectos. |

---

# Ejemplo del proceso

1. Escribir un programa en C++.
2. Guardar el archivo fuente.
3. Compilar el programa.
4. Corregir errores si existen.
5. Enlazar las librerías necesarias.
6. Generar el ejecutable.
7. Ejecutar el programa.

---

# Aplicaciones

Este proceso se utiliza en la mayoría de los lenguajes compilados:

* C
* C++
* Rust
* Go
* Pascal

---

# Conclusión

La edición, compilación y enlazado son etapas fundamentales en el desarrollo de software. Comprender este proceso permite identificar errores con mayor facilidad y entender cómo un programa pasa de ser código fuente a convertirse en una aplicación ejecutable.

---

# Resumen

| Concepto        | Idea principal                              |
| --------------- | ------------------------------------------- |
| Edición         | Escritura y modificación del código fuente. |
| Compilación     | Traducción del código a lenguaje máquina.   |
| Enlazado        | Unión del código con librerías y recursos.  |
| Ejecución       | Funcionamiento del programa.                |
| Resultado final | Programa ejecutable.                        |
