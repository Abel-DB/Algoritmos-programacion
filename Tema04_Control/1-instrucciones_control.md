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
A([Inicio])
B([Fin])
A --> B
~~~

---

## 2. Proceso

~~~mermaid
flowchart TD
A[Calcular suma]
~~~

---

## 3. Entrada / Salida

~~~mermaid
flowchart TD
A[/Leer número/]
B[/Mostrar resultado/]
A --> B
~~~

---

## 4. Decisión

~~~mermaid
flowchart TD
A{¿Edad >= 18?}
A -->|Sí| B[Mayor]
A -->|No| C[Menor]
~~~

---

## 5. Preparación / Inicialización

~~~mermaid
flowchart TD
A{{i = 0}}
~~~

---

## 6. Conector

~~~mermaid
flowchart TD
A((A))
~~~

---

## 7. Almacenamiento

~~~mermaid
flowchart TD
A[(Datos)]
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

## 1. Secuencial

~~~mermaid
flowchart TD
A([Inicio])
B[/Leer A, B/]
C[Sumar A+B]
D[/Mostrar resultado/]
E([Fin])

A --> B --> C --> D --> E
~~~

---

## 2. Selectiva (If)

~~~mermaid
flowchart TD
A([Inicio])
B[/Leer número/]
C{¿Número > 0?}
D[/Positivo/]
E[/Negativo o Cero/]
F([Fin])

A --> B --> C
C -->|Sí| D
C -->|No| E
D --> F
E --> F
~~~

---

## 3. Repetitiva (While)

~~~mermaid
flowchart TD
A([Inicio])
B{{i = 1}}
C{¿i <= 3?}
D[/Mostrar i/]
E[i = i + 1]
F([Fin])

A --> B --> C
C -->|Sí| D
D --> E
E --> C
C -->|No| F
~~~

---

## 4. Ciclo For

~~~mermaid
flowchart TD
A([Inicio])
B{{i = 1}}
C{¿i <= 5?}
D[/Mostrar i/]
E[i++]
F([Fin])

A --> B --> C
C -->|Sí| D
D --> E
E --> C
C -->|No| F
~~~

---

## 5. Switch

~~~mermaid
flowchart TD
A([Inicio])
B[/Leer opción/]
C{Opción}
D[Caso 1]
E[Caso 2]
F[Otro caso]
G([Fin])

A --> B --> C
C -->|1| D
C -->|2| E
C -->|Otro| F
D --> G
E --> G
F --> G
~~~

---

# Ejemplo completo

## Problema: Sumar dos números

~~~mermaid
flowchart TD
A([Inicio])
B[/Leer A, B/]
C[Resultado = A + B]
D[/Mostrar resultado/]
E([Fin])

A --> B --> C --> D --> E
~~~

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

| Diagrama de flujo | Pseudocódigo |
|------------------|-------------|
| Visual | Texto |
| Usa símbolos | Usa instrucciones |
| Más gráfico | Más parecido al código |

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
