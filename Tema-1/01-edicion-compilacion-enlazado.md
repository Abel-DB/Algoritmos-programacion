# Edición, compilación y enlazado de un programa

## Introducción
Un programa es un conjunto de instrucciones escritas en un lenguaje de programación que permiten resolver un problema o realizar una tarea en la computadora. Sin embargo, la computadora no entiende directamente estos lenguajes, sino que necesita que el código sea transformado a lenguaje máquina.

Para que un programa pueda ejecutarse, pasa por tres etapas principales: edición, compilación y enlazado.

---

## 1. Edición
La **edición** es la etapa en la que el programador escribe el código fuente utilizando un lenguaje de programación.

Este proceso se realiza en un editor de código y el resultado es un archivo que contiene instrucciones que aún no pueden ser ejecutadas directamente por la computadora.

Los archivos de código fuente tienen diferentes extensiones según el lenguaje:
- `.cpp` para C++
- `.py` para Python

Durante la edición se pueden realizar modificaciones, correcciones y mejoras al código, pero todavía no se ejecuta.

### Ejemplo en C++
```cpp
    #include <iostream>
    int main() {
        std::cout << "Hola";
        return 0;
    }
```

### Ejemplo en Python
```Python
    print("Hola")
```

---

## 2. Compilación
La **compilación** es el proceso mediante el cual el código fuente se traduce a lenguaje máquina, que es el único lenguaje que entiende la computadora.

Este proceso es realizado por un programa llamado **compilador**.

Durante la compilación:
- Se revisa la sintaxis del programa
- Se detectan errores
- Se genera un archivo ejecutable (en lenguajes como C++)

Si el código contiene errores, la compilación falla y el programa no puede ejecutarse.

### Ejemplo en C++
```cpp
    g++ programa.cpp -o programa
```

Este comando compila el código y genera un archivo ejecutable llamado `programa`.

### Ejemplo de error
```Python
    int x = ;
```

Este código produce un error de compilación porque está mal escrito.

### En Python
En Python no existe compilación manual. El código se ejecuta directamente mediante un intérprete, aunque internamente Python realiza una traducción automática.

---

## 3. Enlazado (Linking)
El **enlazado** es el proceso en el que el programa se conecta con librerías externas que contienen funciones previamente definidas.

Estas librerías permiten utilizar funcionalidades sin tener que programarlas desde cero.

El enlazador se encarga de unir el código del programa con estas librerías para formar un programa completo.

### Ejemplo en C++
```cpp
    #include <iostream>
```

Esta línea permite usar funciones como:
- `cout`
- `endl`

### Ejemplo en Python
```Python
    import math
```

Permite utilizar funciones como:
- `sqrt()`
- `pow()`

### Importancia
Si el enlazado falla:
- El programa no podrá ejecutarse correctamente
- Se producirán errores relacionados con funciones no encontradas

---

## Relación entre las etapas
El proceso completo se puede resumir de la siguiente manera:

Edición → Compilación → Enlazado → Ejecución

- En la edición se escribe el programa  
- En la compilación se traduce  
- En el enlazado se agregan las librerías necesarias  

---

## Diferencia entre C++ y Python

| Etapa        | C++                | Python              |
|--------------|------------------|--------------------|
| Edición      | Sí               | Sí                 |
| Compilación  | Sí (manual)      | No visible         |
| Enlazado     | Sí               | Automático         |
| Ejecución    | Ejecutable       | Intérprete         |

---

## Resumen final
- La **edición** consiste en escribir el código fuente  
- La **compilación** traduce el código a lenguaje máquina y detecta errores  
- El **enlazado** une el programa con librerías externas necesarias  

---

## Idea clave
Primero se escribe el programa (edición), luego se traduce (compilación) y finalmente se enlaza con librerías para poder ejecutarlo correctamente.
