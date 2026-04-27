# Diagramas de Flujo

---

## ¿Qué es un diagrama de flujo?

Un **diagrama de flujo** es la representación gráfica de un algoritmo o proceso mediante símbolos conectados por flechas.

Permite visualizar de forma clara y ordenada los pasos necesarios para resolver un problema.

Se utiliza en:

- Programación
- Sistemas
- Procesos administrativos
- Matemática
- Ingeniería
- Diseño de soluciones

---

## Importancia

Los diagramas de flujo ayudan a:

- Comprender mejor un problema
- Organizar pasos lógicos
- Detectar errores antes de programar
- Comunicar procesos fácilmente
- Facilitar mantenimiento de sistemas

---

# Elementos básicos

Todo diagrama de flujo está compuesto por:

- Símbolos
- Flechas
- Texto descriptivo
- Secuencia lógica

---

# Símbolos principales

## 1. Inicio / Fin

~~~mermaid
flowchart TD
A@{ shape: stadium, label: "Inicio" }
B@{ shape: stadium, label: "Fin"}
A-->B
~~~

---

## 2. Proceso

~~~mermaid
flowchart TD
A@{ shape: rect, label: "Calcular suma" }
~~~

---

## 3. Entrada / Salida

~~~mermaid
flowchart TD
A@{ shape: lean-r, label: "Leer número" }
B@{ shape: doc, label: "Mostrar resultado" }
A-->B
~~~

---

## 4. Decisión

~~~mermaid
flowchart TD
A@{ shape: diamond, label: "Condición" }
~~~

---

## 5. Lineas de flujo de informacion

~~~mermaid
flowchart LR
A(( )) --> B(( ))
~~~

---

## 6. Seleccion multiple "Switch"

~~~mermaid
flowchart TD
A@{ shape: diamond, label: "switch(opción)" }

A -->|1| B@{ shape: rect, label: "Case 1" }
A -->|2| C@{ shape: rect, label: "Case 2" }
A -->|3| D@{ shape: rect, label: "Case 3" }
A -->|default| E@{ shape: rect, label: "Otro" }
~~~

## 7. Repetitiva While

~~~mermaid
flowchart TD
A@{ shape: diamond, label: "while i < 10" }

A -->|No| B@{ shape: rect, label: "Salir" }
B --> A
A -->|Si| C@{ shape: rect, label: "Proceso" }
~~~

## 8. Repetitiva Do While

~~~mermaid
flowchart TD
A@{ shape: rect, label: "Proceso" }
B@{ shape: diamond, label: "Do While" }

A --> B
~~~

## 9. Repetitiva For

~~~mermaid
flowchart TD
A@{ shape: hex, label: "i=0; i-1; i++" }
~~~

---

# Reglas para elaborar diagramas

- Debe tener Inicio y Fin
- Leer de arriba hacia abajo
- Usar flechas claras
- Evitar cruces innecesarios
- Cada símbolo cumple una función
- Texto corto y entendible

---

# Tipos de estructuras en diagramas

Por ahora trabajaremos solo con diagramas de flujo, enfocados en las 3 estructuras principales:

1. Secuencial
2. Selectivas
3. Repetitivas

---

## 1. Estructura Secuencial

Se ejecutan instrucciones una tras otra, en orden.

### Ejemplo:

Leer dos números, sumarlos y mostrar resultado.

```mermaid
flowchart TD

A([Inicio])
B@{ shape: lean-r, label: "Leer A" }
C@{ shape: lean-r, label: "Leer B" }
D@{ shape: rect, label: "Suma = A + B" }
E@{ shape: doc, label: "Mostrar Suma" }
F([Fin])

A --> B --> C --> D --> E --> F
```

---

## 2. Estructuras Selectivas

Permiten tomar decisiones.

Incluyen:

* If simple
* If else
* Switch

---

### Ejemplo IF

```mermaid
flowchart TD

A([Inicio])
B@{ shape: lean-r, label: "Leer N" }

C@{ shape: diamond, label: "N > 0 ?" }

D@{ shape: doc, label: "Positivo" }
E@{ shape: doc, label: "No positivo" }

F([Fin])

A --> B --> C
C -->|Sí| D --> F
C -->|No| E --> F
```

---

### Ejemplo SWITCH

```mermaid
flowchart TD

A([Inicio])
B@{ shape: lean-r, label: "Leer opción" }

C@{ shape: diamond, label: "Switch(opción)" }

D@{ shape: doc, label: "Sumar" }
E@{ shape: doc, label: "Restar" }
F@{ shape: doc, label: "Otro" }

G([Fin])

A --> B --> C

C -->|1| D --> G
C -->|2| E --> G
C -->|Default| F --> G
```

---

## 3. Estructuras Repetitivas

Repiten instrucciones.

Incluyen:

* While
* Do While
* For

---

### Ejemplo WHILE

```mermaid
flowchart TD

A([Inicio])
B@{ shape: rect, label: "i = 1" }

C@{ shape: diamond, label: "i <= 5 ?" }

D@{ shape: doc, label: "Mostrar i" }
E@{ shape: rect, label: "i = i + 1" }

F([Fin])

A --> B --> C
C -->|Sí| D --> E --> C
C -->|No| F
```

---

### Ejemplo DO WHILE

```mermaid
flowchart TD

A([Inicio])

B@{ shape: rect, label: "i = 1" }

C@{ shape: doc, label: "Mostrar i" }

D@{ shape: rect, label: "i = i + 1" }

E@{ shape: diamond, label: "i <= 5 ?" }

F([Fin])

A --> B --> C --> D --> E
E -->|Sí| C
E -->|No| F
```

---

### Ejemplo FOR

```mermaid
flowchart TD

A([Inicio])

B@{ shape: hex, label: "i = 1; i <= 5; i++" }

C@{ shape: doc, label: "Mostrar i" }

D([Fin])

A --> B
B -->|Sí| C --> B
B -->|No| D
```
---

# Ventajas

- Fácil comprensión visual
- Orden lógico claro
- Detecta errores temprano
- Sirve para documentación
- Útil para aprender programación

---

# Desventajas

- Diagramas grandes pueden complicarse
- Cambios constantes requieren edición
- No reemplaza código real

---

# Errores comunes

- No colocar Inicio / Fin
- Flechas mal orientadas
- Decisiones sin dos salidas
- Exceso de texto
- Saltar pasos importantes

---

# Aplicaciones reales

- Sistemas informáticos
- Bancos
- Procesos industriales
- Apps móviles
- Juegos
- Algoritmos matemáticos

---

# Diferencia con pseudocódigo

| Diagrama de flujo | Pseudocódigo           |
|-------------------|------------------------|
| Visual            | Texto                  |
| Usa símbolos      | Usa instrucciones      |
| Más gráfico       | Más parecido al código |

---

# Recomendaciones

- Diseñar primero en papel
- Mantener simpleza
- Nombrar bien procesos
- Probar lógica paso a paso

---

# Resumen

- Representa algoritmos gráficamente
- Usa símbolos estándar
- Muestra secuencia, decisiones y ciclos
- Ayuda antes de programar
- Fundamental en lógica computacional

---
