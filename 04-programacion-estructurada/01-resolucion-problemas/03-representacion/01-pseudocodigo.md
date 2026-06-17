# Pseudocódigo

## ¿Qué es el pseudocódigo?

El **pseudocódigo** es una forma de representar algoritmos mediante instrucciones escritas en lenguaje natural estructurado.

Su objetivo es describir la lógica de una solución sin depender de la sintaxis de un lenguaje de programación específico.

---

# Importancia

El pseudocódigo permite:

- Diseñar algoritmos antes de programar.
- Comprender mejor la lógica de una solución.
- Detectar errores tempranamente.
- Facilitar la comunicación entre personas.
- Servir como puente entre la solución y su implementación.

---

# Características

| Característica | Descripción |
|----------------|-------------|
| Independiente del lenguaje | No pertenece a ningún lenguaje de programación. |
| Fácil de leer | Utiliza lenguaje cercano al humano. |
| Estructurado | Sigue una secuencia lógica. |
| Flexible | Puede adaptarse a distintos problemas. |

---

# Elementos básicos

| Elemento | Función |
|----------|----------|
| Leer | Obtener datos de entrada. |
| Escribir | Mostrar resultados. |
| Asignar | Almacenar valores en variables. |
| Operar | Realizar cálculos o procesos. |
| Decidir | Evaluar condiciones. |
| Repetir | Ejecutar acciones varias veces. |

---

# Reglas básicas para escribir pseudocódigo

Para mantener claridad y uniformidad se recomienda:

- Utilizar instrucciones simples y precisas.
- Escribir una acción por línea.
- Mantener una secuencia lógica.
- Utilizar sangría para mostrar bloques.
- Evitar sintaxis completa de un lenguaje de programación.
- Utilizar nombres descriptivos para las variables.

---

# Estructura general

```text
Inicio

    Instrucciones

Fin
```

Todo algoritmo debe poseer un inicio y un final claramente definidos.

---

# Estructuras básicas del pseudocódigo

Los algoritmos suelen construirse utilizando tres estructuras fundamentales.

## 1. Estructura secuencial

Las instrucciones se ejecutan una después de otra.

### Ejemplo

```text
Inicio

    Leer A
    Leer B

    suma = A + B

    Escribir suma

Fin
```

---

## 2. Estructura condicional

Permite tomar decisiones según se cumpla o no una condición.

### Ejemplo

```text
Inicio

    Leer edad

    if (edad >= 18) then

        Escribir "Mayor de edad"

    else

        Escribir "Menor de edad"

    endif

Fin
```

---

## 3. Estructura repetitiva

Permite ejecutar instrucciones varias veces.

### Ejemplo con for

```text
Inicio

    for (i = 1; i <= 10; i++)

        Escribir i

    endfor

Fin
```

### Ejemplo con while

```text
Inicio

    contador = 1

    while (contador <= 10)

        Escribir contador

        contador = contador + 1

    endwhile

Fin
```

---

# Ejemplo básico

## Problema

Mostrar un mensaje en pantalla.

### Pseudocódigo

```text
Inicio

    Escribir "Hola Mundo"

Fin
```

---

# Ejemplo con variables

## Problema

Sumar dos números.

### Pseudocódigo

```text
Inicio

    Leer numero1
    Leer numero2

    suma = numero1 + numero2

    Escribir suma

Fin
```

---

# Ventajas

| Ventaja | Descripción |
|----------|------------|
| Claridad | Facilita la comprensión del algoritmo. |
| Simplicidad | No requiere conocer sintaxis específica. |
| Organización | Permite estructurar la solución. |
| Corrección | Facilita detectar errores lógicos. |

---

# Diferencia entre algoritmo y pseudocódigo

| Concepto | Descripción |
|----------|-------------|
| Algoritmo | Secuencia de pasos para resolver un problema. |
| Pseudocódigo | Representación escrita del algoritmo. |

---

# Convenciones utilizadas

Para mantener uniformidad en los algoritmos presentados se utilizarán las siguientes convenciones.

| Acción | Sintaxis |
|---------|----------|
| Inicio del algoritmo | Inicio |
| Fin del algoritmo | Fin |
| Entrada de datos | Leer |
| Salida de datos | Escribir |
| Asignación | = |
| Condicional | if (...) then |
| Alternativa | else |
| Fin de condicional | endif |
| Ciclo while | while (...) |
| Fin de while | endwhile |
| Ciclo for | for (...) |
| Fin de for | endfor |

---

# Aplicaciones

El pseudocódigo se utiliza en:

- Diseño de algoritmos.
- Enseñanza de programación.
- Documentación de soluciones.
- Planificación de programas.
- Comunicación de ideas y procesos.

---

# Errores comunes

| Error | Descripción |
|---------|------------|
| Mezclar pseudocódigo con sintaxis completa de un lenguaje | Reduce la claridad. |
| Omitir pasos importantes | Produce algoritmos incompletos. |
| No definir entradas y salidas | Dificulta la comprensión. |
| Utilizar instrucciones ambiguas | Genera confusión. |
| No respetar la estructura | Reduce la legibilidad. |

---

# Conclusión

El pseudocódigo es una herramienta fundamental para representar algoritmos de manera clara y estructurada. Permite concentrarse en la lógica de la solución antes de realizar cualquier implementación.

---

# Resumen

| Concepto | Idea principal |
|----------|---------------|
| Pseudocódigo | Representación textual de un algoritmo. |
| Objetivo | Describir la lógica de una solución. |
| Ventaja principal | Claridad y facilidad de comprensión. |
| Independencia | No depende de un lenguaje de programación. |
| Aplicación | Diseño y documentación de algoritmos. |
