# Diseño Modular

## Definición

El diseño modular es una metodología de programación que consiste en dividir un programa en módulos o subprogramas independientes, donde cada uno se encarga de realizar una tarea específica.

Un programa modular se organiza alrededor de un **módulo principal** que coordina la ejecución del resto de módulos.

Cuando el módulo principal invoca a otro módulo, el control de ejecución se transfiere a dicho módulo. Una vez finalizada su ejecución, el control regresa al punto desde donde fue llamado.

---

## Estructura general

```text
Programa Principal
│
├── Módulo A
├── Módulo B
└── Módulo C
```

Cada módulo puede, a su vez, llamar a otros módulos si es necesario.

---

## Funcionamiento

1. El programa principal recibe el control al iniciar la ejecución.
2. Se invoca un módulo para realizar una tarea específica.
3. El módulo ejecuta sus instrucciones.
4. Finalizada la tarea, devuelve el control al módulo que realizó la llamada.
5. La ejecución continúa desde la instrucción siguiente.

---

## Objetivos del diseño modular

- Dividir problemas complejos en partes más pequeñas.
- Reutilizar código.
- Facilitar el mantenimiento.
- Mejorar la legibilidad de los programas.
- Permitir el desarrollo colaborativo.

---

## Conceptos importantes

### Módulo principal

Es el punto de entrada del programa y coordina la ejecución de los demás módulos.

### Subprograma

Bloque de código independiente que realiza una tarea específica y puede ser invocado desde otras partes del programa.

### Llamada a módulo

Proceso mediante el cual un módulo transfiere el control de ejecución a otro módulo.

### Retorno de control

Una vez finalizada la ejecución de un módulo, el control vuelve al módulo que realizó la llamada.

---

## Resumen

El diseño modular divide un programa en componentes independientes llamados módulos o subprogramas. Cada módulo cumple una función específica y puede ser reutilizado, facilitando el desarrollo, mantenimiento y comprensión del software.
