# Características del Diseño Modular

## Introducción

El diseño modular se basa en la división de un programa en módulos o subprogramas independientes que colaboran entre sí para resolver un problema.

Para que esta división sea efectiva, los módulos deben cumplir ciertas características.

---

## 1. Nombre único

Cada módulo debe poseer un identificador único que permita distinguirlo de los demás.

El nombre del módulo se utiliza para invocarlo desde otras partes del programa.

### Ejemplo

```text
Funcion Sumar()
Funcion Restar()
```

Cada función tiene un nombre diferente.

---

## 2. Parámetros de comunicación

Los módulos pueden intercambiar información mediante parámetros.

Los parámetros permiten enviar datos al módulo para que realice una tarea específica.

### Ejemplo

```text
Funcion Sumar(a, b)
```

Los valores `a` y `b` son parámetros de entrada.

---

## 3. Cabecera y cuerpo

Todo módulo está compuesto por dos partes:

### Cabecera

Contiene:

- Nombre del módulo.
- Lista de parámetros.

### Cuerpo

Contiene:

- Declaración de variables.
- Instrucciones.
- Procesos necesarios para cumplir la tarea.

### Ejemplo

```text
Funcion Sumar(a, b)

    resultado <- a + b

    Retornar resultado

FinFuncion
```

---

## 4. Facilita el trabajo en equipo

La división del programa en módulos permite que varios programadores trabajen simultáneamente en diferentes partes del sistema.

Cada integrante puede desarrollar un módulo específico sin afectar directamente a los demás.

---

## 5. Realiza una tarea específica

Cada módulo debe tener una única responsabilidad.

Esto mejora la organización y facilita el mantenimiento del código.

### Correcto

```text
Funcion CalcularPromedio()
```

### Incorrecto

```text
Funcion CalcularPromedioYGuardarYMostrar()
```

---

## 6. Intercambio de información

Los módulos pueden recibir datos, procesarlos y devolver resultados.

La comunicación entre módulos permite construir programas más complejos a partir de componentes simples.

---

## Resumen

Las principales características del diseño modular son:

- Nombre único.
- Parámetros de comunicación.
- Cabecera y cuerpo.
- Facilita el trabajo en equipo.
- Una tarea específica por módulo.
- Intercambio de información entre módulos.
