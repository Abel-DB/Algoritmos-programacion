# Pruebas de Escritorio

## ¿Qué es una prueba de escritorio?

Una **prueba de escritorio** es una técnica utilizada para verificar el funcionamiento de un algoritmo antes de implementarlo en un lenguaje de programación.

Consiste en simular manualmente la ejecución de cada instrucción utilizando datos de prueba y registrando los resultados obtenidos.

---

# Importancia

Las pruebas de escritorio permiten:

* Detectar errores lógicos.
* Verificar resultados.
* Comprobar el funcionamiento de algoritmos.
* Reducir errores durante la implementación.
* Comprender mejor la lógica de una solución.

---

# Relación con la resolución de problemas

La prueba de escritorio forma parte del proceso de validación de una solución antes de su implementación.

Permite verificar que el análisis del problema, el diseño de la solución, el pseudocódigo y el diagrama de flujo producen los resultados esperados.

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

---

# Objetivo

El objetivo principal es responder la pregunta:

> ¿El algoritmo produce el resultado esperado para determinados datos de entrada?

Si la respuesta es sí, el algoritmo probablemente está correctamente diseñado.

---

# Elementos de una prueba de escritorio

| Elemento         | Descripción                                  |
| ---------------- | -------------------------------------------- |
| Datos de entrada | Valores utilizados para probar el algoritmo. |
| Variables        | Datos que cambian durante la ejecución.      |
| Procesos         | Operaciones realizadas.                      |
| Resultados       | Valores obtenidos al finalizar.              |

---

# Metodología

Una prueba de escritorio suele realizarse siguiendo estos pasos:

1. Analizar el algoritmo.
2. Seleccionar datos de prueba.
3. Simular la ejecución paso a paso.
4. Registrar cambios en las variables.
5. Verificar los resultados obtenidos.

---

# Ejemplo 1: Suma de dos números

## Problema

Leer dos números y mostrar su suma.

### Pseudocódigo

```text
Inicio

    Leer A
    Leer B

    suma ← A + B

    Escribir suma

Fin
```

### Datos de entrada

```text
A = 10
B = 5
```

### Prueba de escritorio

| Paso         | A  | B | suma |
| ------------ | -- | - | ---- |
| Leer A       | 10 | - | -    |
| Leer B       | 10 | 5 | -    |
| suma ← A + B | 10 | 5 | 15   |
| Mostrar suma | 10 | 5 | 15   |

### Resultado

```text
15
```

---

# Ejemplo 2: Cálculo de área

## Problema

Calcular el área de un rectángulo.

### Pseudocódigo

```text
Inicio

    Leer base
    Leer altura

    area ← base * altura

    Escribir area

Fin
```

### Datos de entrada

```text
base = 8
altura = 4
```

### Prueba de escritorio

| Paso                 | base | altura | area |
| -------------------- | ---- | ------ | ---- |
| Leer base            | 8    | -      | -    |
| Leer altura          | 8    | 4      | -    |
| area ← base * altura | 8    | 4      | 32   |
| Mostrar area         | 8    | 4      | 32   |

### Resultado

```text
32
```

---

# Ventajas

| Ventaja             | Descripción                            |
| ------------------- | -------------------------------------- |
| Simplicidad         | No requiere computadora.               |
| Claridad            | Permite seguir la lógica paso a paso.  |
| Corrección temprana | Detecta errores antes de programar.    |
| Comprensión         | Facilita el aprendizaje de algoritmos. |

---

# Limitaciones

| Limitación      | Descripción                               |
| --------------- | ----------------------------------------- |
| Procesos largos | Pueden volverse tediosos.                 |
| Errores humanos | La simulación puede contener fallos.      |
| Escalabilidad   | No es práctica para algoritmos complejos. |

---

# Casos donde se utiliza

Las pruebas de escritorio son especialmente útiles para:

* Algoritmos secuenciales.
* Algoritmos condicionales.
* Algoritmos repetitivos.
* Validación de pseudocódigo.
* Verificación de diagramas de flujo.

---

# Recomendaciones

| Recomendación                | Motivo                                 |
| ---------------------------- | -------------------------------------- |
| Utilizar datos simples       | Facilita la verificación.              |
| Registrar todos los cambios  | Evita omisiones.                       |
| Probar varios casos          | Permite validar diferentes escenarios. |
| Verificar entradas y salidas | Garantiza resultados correctos.        |

---

# Errores comunes

| Error                                 | Descripción                       |
| ------------------------------------- | --------------------------------- |
| Saltar pasos                          | Produce resultados incorrectos.   |
| No registrar cambios de variables     | Dificulta el análisis.            |
| Utilizar pocos casos de prueba        | Reduce la confiabilidad.          |
| Confundir valores iniciales y finales | Genera errores de interpretación. |

---

# Información complementaria

Para comprender el proceso completo de resolución de problemas consulte:

* [Etapas de resolución](../Tema04_resolucion_problemas/1-etapas_resolucion.md)

Para conocer la representación textual de algoritmos consulte:

* [Pseudocódigo](../Tema04_resolucion_problemas/2-pseudocodigo.md)

Para conocer la representación gráfica de algoritmos consulte:

* [Diagramas de flujo](../Tema04_resolucion_problemas/3-diagramas_flujo.md)

---

# Buenas prácticas

Al realizar pruebas de escritorio se recomienda:

* Probar casos simples antes de utilizar casos complejos.
* Utilizar valores que permitan verificar todas las condiciones del algoritmo.
* Registrar todos los cambios de las variables.
* Revisar paso a paso cada instrucción.
* Verificar que las salidas coincidan con los resultados esperados.
* Realizar varias pruebas con diferentes datos de entrada.

---

# Conclusión

Las pruebas de escritorio constituyen una herramienta fundamental para validar algoritmos antes de programarlos. Permiten analizar paso a paso el comportamiento de una solución y detectar errores de lógica de manera temprana.

---

# Resumen

| Concepto             | Idea principal                            |
| -------------------- | ----------------------------------------- |
| Prueba de escritorio | Simulación manual de un algoritmo.        |
| Objetivo             | Verificar resultados y lógica.            |
| Datos de prueba      | Valores utilizados durante la simulación. |
| Ventaja principal    | Detectar errores antes de programar.      |
| Aplicación           | Validación de algoritmos y pseudocódigo.  |
