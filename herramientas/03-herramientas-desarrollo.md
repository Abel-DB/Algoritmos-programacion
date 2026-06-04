# Herramientas de Desarrollo

## ¿Qué son las herramientas de desarrollo?

Las herramientas de desarrollo son programas que permiten crear, editar, compilar, ejecutar, depurar y administrar proyectos de software.

Constituyen el entorno de trabajo del programador y facilitan el desarrollo de aplicaciones de manera eficiente y organizada.

---

# Importancia

Las herramientas de desarrollo permiten:

* Escribir código.
* Compilar programas.
* Ejecutar aplicaciones.
* Detectar errores.
* Administrar proyectos.
* Controlar versiones.
* Automatizar tareas.

---

# Clasificación

| Categoría            | Herramientas             |
| -------------------- | ------------------------ |
| Sistema Operativo    | Linux, EndeavourOS       |
| Shell                | Zsh                      |
| Terminal             | Kitty                    |
| Editor               | Neovim, NvChad           |
| Compiladores         | GCC, G++, Clang, Clang++ |
| Análisis de Código   | Clangd                   |
| Construcción         | Make, CMake              |
| Depuración           | GDB                      |
| Control de Versiones | Git                      |
| Repositorios Remotos | GitHub                   |

---

# Sistema Operativo

## Linux

Linux es un sistema operativo libre y de código abierto ampliamente utilizado en desarrollo de software.

### Ventajas

* Estabilidad.
* Seguridad.
* Personalización.
* Amplia disponibilidad de herramientas de desarrollo.

---

## EndeavourOS

EndeavourOS es una distribución basada en Arch Linux.

### Características

* Sistema ligero.
* Acceso a los repositorios de Arch.
* Actualizaciones continuas.
* Gran capacidad de personalización.

---

# Shell

## Zsh

Z Shell (Zsh) es un intérprete de comandos avanzado compatible con Bash.

### Ventajas

* Autocompletado mejorado.
* Historial avanzado.
* Personalización.
* Productividad en terminal.

---

# Terminal

## Kitty

Kitty es un emulador de terminal moderno orientado al rendimiento.

### Características

* Alta velocidad.
* Soporte para Unicode.
* Multiplexación de ventanas.
* Configuración sencilla.

---

# Editor de Código

## Neovim

Neovim es un editor de texto orientado al desarrollo de software.

### Ventajas

* Ligero.
* Rápido.
* Altamente configurable.
* Orientado al uso del teclado.

### Funciones

* Edición de código.
* Navegación de proyectos.
* Integración con herramientas externas.
* Soporte para múltiples lenguajes.

---

## NvChad

NvChad es una configuración predefinida para Neovim.

### Ventajas

* Configuración moderna.
* Interfaz mejorada.
* Integración con LSP.
* Productividad inmediata.

---

# Compiladores

## GCC

GNU Compiler Collection es una colección de compiladores desarrollada por GNU.

### Uso principal

```text
Lenguaje C
```

---

## G++

Compilador de C++ incluido dentro de GCC.

### Uso principal

```text
Lenguaje C++
```

### Ejemplo

```bash
g++ main.cpp -o programa
```

---

## Clang

Compilador desarrollado dentro del proyecto LLVM.

### Uso principal

```text
Lenguaje C
```

---

## Clang++

Versión de Clang orientada al lenguaje C++.

### Ventajas

* Mensajes de error más descriptivos.
* Integración con herramientas modernas.
* Excelente soporte para estándares recientes de C++.

### Ejemplo

```bash
clang++ main.cpp -o programa
```

---

# Análisis de Código

## Clangd

Clangd es un servidor de lenguaje (LSP) basado en Clang.

### Funciones

* Autocompletado.
* Navegación de código.
* Diagnóstico de errores.
* Refactorización.

### Integración

Se utiliza habitualmente junto con:

* Neovim
* NvChad

---

# Construcción de Proyectos

## Make

Make automatiza la compilación de proyectos mediante archivos Makefile.

### Ventajas

* Automatización.
* Compilación incremental.
* Organización de proyectos.

---

## CMake

CMake es una herramienta para generar sistemas de construcción.

### Ventajas

* Multiplataforma.
* Compatible con múltiples compiladores.
* Utilizado ampliamente en proyectos profesionales de C++.

### Flujo básico

```text
Código Fuente
      ↓
CMake
      ↓
Make / Ninja
      ↓
Ejecutable
```

---

# Depuración

## GDB

GNU Debugger es una herramienta utilizada para analizar programas durante su ejecución.

### Permite

* Detectar errores.
* Inspeccionar variables.
* Ejecutar paso a paso.
* Analizar fallos.

---

# Control de Versiones

## Git

Git es un sistema de control de versiones distribuido.

### Ventajas

* Historial de cambios.
* Recuperación de versiones anteriores.
* Trabajo colaborativo.
* Organización de proyectos.

### Comandos básicos

```bash
git init
git add .
git commit -m "mensaje"
git status
```

---

## GitHub

GitHub es una plataforma basada en Git para almacenar repositorios remotos.

### Funciones

* Hospedaje de proyectos.
* Trabajo colaborativo.
* Gestión de versiones.
* Documentación.

---

# Mi Entorno de Desarrollo

## Sistema Operativo

* Linux
* EndeavourOS

## Shell

* Zsh

## Terminal

* Kitty

## Editor

* Neovim
* NvChad

## Compiladores

* GCC
* G++
* Clang
* Clang++

## Análisis de Código

* Clangd

## Construcción

* Make
* CMake

## Depuración

* GDB

## Control de Versiones

* Git
* GitHub

---

# Flujo de Trabajo General

```text
Neovim / NvChad
        ↓
      Clangd
        ↓
Código Fuente
        ↓
 G++ / Clang++
        ↓
 Make / CMake
        ↓
 Ejecutable
        ↓
      GDB
        ↓
 Git / GitHub
```

---

# Información complementaria

Consulte:

* Comandos de g++
* Atajos de Neovim
* Buenas prácticas en C++
* Convenciones de nombres

---

# Conclusión

Las herramientas de desarrollo constituyen el entorno de trabajo del programador. Dominar estas herramientas permite aumentar la productividad, mejorar la calidad del software y facilitar el desarrollo de proyectos profesionales.

---

# Resumen

| Categoría         | Herramientas             |
| ----------------- | ------------------------ |
| Sistema Operativo | Linux, EndeavourOS       |
| Shell             | Zsh                      |
| Terminal          | Kitty                    |
| Editor            | Neovim, NvChad           |
| Compiladores      | GCC, G++, Clang, Clang++ |
| Análisis          | Clangd                   |
| Construcción      | Make, CMake              |
| Depuración        | GDB                      |
| Versionado        | Git, GitHub              |
