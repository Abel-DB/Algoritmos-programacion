# Diagramas de Flujo y Resolución de Problemas

---

## Diagrama de flujo

Un **diagrama de flujo** es la representación gráfica de un algoritmo mediante símbolos.

Permite visualizar de forma clara los pasos necesarios para resolver un problema.

---

## Símbolos básicos

### Inicio / Fin

* Representa el comienzo o final del algoritmo
* **Forma:** óvalo

---

### Proceso

* Representa operaciones o cálculos
* **Forma:** rectángulo

---

### Entrada de datos

* Permite ingresar información
* **Forma:** paralelogramo

---

### Salida de datos

Puede representarse de dos formas:

* **Paralelogramo:** mostrar en pantalla
* **Documento:** salida en forma de reporte o impresión

---

### Decisión

* Representa una condición (sí / no)
* **Forma:** rombo

---

### Líneas de flujo

* Indican la dirección del algoritmo

---

## Etapas de resolución de problemas

Antes de programar, se deben seguir estas etapas:

---

### Análisis

Es la etapa más importante, donde se entiende el problema.

Se responde a las siguientes preguntas:

#### ¿Qué? (Objetivo)

* ¿Qué se desea resolver?

#### Datos (Entrada)

* ¿Qué información se necesita?

#### Procesos (¿Cómo?)

* ¿Qué operaciones se realizarán?

#### Resultados (Salida)

* ¿Qué se espera obtener?

---

## Prueba de escritorio

La **prueba de escritorio** es una técnica para verificar el algoritmo paso a paso sin usar la computadora.

Consiste en simular la ejecución con valores de ejemplo.

---

### Ejemplo

**Problema:** Sumar dos números

| Paso    | A | B | Suma |
| ------- | - | - | ---- |
| Entrada | 2 | 3 | -    |
| Proceso | 2 | 3 | 5    |
| Salida  | 2 | 3 | 5    |

---

## Importancia

* Permite detectar errores antes de programar
* Ayuda a entender mejor la lógica
* Evita errores en el código

---

## Relación con C++

Todo este proceso se traduce luego en código:

```cpp id="1h4y7l"
#include <iostream>
using namespace std;

int main() {
    int a, b, suma;

    cout << "Ingrese dos numeros: ";
    cin >> a >> b;

    suma = a + b;

    cout << "Resultado: " << suma;

    return 0;
}
```

---

## Resumen

* El diagrama de flujo representa un algoritmo gráficamente.
* El análisis define el problema (qué, datos, proceso, resultado).
* La prueba de escritorio permite validar la lógica sin programar.

---

