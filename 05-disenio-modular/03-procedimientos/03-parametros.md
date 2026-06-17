# Parámetros de Procedimientos

## ¿Qué son los parámetros?

Los parámetros son datos que se envían a un procedimiento para que pueda realizar una tarea determinada.

Permiten que un mismo procedimiento trabaje con diferentes valores sin necesidad de modificar su código.

Los parámetros se definen en la cabecera del procedimiento y reciben valores cuando el procedimiento es invocado.

---

# Importancia

Los parámetros permiten:

- Reutilizar procedimientos.
- Evitar la repetición de código.
- Trabajar con datos diferentes.
- Hacer los programas más flexibles.
- Favorecer la modularidad.

Sin parámetros sería necesario crear procedimientos distintos para cada situación.

---

# Sintaxis general

```text
Procedimiento nombreProcedimiento(parametro1, parametro2, ...)

    instrucciones

FinProcedimiento
```

---

# ¿Cómo funcionan?

Cuando un procedimiento es llamado:

1. Se envían datos desde la llamada.
2. Los parámetros reciben esos valores.
3. El procedimiento ejecuta sus instrucciones.
4. Finaliza la ejecución.
5. El programa continúa normalmente.

```text
Llamada
    ↓
Parámetros
    ↓
Ejecución
    ↓
Fin del procedimiento
```

---

# Ejemplo básico

## Declaración

```text
Procedimiento saludar(nombre)

    Escribir "Hola ", nombre

FinProcedimiento
```

---

## Llamada

```text
saludar("Juan")
```

---

## Salida

```text
Hola Juan
```

---

# Procedimiento con un parámetro

## Declaración

```text
Procedimiento mostrarEdad(edad)

    Escribir edad

FinProcedimiento
```

---

## Llamada

```text
mostrarEdad(20)
```

---

## Salida

```text
20
```

---

# Procedimiento con varios parámetros

## Declaración

```text
Procedimiento mostrarSuma(a, b)

    suma = a + b

    Escribir suma

FinProcedimiento
```

---

## Llamada

```text
mostrarSuma(6, 8)
```

---

## Salida

```text
14
```

---

# Correspondencia de parámetros

Los valores enviados deben respetar la cantidad y el orden definido en el procedimiento.

## Procedimiento

```text
Procedimiento mostrarDatos(nombre, edad)

    Escribir nombre
    Escribir edad

FinProcedimiento
```

---

## Llamada correcta

```text
mostrarDatos("Ana", 20)
```

### Resultado

```text
Ana
20
```

---

## Llamada incorrecta

```text
mostrarDatos(20, "Ana")
```

Los datos llegarán a parámetros incorrectos.

---

# Parámetros y argumentos

Aunque suelen confundirse, no son exactamente lo mismo.

## Parámetros

Son las variables definidas en el procedimiento.

```text
Procedimiento mostrarDatos(nombre, edad)
```

`nombre` y `edad` son parámetros.

---

## Argumentos

Son los valores enviados durante la llamada.

```text
mostrarDatos("Ana", 20)
```

`"Ana"` y `20` son argumentos.

---

# Flujo de los parámetros

```mermaid
flowchart TD

A[MostrarSuma(6, 8)]

B[a = 6]

C[b = 8]

D[Ejecutar procedimiento]

E[Escribir 14]

A --> B
A --> C
B --> D
C --> D
D --> E
```

---

# Ventajas de utilizar parámetros

- Permiten reutilizar procedimientos.
- Facilitan el mantenimiento.
- Reducen la duplicación de código.
- Mejoran la modularidad.
- Incrementan la flexibilidad de los programas.

---

# Buenas prácticas

- Utilizar nombres descriptivos.
- Mantener únicamente los parámetros necesarios.
- Respetar el orden de los parámetros.
- Evitar parámetros innecesarios.
- Documentar claramente su propósito cuando sea necesario.

---

# Relación con la llamada

Los parámetros forman parte de la comunicación entre el programa y el procedimiento.

```text
Llamada
        ↓
Argumentos
        ↓
Parámetros
        ↓
Ejecución
```

---

# Conclusión

Los parámetros permiten que un procedimiento reciba información para realizar una tarea específica. Gracias a ellos, los procedimientos pueden reutilizarse con diferentes datos, favoreciendo la modularidad, flexibilidad y mantenimiento de los programas.

---

# Resumen

| Concepto | Descripción |
|-----------|------------|
| Parámetro | Variable definida en el procedimiento. |
| Argumento | Valor enviado durante la llamada. |
| Parámetro único | Recibe un solo dato. |
| Múltiples parámetros | Reciben varios datos. |
| Beneficio principal | Reutilización y flexibilidad. |
