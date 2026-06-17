# Pruebas de Escritorio

## ¿Qué es una prueba de escritorio?

Una **prueba de escritorio** es una técnica utilizada para verificar el funcionamiento de un algoritmo antes de implementarlo en un lenguaje de programación.

Consiste en simular manualmente la ejecución de cada instrucción utilizando datos de prueba y registrando los resultados obtenidos.

Su objetivo es comprobar que la lógica planteada produce los resultados esperados.

---

# Importancia

Las pruebas de escritorio permiten:

- Detectar errores lógicos.
- Verificar resultados.
- Comprobar el funcionamiento de algoritmos.
- Reducir errores durante la implementación.
- Comprender mejor la lógica de una solución.

---

# Objetivo

El objetivo principal de una prueba de escritorio es responder la siguiente pregunta:

> ¿El algoritmo produce el resultado esperado para determinados datos de entrada?

Si los resultados obtenidos coinciden con los resultados esperados, existe una alta probabilidad de que el algoritmo esté correctamente diseñado.

---

# ¿Cuándo realizar una prueba de escritorio?

La prueba de escritorio se realiza después de construir el pseudocódigo o el diagrama de flujo y antes de implementar la solución en un lenguaje de programación.

Su propósito es verificar que la lógica del algoritmo funcione correctamente antes de comenzar a programar.

---

# Elementos de una prueba de escritorio

| Elemento | Descripción |
|-----------|------------|
| Datos de entrada | Valores utilizados para probar el algoritmo. |
| Variables | Datos que cambian durante la ejecución. |
| Procesos | Operaciones realizadas. |
| Resultados | Valores obtenidos al finalizar la ejecución. |

---

# Metodología

Para realizar una prueba de escritorio se recomienda seguir los siguientes pasos:

1. Revisar el problema.
2. Analizar las entradas y salidas.
3. Seleccionar casos de prueba.
4. Ejecutar el algoritmo paso a paso.
5. Registrar los cambios de las variables.
6. Comparar el resultado obtenido con el esperado.

---

# ¿Cómo construir una tabla de prueba de escritorio?

La tabla debe incluir todas las variables cuyo valor pueda cambiar durante la ejecución del algoritmo.

Para identificar las variables que deben aparecer en la tabla se recomienda:

1. Revisar el pseudocódigo.
2. Identificar todas las variables utilizadas.
3. Agregar una columna para cada variable.
4. Registrar los cambios cada vez que una variable modifica su valor.

---

## Ejemplo

### Pseudocódigo

```text
Inicio

    Leer A
    Leer B

    suma = A + B

    Escribir suma

Fin
```

### Variables identificadas

```text
A
B
suma
```

### Tabla de prueba de escritorio

| Paso | A | B | suma |
|--------|---|---|------|
| Leer A | 10 | - | - |
| Leer B | 10 | 5 | - |
| suma = A + B | 10 | 5 | 15 |
| Escribir suma | 10 | 5 | 15 |

---

## Variables que sí deben incluirse

Normalmente deben aparecer:

- Variables de entrada.
- Variables de salida.
- Contadores.
- Acumuladores.
- Variables auxiliares.

### Ejemplo

```text
base
altura
area

contador
suma
promedio
i
j
```

---

## Variables que no es necesario incluir

No es necesario agregar constantes o valores fijos.

### Ejemplo

```text
1
5
10
100
3.14
```

Estos valores forman parte de las operaciones, pero no cambian durante la ejecución.

---

# ¿Qué hacer cuando una variable cambia varias veces?

Cada vez que una variable modifica su valor, dicho cambio debe registrarse en la tabla.

Por ejemplo:

```text
suma = suma + i
```

La variable `suma` cambiará en cada iteración y debe actualizarse en cada fila de la tabla.

Esta práctica permite observar cómo evoluciona el algoritmo paso a paso.

---

# Ejemplo 1: Estructura secuencial

## Problema

Leer dos números y mostrar su suma.

### Pseudocódigo

```text
Inicio

    Leer A
    Leer B

    suma = A + B

    Escribir suma

Fin
```

### Datos de entrada

```text
A = 10
B = 5
```

### Prueba de escritorio

| Paso | A | B | suma |
|--------|---|---|------|
| Leer A | 10 | - | - |
| Leer B | 10 | 5 | - |
| suma = A + B | 10 | 5 | 15 |
| Escribir suma | 10 | 5 | 15 |

### Resultado

```text
15
```

### Análisis

La variable `suma` almacena el resultado de la operación `A + B`.

Al finalizar la ejecución, el algoritmo muestra correctamente el valor `15`.

---

# Ejemplo 2: Estructura condicional

## Problema

