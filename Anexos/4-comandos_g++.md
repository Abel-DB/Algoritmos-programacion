# Comandos de G++

## ¿Qué es G++?

**G++** es el compilador de C++ incluido dentro de GCC (GNU Compiler Collection).

Su función es transformar el código fuente escrito en C++ en un programa ejecutable.

---

# Flujo de compilación

```text
Código Fuente (.cpp)
        ↓
       G++
        ↓
   Ejecutable
        ↓
    Ejecución
```

---

# Verificar instalación

Permite comprobar si G++ está instalado.

```bash
g++ --version
```

### Ejemplo

```text
g++ (GCC) 14.x.x
```

---

# Compilación básica

## Compilar un archivo

```bash
g++ main.cpp
```

Genera un ejecutable llamado:

```text
a.out
```

---

# Ejecutar programa

```bash
./a.out
```

---

# Especificar nombre del ejecutable

## Compilar

```bash
g++ main.cpp -o programa
```

## Ejecutar

```bash
./programa
```

---

# Compilar varios archivos

## Ejemplo

```bash
g++ main.cpp funciones.cpp utilidades.cpp -o programa
```

---

# Mostrar advertencias

Las advertencias ayudan a detectar posibles errores.

```bash
g++ -Wall main.cpp -o programa
```

---

# Advertencias adicionales

```bash
g++ -Wall -Wextra main.cpp -o programa
```

### Recomendación

Utilizar siempre:

```bash
g++ -Wall -Wextra
```

durante el aprendizaje.

---

# Estándares de C++

G++ permite seleccionar la versión del lenguaje.

## C++11

```bash
g++ -std=c++11 main.cpp -o programa
```

---

## C++17

```bash
g++ -std=c++17 main.cpp -o programa
```

---

## C++20

```bash
g++ -std=c++20 main.cpp -o programa
```

---

## C++23

```bash
g++ -std=c++23 main.cpp -o programa
```

---

# Compilación recomendada

Para la mayoría de ejercicios:

```bash
g++ -std=c++20 -Wall -Wextra main.cpp -o programa
```

---

# Generar información para depuración

Permite utilizar GDB.

```bash
g++ -g main.cpp -o programa
```

---

# Optimización

## Nivel básico

```bash
g++ -O1 main.cpp -o programa
```

---

## Nivel medio

```bash
g++ -O2 main.cpp -o programa
```

---

## Nivel alto

```bash
g++ -O3 main.cpp -o programa
```

### Nota

Durante el aprendizaje normalmente no es necesario utilizar optimizaciones.

---

# Compilar y ejecutar

## Método tradicional

```bash
g++ main.cpp -o programa

./programa
```

---

## Una sola línea

```bash
g++ main.cpp -o programa && ./programa
```

---

# Archivos de cabecera

Cuando se utilizan archivos `.h` y `.cpp`:

```text
main.cpp
calculadora.cpp
calculadora.h
```

Compilación:

```bash
g++ main.cpp calculadora.cpp -o programa
```

---

# Uso con Make

Cuando el proyecto crece, la compilación suele automatizarse mediante Make.

```bash
make
```

> Consulte: Herramientas de Desarrollo.

---

# Uso con CMake

En proyectos medianos y grandes suele utilizarse CMake.

```bash
cmake -B build

cmake --build build
```

---

# Errores frecuentes

## Archivo no encontrado

```text
fatal error: archivo.cpp: No such file or directory
```

### Causa

Nombre incorrecto o archivo inexistente.

---

## Error de sintaxis

```text
expected ';'
```

### Causa

Falta de punto y coma.

---

## Función no definida

```text
undefined reference
```

### Causa

Se olvidó compilar algún archivo fuente.

---

# Buenas prácticas

| Práctica                      | Recomendación   |
| ----------------------------- | --------------- |
| Utilizar advertencias         | `-Wall -Wextra` |
| Especificar estándar          | `-std=c++20`    |
| Usar nombres descriptivos     | `-o programa`   |
| Utilizar GDB para depuración  | `-g`            |
| Automatizar proyectos grandes | Make o CMake    |

---

# Comandos más utilizados

## Ver versión

```bash
g++ --version
```

---

## Compilar

```bash
g++ main.cpp -o programa
```

---

## Compilar con advertencias

```bash
g++ -Wall -Wextra main.cpp -o programa
```

---

## Compilar con C++20

```bash
g++ -std=c++20 -Wall -Wextra main.cpp -o programa
```

---

## Depuración

```bash
g++ -g main.cpp -o programa
```

---

## Ejecutar

```bash
./programa
```

---

# Información complementaria

Consulte:

* Herramientas de Desarrollo
* Buenas Prácticas en C++
* GDB
* Make
* CMake

---

# Conclusión

G++ es una de las herramientas fundamentales para el desarrollo en C++. Dominar sus comandos básicos permite compilar, ejecutar y depurar programas de manera eficiente.

---

# Resumen

| Comando           | Función                  |
| ----------------- | ------------------------ |
| `g++ archivo.cpp` | Compilar                 |
| `-o`              | Nombre del ejecutable    |
| `-Wall`           | Advertencias             |
| `-Wextra`         | Advertencias adicionales |
| `-std=c++20`      | Estándar del lenguaje    |
| `-g`              | Depuración               |
| `./programa`      | Ejecutar                 |
