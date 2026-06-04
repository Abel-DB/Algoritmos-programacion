# Compilación y Enlazado en C++

## Introducción

Antes de que un programa pueda ejecutarse, debe pasar por varias etapas que transforman el código fuente en un archivo ejecutable.

Comprender este proceso ayuda a identificar errores y entender cómo se construyen los programas en C++.

---

# Flujo General

```text
Código Fuente (.cpp)
        ↓
    Compilación
        ↓
 Código Objeto (.o)
        ↓
     Enlazado
        ↓
    Ejecutable
        ↓
     Ejecución
```

---

# 1. Edición

Es la etapa donde se escribe el código fuente.

Ejemplo:

```bash
nvim main.cpp
nvim suma.cpp
```

Archivos creados:

```text
main.cpp
suma.cpp
```

---

# 2. Compilación

La compilación transforma cada archivo fuente (`.cpp`) en un archivo objeto (`.o`).

Ejemplo:

```bash
g++ -c main.cpp
g++ -c suma.cpp
```

Resultado:

```text
main.o
suma.o
```

### Características

* Traduce el código fuente a código máquina.
* Detecta errores de sintaxis.
* Genera archivos objeto.
* Todavía no existe un ejecutable.

---

# 3. Enlazado

El enlazado une los archivos objeto y las bibliotecas necesarias para crear el programa ejecutable.

Ejemplo:

```bash
g++ main.o suma.o -o programa
```

Resultado:

```text
programa
```

### Funciones del enlazador

* Une múltiples archivos objeto.
* Resuelve llamadas a funciones externas.
* Conecta las bibliotecas necesarias.
* Genera el ejecutable final.

---

# Ejemplo Práctico

Archivo `suma.cpp`

```cpp
int suma(int a, int b) {
    return a + b;
}
```

Archivo `main.cpp`

```cpp
#include <iostream>

int suma(int, int);

int main() {
    std::cout << suma(3, 4);
}
```

Compilación:

```bash
g++ -c suma.cpp
g++ -c main.cpp
```

Enlazado:

```bash
g++ main.o suma.o -o programa
```

Ejecución:

```bash
./programa
```

Salida:

```text
7
```

---

# Error Común

Modificar un archivo fuente y olvidar recompilarlo.

Ejemplo:

```text
Modificar main.cpp
↓
No recompilar main.cpp
↓
main.o queda desactualizado
↓
El ejecutable utiliza una versión antigua del código
```

Solución:

```bash
g++ -c main.cpp
g++ main.o suma.o -o programa
```

---

# 4. Ejecución

Una vez generado el ejecutable, puede ejecutarse desde la terminal.

```bash
./programa
```

Durante esta etapa el sistema operativo carga el programa en memoria y comienza la ejecución desde la función `main()`.

---

# Resumen

| Etapa       | Acción                          |
| ----------- | ------------------------------- |
| Edición     | Escribir código fuente (`.cpp`) |
| Compilación | Generar archivos objeto (`.o`)  |
| Enlazado    | Crear el ejecutable             |
| Ejecución   | Ejecutar el programa            |

---

# Ejemplo Completo

```bash
g++ -c main.cpp
g++ -c suma.cpp

g++ main.o suma.o -o programa

./programa
```

---

# Idea Clave

Un archivo `.cpp` no se convierte directamente en un programa ejecutable.

El proceso habitual es:

```text
.cpp
 ↓
.o
 ↓
ejecutable
 ↓
ejecución
```

Comprender esta secuencia facilita el desarrollo de programas en C++ y ayuda a identificar errores de compilación y enlazado.
