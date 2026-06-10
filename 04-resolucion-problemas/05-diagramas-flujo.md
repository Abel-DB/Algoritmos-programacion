# Diagramas de Flujo

## ¿Qué es un diagrama de flujo?

Un **diagrama de flujo** es una representación gráfica de un algoritmo o proceso mediante símbolos conectados por flechas que indican la secuencia de ejecución.

Permite visualizar de forma clara y ordenada los pasos necesarios para resolver un problema.

---

# Importancia

Los diagramas de flujo permiten:

* Comprender mejor un algoritmo.
* Detectar errores lógicos antes de programar.
* Facilitar la comunicación entre personas.
* Documentar procesos y soluciones.
* Servir como guía durante la implementación.

---

# Relación con la resolución de problemas

Los diagramas de flujo forman parte del proceso completo de resolución de problemas.

Su objetivo es representar gráficamente la lógica previamente definida durante el análisis y el diseño de la solución.

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

Antes de elaborar un diagrama de flujo se recomienda:

1. Analizar el problema.
2. Diseñar la solución.
3. Elaborar el pseudocódigo.
4. Construir el diagrama de flujo.

---

# Elementos básicos

Todo diagrama de flujo está compuesto por:

* Símbolos.
* Flechas.
* Texto descriptivo.
* Secuencia lógica.

---

# Estructuras representadas en diagramas de flujo

Los diagramas de flujo permiten representar las tres estructuras fundamentales de los algoritmos.

| Estructura | Descripción |
| ---------- | ----------- |
| Secuencial | Las instrucciones se ejecutan una después de otra. |
| Condicional | Permite tomar decisiones según una condición. |
| Repetitiva | Permite ejecutar acciones varias veces. |

Estas estructuras constituyen la base de la mayoría de los algoritmos.

---

# Símbolos principales

## 1. Inicio / Fin

Representa el comienzo o final del algoritmo.

```mermaid
flowchart TD
A([Inicio])
B([Fin])

A --> B
```

### Uso

* Comenzar un algoritmo.
* Finalizar un algoritmo.

---

## 2. Proceso

Representa una operación o instrucción.

```mermaid
flowchart TD
A[Calcular suma]
```

### Uso

* Realizar cálculos.
* Asignar valores.
* Ejecutar operaciones.

---

## 3. Entrada / Salida

Representa la lectura o escritura de datos.

```mermaid
flowchart TD
A[/Leer número/]
B[/Mostrar resultado/]

A --> B
```

### Uso

* Leer datos.
* Mostrar resultados.

---

## 4. Decisión

Representa una condición que puede generar distintos caminos.

```mermaid
flowchart TD

A{Edad >= 18?}

A -->|Sí| B[Aprobado]
A -->|No| C[Rechazado]
```

### Uso

* IF
* IF ELSE
* Validaciones
* Comparaciones

---

## 5. Línea de flujo

Indica la dirección de ejecución.

```mermaid
flowchart LR

A[Proceso 1] --> B[Proceso 2]
```

### Uso

* Conectar símbolos.
* Indicar secuencia lógica.

---

## 6. Selección múltiple (Switch)

Representa una selección entre varias alternativas.

```mermaid
flowchart TD
    A([Inicio])
    B[/Ingresar opción/]
    C{Opción}

    A --> B
    B --> C

    C -->|1| D[Acción 1]
    C -->|2| E[Acción 2]
    C -->|3| F[Acción 3]
    C -->|Otro| G[Acción por defecto]

    D --> H([Fin])
    E --> H
    F --> H
    G --> H
```

### Uso

* Menús.
* Opciones múltiples.
* Selección de acciones.

---

## 7. Repetitiva While

Representa una repetición controlada por condición.

```mermaid
flowchart TD

A{i < 10 ?}

A -->|Sí| B[Proceso]
B --> A

A -->|No| C[Fin]
```

### Uso

* Repetir mientras una condición sea verdadera.

---

## 8. Repetitiva Do While

Representa una repetición donde el proceso se ejecuta al menos una vez.

```mermaid
flowchart TD

A[Proceso]
B{Condición}

A --> B

B -->|Sí| A
B -->|No| C[Fin]
```

### Uso

* Menús.
* Validación de datos.
* Procesos que deben ejecutarse una primera vez.

---

## 9. Repetitiva For

Representa una repetición controlada por contador.

```mermaid
flowchart TD

A{{i = 0; i < 5; i++}}

A -->|Sí| B[Proceso]
B --> A

A -->|No| C[Fin]
```

