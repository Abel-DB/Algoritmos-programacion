# Git y GitHub

## ¿Qué es Git?

Git es un sistema de control de versiones distribuido que permite registrar y administrar los cambios realizados en un proyecto.

Fue creado por Linus Torvalds en 2005 para el desarrollo del kernel Linux.

---

# ¿Qué es GitHub?

GitHub es una plataforma basada en Git que permite almacenar repositorios de forma remota, colaborar con otros desarrolladores y gestionar proyectos.

---

# ¿Por qué utilizar Git?

Git permite:

* Guardar el historial de cambios.
* Recuperar versiones anteriores.
* Trabajar en equipo.
* Evitar pérdida de código.
* Organizar proyectos.

---

# Conceptos fundamentales

| Concepto    | Descripción                    |
| ----------- | ------------------------------ |
| Repositorio | Carpeta controlada por Git     |
| Commit      | Punto de guardado del proyecto |
| Branch      | Rama de desarrollo             |
| Merge       | Unión de ramas                 |
| Remote      | Repositorio remoto             |
| Clone       | Copiar repositorio remoto      |
| Push        | Enviar cambios                 |
| Pull        | Descargar cambios              |

---

# Flujo de trabajo básico

```text
Modificar archivos
        ↓
git add
        ↓
git commit
        ↓
git push
        ↓
GitHub
```

---

# Configuración inicial

## Nombre de usuario

```bash
git config --global user.name "Tu Nombre"
```

---

## Correo electrónico

```bash
git config --global user.email "correo@ejemplo.com"
```

---

## Ver configuración

```bash
git config --list
```

---

# Crear repositorio

## Inicializar proyecto

```bash
git init
```

Se crea el directorio:

```text
.git
```

que contiene toda la información del repositorio.

---

# Estado del repositorio

## Ver estado

```bash
git status
```

Permite visualizar:

* Archivos modificados.
* Archivos nuevos.
* Archivos preparados para commit.

---

# Agregar cambios

## Agregar archivo específico

```bash
git add archivo.cpp
```

---

## Agregar todos los archivos

```bash
git add .
```

---

# Crear commit

## Guardar cambios

```bash
git commit -m "Agregar tema de variables"
```

---

# Historial

## Ver commits

```bash
git log
```

---

## Historial resumido

```bash
git log --oneline
```

---

# Trabajar con GitHub

## Clonar repositorio

```bash
git clone URL_REPOSITORIO
```

Ejemplo:

```bash
git clone https://github.com/usuario/proyecto.git
```

---

# Conectar repositorio local

```bash
git remote add origin URL_REPOSITORIO
```

---

# Ver repositorios remotos

```bash
git remote -v
```

---

# Enviar cambios

## Primer envío

```bash
git push -u origin main
```

---

## Envíos posteriores

```bash
git push
```

---

# Descargar cambios

```bash
git pull
```

---

# Ramas

## Ver ramas

```bash
git branch
```

---

## Crear rama

```bash
git branch desarrollo
```

---

## Cambiar de rama

```bash
git checkout desarrollo
```

---

## Crear y cambiar

```bash
git checkout -b desarrollo
```

---

# Fusionar ramas

```bash
git merge desarrollo
```

---

# Ignorar archivos

## .gitignore

Permite excluir archivos que no deben ser versionados.

### Ejemplo

```text
*.o
*.exe
build/
.vscode/
```

---

# Proyecto C++

## Estructura típica

```text
Proyecto/
│
├── src/
├── include/
├── build/
├── CMakeLists.txt
├── README.md
└── .gitignore
```

---

# Flujo recomendado para la universidad

## Crear proyecto

```bash
mkdir proyecto
cd proyecto
git init
```

---

## Crear README

```bash
touch README.md
```

---

## Primer commit

```bash
git add .
git commit -m "Primer commit"
```

---

## Conectar GitHub

```bash
git remote add origin URL
git push -u origin main
```

---

# Buenas prácticas

| Práctica                 | Recomendación                |
| ------------------------ | ---------------------------- |
| Commits frecuentes       | Guardar cambios pequeños     |
| Mensajes descriptivos    | Explicar qué cambió          |
| Utilizar .gitignore      | Evitar archivos innecesarios |
| Mantener README          | Documentar proyectos         |
| Hacer pull antes de push | Evitar conflictos            |

---

# Ejemplos de mensajes de commit

## Correctos

```text
Agregar tema de variables

Corregir errores de compilación

Actualizar apuntes de estructuras

Implementar ejercicio de ciclos
```

---

## Incorrectos

```text
Cambios

asd

Prueba

Arreglo
```

---

# Errores frecuentes

## Olvidar agregar archivos

```bash
git add .
```

---

## Push sin repositorio remoto

```text
fatal: no configured push destination
```

### Solución

```bash
git remote add origin URL
```

---

## Conflictos de fusión

Ocurren cuando dos versiones modifican la misma parte de un archivo.

---

# Comandos más utilizados

## Estado

```bash
git status
```

## Agregar

```bash
git add .
```

## Commit

```bash
git commit -m "mensaje"
```

## Historial

```bash
git log --oneline
```

## Enviar

```bash
git push
```

## Descargar

```bash
git pull
```

---

# Mi flujo de trabajo

```text
Neovim
   ↓
Guardar archivo
   ↓
git add .
   ↓
git commit -m "mensaje"
   ↓
git push
   ↓
GitHub
```

---

# Relación con otras herramientas

Git se integra con:

* Linux
* Zsh
* Kitty
* Neovim
* NvChad
* GCC / G++
* Clang / Clang++
* CMake
* Make

---

# Conclusión

Git y GitHub son herramientas fundamentales para cualquier desarrollador. Permiten mantener un historial completo de los proyectos, colaborar con otros programadores y trabajar de forma segura y organizada.

---

# Resumen

| Comando    | Función            |
| ---------- | ------------------ |
| git init   | Crear repositorio  |
| git status | Ver estado         |
| git add .  | Agregar cambios    |
| git commit | Crear commit       |
| git log    | Ver historial      |
| git clone  | Clonar repositorio |
| git pull   | Descargar cambios  |
| git push   | Enviar cambios     |
| git branch | Administrar ramas  |
| git merge  | Fusionar ramas     |