Determinar si una persona es mayor de edad.

### Pseudocódigo

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

### Datos de entrada

```text
edad = 20
```

### Prueba de escritorio

| Paso | edad | Salida |
|--------|------|---------|
| Leer edad | 20 | - |
| Evaluar condición | 20 | Verdadero |
| Escribir resultado | 20 | Mayor de edad |

### Resultado

```text
Mayor de edad
```

### Análisis

La condición `edad >= 18` resulta verdadera.

Por esta razón se ejecuta el bloque correspondiente al `if` y se muestra el mensaje **Mayor de edad**.

---

# Ejemplo 3: Estructura repetitiva

## Problema

Calcular la suma de los números del 1 al 5.

### Pseudocódigo

```text
Inicio

    suma = 0

    for (i = 1; i <= 5; i++)

        suma = suma + i

    endfor

    Escribir suma

Fin
```

### Variables identificadas

```text
i
suma
```

### Datos iniciales

```text
suma = 0
```

### Prueba de escritorio

| Iteración | i | suma |
|------------|---|------|
| Inicial | - | 0 |
| 1 | 1 | 1 |
| 2 | 2 | 3 |
| 3 | 3 | 6 |
| 4 | 4 | 10 |
| 5 | 5 | 15 |

### Resultado

```text
15
```

### Análisis detallado

Inicialmente:

```text
suma = 0
```

Primera iteración:

```text
suma = 0 + 1 = 1
```

Segunda iteración:

```text
suma = 1 + 2 = 3
```

Tercera iteración:

```text
suma = 3 + 3 = 6
```

Cuarta iteración:

```text
suma = 6 + 4 = 10
```

Quinta iteración:

```text
suma = 10 + 5 = 15
```

Al finalizar el ciclo, la variable `suma` contiene el resultado de:

```text
1 + 2 + 3 + 4 + 5
```

Por lo tanto:

```text
suma = 15
```

Este tipo de prueba de escritorio es especialmente útil para comprender cómo cambian las variables dentro de ciclos y acumuladores.

---

# Ventajas

| Ventaja | Descripción |
|----------|------------|
| Simplicidad | No requiere computadora. |
| Claridad | Permite seguir la lógica paso a paso. |
| Corrección temprana | Detecta errores antes de programar. |
| Comprensión | Facilita el aprendizaje de algoritmos. |

---

# Limitaciones

| Limitación | Descripción |
|------------|------------|
| Procesos largos | Pueden volverse tediosos. |
| Errores humanos | La simulación puede contener fallos. |
| Escalabilidad | No es práctica para algoritmos complejos. |

---

# Casos donde se utiliza

Las pruebas de escritorio son especialmente útiles para:

- Algoritmos secuenciales.
- Algoritmos condicionales.
- Algoritmos repetitivos.
- Validación de pseudocódigo.
- Verificación de diagramas de flujo.

---

# Recomendaciones

| Recomendación | Motivo |
|---------------|--------|
| Utilizar datos simples | Facilita la verificación. |
| Registrar todos los cambios | Evita omisiones. |
| Probar varios casos | Permite validar diferentes escenarios. |
| Verificar entradas y salidas | Garantiza resultados correctos. |

---

# Errores comunes

| Error | Descripción |
|---------|------------|
| Saltar pasos | Produce resultados incorrectos. |
| No registrar cambios de variables | Dificulta el análisis. |
| Utilizar pocos casos de prueba | Reduce la confiabilidad. |
| Confundir valores iniciales y finales | Genera errores de interpretación. |

---

# Buenas prácticas

Al realizar pruebas de escritorio se recomienda:

- Probar casos simples antes de utilizar casos complejos.
- Utilizar valores que permitan verificar todas las condiciones del algoritmo.
- Registrar todos los cambios de las variables.
- Revisar paso a paso cada instrucción.
- Verificar que las salidas coincidan con los resultados esperados.
- Realizar varias pruebas con diferentes datos de entrada.

---

# Conclusión

Las pruebas de escritorio constituyen una herramienta fundamental para validar algoritmos antes de programarlos.

Mediante la simulación manual de la ejecución de un algoritmo es posible verificar resultados, detectar errores lógicos y comprender cómo evolucionan las variables durante el proceso de resolución.

---

# Resumen

| Concepto | Idea principal |
|-----------|---------------|
| Prueba de escritorio | Simulación manual de un algoritmo. |
| Objetivo | Verificar resultados y lógica. |
| Datos de prueba | Valores utilizados durante la simulación. |
| Tabla de seguimiento | Permite observar cambios en las variables. |
| Ventaja principal | Detectar errores antes de programar. |
| Aplicación | Validación de algoritmos y pseudocódigo. |