### Uso

* Repeticiones conocidas.
* Recorridos de tablas.
* Contadores.

---

# Ejemplo básico

## Problema

Leer dos números y mostrar su suma.

```mermaid
flowchart TD

A([Inicio])

B[/Leer A/]
C[/Leer B/]

D[Suma = A + B]

E[/Mostrar suma/]

F([Fin])

A --> B --> C --> D --> E --> F
```

---

# Reglas para elaborar diagramas

| Regla                         | Descripción                                   |
| ----------------------------- | --------------------------------------------- |
| Tener un único inicio         | El algoritmo debe comenzar en un solo punto.  |
| Tener un único fin            | El algoritmo debe finalizar correctamente.    |
| Utilizar símbolos adecuados   | Cada acción debe representarse correctamente. |
| Mantener una secuencia lógica | El flujo debe ser claro y ordenado.           |
| Evitar cruces innecesarios    | Mejora la legibilidad.                        |
| Utilizar texto breve          | Facilita la comprensión del diagrama.         |

---

# Ventajas

| Ventaja              | Descripción                                |
| -------------------- | ------------------------------------------ |
| Claridad             | Facilita la comprensión del algoritmo.     |
| Organización         | Permite visualizar el proceso completo.    |
| Comunicación         | Facilita el trabajo en equipo.             |
| Detección de errores | Ayuda a identificar fallos lógicos.        |
| Documentación        | Sirve como apoyo para futuros desarrollos. |

---

# Desventajas

| Desventaja    | Descripción                                                |
| ------------- | ---------------------------------------------------------- |
| Espacio       | Los diagramas complejos ocupan más espacio.                |
| Mantenimiento | Deben actualizarse cuando cambia el algoritmo.             |
| Complejidad   | Diagramas muy grandes pueden ser difíciles de interpretar. |

---

# Aplicaciones

Los diagramas de flujo se utilizan en:

* Diseño de algoritmos.
* Desarrollo de software.
* Automatización de procesos.
* Documentación técnica.
* Modelado de sistemas.
* Resolución de problemas.

---

# Errores comunes

| Error                             | Descripción                       |
| --------------------------------- | --------------------------------- |
| Utilizar símbolos incorrectos     | Dificulta la interpretación.      |
| Omitir flechas                    | Genera ambigüedad.                |
| Múltiples inicios o finales       | Reduce la claridad del algoritmo. |
| Diagramas excesivamente complejos | Dificultan la comprensión.        |
| Saltar pasos importantes          | Produce errores lógicos.          |

---

# Información complementaria

Para comprender cómo se construyen los algoritmos representados en diagramas de flujo, consulte:

* [Algoritmos](../Tema01_fundamentos/1-algoritmos.md)

Para conocer la representación textual de los algoritmos, consulte:

* [Pseudocódigo](../Tema04_resolucion_problemas/2-pseudocodigo.md)

Para entender dónde se utilizan dentro del proceso de resolución de problemas, consulte:

* [Etapas de resolución](../Tema04_resolucion_problemas/1-etapas_resolucion.md)

---

# Buenas prácticas

Al elaborar diagramas de flujo se recomienda:

* Mantener un flujo de arriba hacia abajo.
* Utilizar nombres claros y descriptivos.
* Evitar cruces innecesarios entre líneas.
* Utilizar un único inicio y un único fin.
* Mantener una distribución ordenada de los símbolos.
* Verificar que todas las decisiones tengan salidas claramente identificadas.
* Utilizar símbolos estandarizados.
* Mantener la simplicidad y claridad del diagrama.

---

# Conclusión

Los diagramas de flujo constituyen una herramienta gráfica fundamental para representar algoritmos y procesos. Su utilización facilita la comprensión, análisis y diseño de soluciones antes de implementar el código.

Además, permiten representar estructuras secuenciales, selectivas y repetitivas mediante símbolos estandarizados que facilitan la comunicación y documentación de algoritmos.

---

# Resumen

| Concepto          | Idea principal                                  |
| ----------------- | ----------------------------------------------- |
| Diagrama de flujo | Representación gráfica de un algoritmo.         |
| Símbolos          | Elementos utilizados para representar acciones. |
| Flujo             | Secuencia de ejecución del algoritmo.           |
| Decisión          | Permite evaluar condiciones.                    |
| Repetición        | Permite representar ciclos.                     |
| Aplicación        | Diseño y documentación de soluciones.           |
