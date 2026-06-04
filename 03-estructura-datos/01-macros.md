# Macros

## ¿Qué es una macro?

Una **macro** es una instrucción del preprocesador que permite definir sustituciones de texto antes de que el programa sea compilado.

Las macros se crean mediante la directiva `#define`.

---

# Importancia

Las macros permiten:

* Reemplazar valores constantes por nombres descriptivos.
* Facilitar el mantenimiento del código.
* Evitar la repetición de información.
* Mejorar la legibilidad de los programas.

---

# El preprocesador

Antes de la compilación, el código pasa por una etapa llamada **preprocesamiento**.

Durante esta etapa se procesan directivas como:

```cpp
#define
#include
```

Estas instrucciones son interpretadas antes de que el compilador analice el programa.

---

# Sintaxis básica

```cpp
#define NOMBRE valor
```

### Ejemplo

```cpp
#define PI 3.141592
```

Cuando el compilador procesa el programa, reemplaza automáticamente:

```cpp
PI
```

por:

```cpp
3.141592
```

---

# Ejemplo en C++

```cpp
#include <iostream>

#define PI 3.141592

using namespace std;

int main() {
    cout << PI << endl;
    return 0;
}
```

---

# Ventajas

| Ventaja       | Descripción                                                |
| ------------- | ---------------------------------------------------------- |
| Legibilidad   | Los nombres son más fáciles de comprender que los números. |
| Mantenimiento | Un cambio se realiza en un solo lugar.                     |
| Reutilización | La misma definición puede utilizarse en todo el programa.  |
| Organización  | Reduce la aparición de valores repetidos.                  |

---

# Uso de constantes simbólicas

Sin macro:

```cpp
double area = 3.141592 * radio * radio;
```

Con macro:

```cpp
#define PI 3.141592

double area = PI * radio * radio;
```

La segunda versión es más fácil de comprender.

---

# Ejemplos comunes

```cpp
#define PI 3.141592
#define IVA 0.21
#define MAX_ESTUDIANTES 100
#define DIAS_SEMANA 7
```

---

# Relación con las constantes

Las macros suelen utilizarse para representar valores constantes.

Sin embargo, en C++ moderno se recomienda utilizar:

```cpp
const
```

o

```cpp
constexpr
```

porque ofrecen mayor seguridad y control.

### Ejemplo

```cpp
const double PI = 3.141592;
```

---

# Comparación

| Característica                 | Macro    | Constante (`const`) |
| ------------------------------ | -------- | ------------------- |
| Tipo de dato                   | No posee | Sí posee            |
| Verificación por el compilador | No       | Sí                  |
| Seguridad                      | Menor    | Mayor               |
| Uso recomendado en C++ moderno | Limitado | Sí                  |

---

# Aplicaciones

Las macros se utilizan para:

* Definir constantes simbólicas.
* Configurar programas.
* Evitar números mágicos.
* Mejorar la legibilidad del código.

---

# Errores comunes

| Error                                              | Descripción                         |
| -------------------------------------------------- | ----------------------------------- |
| Usar nombres poco descriptivos                     | Reduce la claridad del programa.    |
| Abusar de macros                                   | Dificulta el mantenimiento.         |
| Confundir macros con variables                     | Las macros no almacenan valores.    |
| Utilizar valores repetidos sin macros o constantes | Reduce la reutilización del código. |

---

# Información complementaria

Para conocer la convención utilizada para constantes, consulte:

* [Convenciones de nombres](../herramientas/01-convensiones-nombres.md)

---

# Conclusión

Las macros permiten definir sustituciones de texto antes de la compilación y facilitan la utilización de valores simbólicos dentro de los programas. Aunque siguen siendo utilizadas, en C++ moderno muchas veces son reemplazadas por constantes definidas mediante `const` o `constexpr`.

---

# Resumen

| Concepto            | Idea principal                                       |
| ------------------- | ---------------------------------------------------- |
| Macro               | Sustitución de texto realizada por el preprocesador. |
| Directiva           | Se define mediante `#define`.                        |
| Ventaja principal   | Mejora la legibilidad y reutilización.               |
| Uso común           | Constantes simbólicas.                               |
| Alternativa moderna | `const` y `constexpr`.                               |
