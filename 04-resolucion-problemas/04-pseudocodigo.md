# Pseudocódigo

## ¿Qué es el pseudocódigo?

El **pseudocódigo** es una forma de representar algoritmos mediante instrucciones escritas en lenguaje natural estructurado.

Su objetivo es describir la lógica de una solución sin depender de la sintaxis de un lenguaje de programación específico.

---

# Importancia

El pseudocódigo permite:

* Diseñar algoritmos antes de programar.
* Comprender mejor la lógica de una solución.
* Detectar errores tempranamente.
* Facilitar la comunicación entre personas.
* Servir como puente entre el algoritmo y el código.

---

# Características

| Característica             | Descripción                                     |
| -------------------------- | ----------------------------------------------- |
| Independiente del lenguaje | No pertenece a ningún lenguaje de programación. |
| Fácil de leer              | Utiliza lenguaje cercano al humano.             |
| Estructurado               | Sigue una secuencia lógica.                     |
| Flexible                   | Puede adaptarse a distintos problemas.          |

---

# Elementos básicos

| Elemento | Función                         |
| -------- | ------------------------------- |
| Leer     | Obtener datos de entrada.       |
| Escribir | Mostrar resultados.             |
| Asignar  | Almacenar valores en variables. |
| Operar   | Realizar cálculos o procesos.   |
| Decidir  | Evaluar condiciones.            |
| Repetir  | Ejecutar acciones varias veces. |

---

# Relación con la resolución de problemas

El pseudocódigo forma parte del proceso completo de resolución de problemas.

Antes de escribir un pseudocódigo es necesario comprender el problema y diseñar una solución.

## Flujo de trabajo

```text
Problema
    ↓
Análisis del problema
    ↓
Diseño de la solución
    ↓
Pseudocódigo
    ↓
Diagrama de flujo
    ↓
Prueba de escritorio
    ↓
Implementación
    ↓
Pruebas y corrección
```

El pseudocódigo no es la primera etapa de resolución. Antes de escribirlo se debe realizar el análisis del problema y el diseño de la solución.

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

    Suma ← A + B

    Escribir Suma

Fin
```

---

## 2. Estructura condicional

Permite tomar decisiones según se cumpla o no una condición.

### Ejemplo

```text
Inicio

    Leer edad

    Si edad >= 18 Entonces

        Escribir "Mayor de edad"

    Sino

        Escribir "Menor de edad"

    FinSi

Fin
```

---

## 3. Estructura repetitiva

Permite ejecutar instrucciones varias veces.

### Ejemplo

```text
Inicio

    Para i ← 1 Hasta 10

        Escribir i

    FinPara

Fin
```

---

# Ejemplo básico

### Problema

Mostrar un mensaje en pantalla.

### Pseudocódigo

```text
Inicio

    Escribir "Hola Mundo"

Fin
```

---

# Ejemplo con variables

### Problema

Sumar dos números.

### Pseudocódigo

```text
Inicio

    Leer numero1
    Leer numero2

    suma ← numero1 + numero2

    Escribir suma

Fin
```

---

# Entrada, proceso y salida

Todo pseudocódigo puede analizarse mediante el modelo:

```text
Entrada → Proceso → Salida
```

### Ejemplo

| Etapa   | Información              |
| ------- | ------------------------ |
| Entrada | numero1, numero2         |
| Proceso | suma ← numero1 + numero2 |
| Salida  | suma                     |

---

# Ventajas

| Ventaja      | Descripción                              |
| ------------ | ---------------------------------------- |
| Claridad     | Facilita la comprensión del algoritmo.   |
| Simplicidad  | No requiere conocer sintaxis específica. |
| Organización | Permite estructurar la solución.         |
| Corrección   | Facilita detectar errores lógicos.       |

---

# Diferencia entre algoritmo y pseudocódigo

| Concepto     | Descripción                                   |
| ------------ | --------------------------------------------- |
| Algoritmo    | Secuencia de pasos para resolver un problema. |
| Pseudocódigo | Representación escrita del algoritmo.         |

---

# Relación con C++

### Pseudocódigo

```text
Inicio

    Leer edad
    Escribir edad

Fin
```

### C++

```cpp
int edad;

cin >> edad;
cout << edad;
```

El pseudocódigo permite diseñar la solución antes de implementarla.

---

# Aplicaciones

El pseudocódigo se utiliza en:

* Diseño de algoritmos.
* Enseñanza de programación.
* Documentación de soluciones.
* Planificación de programas.

---

# Errores comunes

| Error                                            | Descripción                     |
| ------------------------------------------------ | ------------------------------- |
| Mezclar pseudocódigo con sintaxis de un lenguaje | Reduce la claridad.             |
| Omitir pasos importantes                         | Produce algoritmos incompletos. |
| No definir entradas y salidas                    | Dificulta la comprensión.       |
| Utilizar instrucciones ambiguas                  | Genera confusión.               |

---

# Información complementaria

Para comprender cómo se integra el pseudocódigo dentro de la resolución de problemas, consulte:

* [Etapas de resolución](../Tema04_resolucion_problemas/1-etapas_resolucion.md)

Para conocer una representación gráfica de los algoritmos, consulte:

* [Diagramas de flujo](../Tema04_resolucion_problemas/3-diagramas_flujo.md)

---

# Convenciones utilizadas

Para mantener uniformidad en todos los algoritmos se utilizarán las siguientes convenciones.

| Acción               | Sintaxis                 |
| -------------------- | ------------------------ |
| Inicio del algoritmo | Inicio                   |
| Fin del algoritmo    | Fin                      |
| Entrada de datos     | Leer                     |
| Salida de datos      | Escribir                 |
| Asignación           | ←                        |
| Condicional          | Si ... Entonces          |
| Alternativa          | Sino                     |
| Fin de condicional   | FinSi                    |
| Ciclo Para           | Para ... FinPara         |
| Ciclo Mientras       | Mientras ... FinMientras |

Estas convenciones serán utilizadas en todos los ejercicios desarrollados durante el curso.

---

# Conclusión

El pseudocódigo es una herramienta fundamental para representar algoritmos de manera clara y estructurada. Permite concentrarse en la lógica de la solución antes de escribir código en un lenguaje de programación.

---

# Resumen

| Concepto                  | Idea principal                          |
| ------------------------- | --------------------------------------- |
| Pseudocódigo              | Representación textual de un algoritmo. |
| Objetivo                  | Diseñar soluciones antes de programar.  |
| Ventaja principal         | Claridad y facilidad de comprensión.    |
| Relación con el algoritmo | Expresa la lógica de solución.          |
| Aplicación                | Diseño y documentación de programas.    |
