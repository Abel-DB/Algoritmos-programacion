# Retorno de Funciones

## ¿Qué es el retorno de una función?

El retorno es el valor que una función devuelve al programa que la invocó una vez que ha finalizado su ejecución.

Gracias al retorno, una función puede entregar el resultado de un procesamiento para que sea utilizado en otras partes del programa.

---

# Importancia

El retorno permite:

- Obtener resultados de una función.
- Reutilizar cálculos.
- Evitar la repetición de código.
- Construir programas más organizados.
- Comunicar resultados entre módulos.

Sin el retorno, una función no podría entregar el resultado de su procesamiento.

---

# Instrucción de retorno

La devolución de un valor se realiza mediante la instrucción:

```text
Retornar
```

### Sintaxis general

```text
Retornar valor
```

Cuando se ejecuta la instrucción `Retornar`, la función finaliza su ejecución y devuelve el valor indicado.

---

# Estructura general

```text
Funcion nombreFuncion(parametros)

    instrucciones

    Retornar resultado

FinFuncion
```

---

# ¿Cómo funciona el retorno?

El proceso sigue la siguiente secuencia:

```text
Datos de entrada
        ↓
Procesamiento
        ↓
Retornar resultado
        ↓
Variable receptora
```

---

# Ejemplo básico

```text
Funcion sumar(a, b)

    resultado = a + b

    Retornar resultado

FinFuncion
```

### Llamada

```text
sumar(6, 8)
```

### Resultado

```text
14
```

---

# Retorno de una variable

La función puede devolver una variable previamente calculada.

### Ejemplo

```text
Funcion cuadrado(numero)

    resultado = numero * numero

    Retornar resultado

FinFuncion
```

### Llamada

```text
cuadrado(5)
```

### Resultado

```text
25
```

---

# Retorno de una expresión

No siempre es necesario utilizar una variable intermedia.

También es posible devolver directamente una expresión.

### Ejemplo

```text
Funcion sumar(a, b)

    Retornar a + b

FinFuncion
```

### Resultado

```text
14
```

---

# Uso del valor retornado

El valor devuelto puede almacenarse en una variable.

### Ejemplo

```text
resultado = sumar(6, 8)
```

Después de la ejecución:

```text
resultado = 14
```

---

# Uso directo del retorno

También es posible utilizar el valor retornado sin almacenarlo previamente.

### Ejemplo

```text
Escribir sumar(6, 8)
```

### Resultado

```text
14
```

---

# Función sin parámetros con retorno

Una función puede devolver un valor sin recibir parámetros.

### Ejemplo

```text
Funcion obtenerPI()

    Retornar 3.1416

FinFuncion
```

### Resultado

```text
3.1416
```

---

# Representación gráfica

```mermaid
flowchart LR

A[Parámetros]

B[Procesamiento]

C[Retorno]

D[Variable receptora]

A --> B
B --> C
C --> D
```

---

# Consideraciones importantes

- Una función devuelve un único valor.
- La instrucción `Retornar` finaliza la ejecución de la función.
- El valor retornado puede almacenarse o utilizarse directamente.
- Una función puede retornar una variable o una expresión.
- No es obligatorio recibir parámetros para retornar un valor.

---

# Diferencia con un procedimiento

La principal diferencia entre una función y un procedimiento es el retorno.

### Función

```text
promedio = calcularPromedio()
```

Devuelve un valor.

---

### Procedimiento

```text
mostrarPromedio()
```

Realiza una acción, pero no devuelve un resultado.

---

# Ventajas del retorno

- Permite reutilizar resultados.
- Facilita la modularización.
- Mejora la organización del programa.
- Reduce la duplicación de código.
- Favorece la comunicación entre módulos.

---

# Buenas prácticas

- Retornar únicamente la información necesaria.
- Utilizar nombres descriptivos para las variables retornadas.
- Evitar cálculos excesivamente complejos en una sola instrucción de retorno.
- Verificar que siempre exista un valor válido para retornar.

---

# Relación con otros conceptos

El retorno forma parte de la estructura de una función.

```text
Función
│
├── Nombre
├── Parámetros
├── Instrucciones
└── Retorno
```

---

# Conclusión

El retorno es el mecanismo mediante el cual una función devuelve un resultado al programa que la invocó. Gracias a él, las funciones pueden entregar información procesada para ser reutilizada en otras partes del programa, favoreciendo la organización y reutilización del código.

---

# Resumen

| Concepto | Descripción |
|-----------|------------|
| Retorno | Valor devuelto por una función. |
| Retornar | Instrucción utilizada para devolver resultados. |
| Variable receptora | Almacena el valor retornado. |
| Retorno directo | Devuelve una expresión sin variable intermedia. |
| Beneficio principal | Comunicación de resultados entre módulos. |
