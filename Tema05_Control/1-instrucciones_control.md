# Instrucciones de Control

---

## ¿Qué son las instrucciones de control?

Las **instrucciones de control** permiten dirigir el flujo de un algoritmo, indicando:

* El orden en que se ejecutan las instrucciones
* Las decisiones que se deben tomar
* Las repeticiones de procesos

Son fundamentales para construir la lógica de cualquier programa.

---

## Tipos de instrucciones de control

1. Secuenciales
2. Selectivas (condicionales)
3. Repetitivas (ciclos)

---

# 1. Estructura Secuencial

Las instrucciones se ejecutan una tras otra, sin interrupciones.

---

## Diagrama de flujo

```
   ┌───────────┐
   │  INICIO   │      ← Inicio/Fin (óvalo)
   └─────┬─────┘
         │
   ┌───────────────┐
   │ Leer A, B     │  ← Entrada (paralelogramo)
   └─────┬─────────┘
         │
   ┌───────────────┐
   │ Suma = A + B  │  ← Proceso (rectángulo)
   └─────┬─────────┘
         │
   ┌──────────────────┐
   │ Mostrar resultado│  ← Salida (documento)
   └─────┬────────────┘
         │
   ┌───────────┐
   │   FIN     │
   └───────────┘
```

---

## Prueba de escritorio

| Paso    | A   | B  | Suma |
| ------- | --- | -- | ---- |
| Leer A  | 123 | -  | -    |
| Leer B  | 123 | 77 | -    |
| Proceso | 123 | 77 | 200  |
| Mostrar | 123 | 77 | 200  |

---

# 2. Estructura Selectiva (Condicional)

Permite tomar decisiones según una condición.

---

## Diagrama de flujo

```
        ┌───────────┐
        │  INICIO   │
        └─────┬─────┘
              │
        ┌──────────────┐
        │ Leer número  │  ← Entrada
        └─────┬────────┘
              │
        ┌──────────────┐
        │ ¿Número > 0? │  ← Decisión (rombo)
        └───┬─────┬────┘
            │     │
           Sí     No
            │     │
   ┌────────────┐ ┌────────────┐
   │ "Positivo" │ │ "Negativo" │ ← Salida (documento)
   └─────┬──────┘ └─────┬──────┘
         │              │
         └──────┬───────┘
                │
        ┌───────────┐
        │   FIN     │
        └───────────┘
```

---

## Prueba de escritorio

| Paso     | Número | Resultado |
| -------- | ------ | --------- |
| Leer     | 5      | -         |
| Decisión | 5      | Positivo  |
| Mostrar  | 5      | Positivo  |

---

# 3. Estructura Repetitiva (Ciclo)

Permite repetir instrucciones varias veces.

---

## Diagrama de flujo

```
        ┌───────────┐
        │  INICIO   │
        └─────┬─────┘
              │
        ┌───────────┐
        │ i = 1     │  ← Proceso
        └─────┬─────┘
              │
        ┌────────────┐
        │ ¿i ≤ 3?    │  ← Decisión
        └───┬────┬───┘
            │    │
           Sí    No
            │    │
   ┌────────────┐ │
   │ Mostrar i  │ │ ← Salida (documento)
   └─────┬──────┘ │
         │        │
   ┌────────────┐ │
   │ i = i + 1  │ │ ← Proceso
   └─────┬──────┘ │
         │        │
         └────────┘ ← Regresa a la condición
              │
        ┌───────────┐
        │   FIN     │
        └───────────┘
```

---

## Prueba de escritorio

| Paso        | i | Salida |
| ----------- | - | ------ |
| Inicializar | 1 | -      |
| Mostrar     | 1 | 1      |
| Incremento  | 2 | -      |
| Mostrar     | 2 | 2      |
| Incremento  | 3 | -      |
| Mostrar     | 3 | 3      |

---

## Símbolos utilizados

* Inicio / Fin → óvalo
* Proceso → rectángulo
* Entrada → paralelogramo
* Salida → documento
* Decisión → rombo

---

## Importancia

Las instrucciones de control permiten:

* Resolver problemas complejos
* Tomar decisiones dentro de un algoritmo
* Automatizar procesos repetitivos

---

## Resumen

* Secuencial → ejecución en orden
* Selectiva → toma de decisiones
* Repetitiva → repetición de procesos

Son la base de la lógica en programación.

---
