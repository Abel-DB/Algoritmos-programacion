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

Todo módulo está compuesto por dos partes.

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

## 4. Responsabilidad única

Cada módulo debe encargarse de realizar una única tarea específica.

Esto mejora la organización del programa y facilita su mantenimiento.

### Correcto

```text
Funcion CalcularPromedio()
```

### Incorrecto

```text
Funcion CalcularPromedioYGuardarYMostrar()
```

---

## 5. Intercambio de información

Los módulos pueden recibir datos, procesarlos y devolver resultados.

La comunicación entre módulos permite construir programas complejos a partir de componentes simples e independientes.

### Ejemplo

```text
promedio <- CalcularPromedio(nota1, nota2, nota3)
```

El módulo recibe datos, realiza un procesamiento y devuelve un resultado.

---

## Resumen

Las principales características del diseño modular son:

- Nombre único.
- Parámetros de comunicación.
- Cabecera y cuerpo.
- Responsabilidad única.
- Intercambio de información entre módulos.
