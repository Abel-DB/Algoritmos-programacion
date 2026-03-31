# Macros

---

## ¿Qué es una macro?

Una **macro** es una instrucción que permite **definir un texto o valor que será reemplazado automáticamente** antes de ejecutar el programa.

Es decir:

* No se ejecuta como código
* Se **sustituye antes de la ejecución**

---

## Idea clave

Una macro funciona como un **reemplazo automático de texto**.

---

## Ejemplo conceptual

```id="x2p9lw"
PI → 3.1416
```

Cuando el programa usa **PI**, en realidad se reemplaza por **3.1416**.

---

## ¿Dónde se usan?

En la etapa de:

**Preprocesamiento**

---

## Flujo del programa

```id="q7v2mz"
Código → Preprocesador → Compilación → Ejecución
```

- Las macros actúan **antes de compilar**

---

# Tipos de macros

---

## 1. Macros constantes

Definen valores fijos.

Ejemplo:

```id="k8v1dn"
MAX = 100
PI = 3.14
```

- Evitan repetir valores en el programa

---

## 2. Macros con parámetros

Funcionan como funciones simples.

Ejemplo:

```id="1m7zqs"
SUMA(a, b) → a + b
```

---

## Ejemplo práctico

```id="3c0gpa"
SUMA(2,3) → 2 + 3 → 5
```

---

# Diagrama de funcionamiento

```id="p9r2xk"
   ┌──────────────┐
   │ Código fuente│
   └─────┬────────┘
         │
   ┌──────────────┐
   │ Preprocesador│ ← Aplica macros
   └─────┬────────┘
         │
   ┌──────────────┐
   │ Código final │
   └─────┬────────┘
         │
   ┌──────────────┐
   │ Compilación  │
   └──────────────┘
```

---

# Ventajas

- Reduce repetición de código
- Hace el código más legible
- Facilita cambios globales
- Mejora la organización

---

# Desventajas

- No tienen control de tipos
- Pueden generar errores difíciles
- No respetan prioridad de operaciones
- Difíciles de depurar

---

# Problema clásico

---

## Ejemplo incorrecto

```id="2r5tpa"
CUADRADO(x) → x * x
```

Uso:

```id="6j3f1a"
CUADRADO(2 + 3)
```

Resultado:

```id="9q8t1z"
2 + 3 * 2 + 3 = 11
```

- Error por prioridad de operaciones

---

## Forma correcta

```id="z0h3ks"
CUADRADO(x) → (x * x)
```

---

# Prueba de escritorio

| Expresión   | Reemplazo | Resultado |
| ----------- | --------- | --------- |
| SUMA(2,3)   | 2 + 3     | 5         |
| CUADRADO(4) | 4 * 4     | 16        |

---

# Diferencia con funciones

| Macro              | Función           |
| ------------------ | ----------------- |
| Reemplazo de texto | Código ejecutable |
| No valida tipos    | Sí valida         |
| Más rápida         | Más segura        |
| Más peligrosa      | Más controlada    |

---

# Buenas prácticas

- Usar para constantes
- Usar nombres en MAYÚSCULAS
- Usar paréntesis en operaciones
- Evitar macros complejas

---

# Aplicaciones

* Definir constantes
* Simplificar cálculos
* Configuración de programas
* Optimización

---

# Conceptos clave

---

## 1. Preprocesador

Programa que transforma el código antes de compilar.

---

## 2. Sustitución textual

Reemplazo directo sin interpretación.

---

## 3. Expansión de macros

Proceso de reemplazo automático.

---

# Errores comunes

* No usar paréntesis
* Usar macros como funciones complejas
* Confundir macros con variables
* No entender el preprocesamiento

---

# Conclusión

Las macros son una herramienta poderosa pero peligrosa.

- Se deben usar con cuidado.

---

# Resumen

* Son reemplazos de texto
* Se ejecutan antes del programa
* No son funciones reales
* Útiles para constantes y simplificación

---
