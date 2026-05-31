# Estructuras

## ¿Qué es una estructura?

Una **estructura** (*struct*) es una estructura de datos que permite agrupar variables de diferentes tipos bajo un mismo nombre.

Las estructuras facilitan la representación de entidades u objetos del mundo real.

---

# Importancia

Las estructuras permiten:

* Organizar información relacionada.
* Agrupar datos bajo una única entidad.
* Mejorar la legibilidad del código.
* Facilitar el manejo de información compleja.

---

# Conceptos fundamentales

| Concepto       | Descripción                                 |
| -------------- | ------------------------------------------- |
| Estructura     | Agrupación de variables relacionadas.       |
| Miembro        | Variable que pertenece a una estructura.    |
| Instancia      | Variable creada a partir de una estructura. |
| Tipo compuesto | Tipo formado por varios datos.              |

---

# Problema que resuelven

Sin estructuras:

```cpp
string nombre;
int edad;
float promedio;
```

A medida que aumenta la cantidad de datos, resulta más difícil mantenerlos organizados.

Con estructuras:

```cpp
Estudiante alumno;
```

Toda la información queda agrupada bajo una misma entidad.

---

# Sintaxis básica

```cpp
struct NombreEstructura {
    tipo miembro1;
    tipo miembro2;
};
```

---

# Ejemplo

```cpp
struct Estudiante {
    string nombre;
    int edad;
    float promedio;
};
```

En este ejemplo:

| Miembro  | Tipo   |
| -------- | ------ |
| nombre   | string |
| edad     | int    |
| promedio | float  |

---

# Creación de instancias

Una vez definida la estructura, pueden crearse variables de ese tipo.

### Ejemplo

```cpp
Estudiante alumno;
```

---

# Acceso a los miembros

Se utiliza el operador punto (`.`).

### Ejemplo

```cpp
alumno.nombre = "Juan";
alumno.edad = 20;
alumno.promedio = 85.5;
```

---

# Lectura y escritura

### Lectura

```cpp
cin >> alumno.nombre;
cin >> alumno.edad;
```

### Escritura

```cpp
cout << alumno.nombre << endl;
cout << alumno.edad << endl;
```

---

# Ejemplo completo

```cpp
#include <iostream>
#include <string>

using namespace std;

struct Estudiante {
    string nombre;
    int edad;
    float promedio;
};

int main() {
    Estudiante alumno;

    alumno.nombre = "Juan";
    alumno.edad = 20;
    alumno.promedio = 85.5;

    cout << alumno.nombre << endl;
    cout << alumno.edad << endl;
    cout << alumno.promedio << endl;

    return 0;
}
```

---

# Representación conceptual

```text
Estudiante
│
├── nombre   → Juan
├── edad     → 20
└── promedio → 85.5
```

---

# Ventajas

| Ventaja       | Descripción                           |
| ------------- | ------------------------------------- |
| Organización  | Agrupa información relacionada.       |
| Claridad      | Facilita la lectura del código.       |
| Reutilización | Permite crear múltiples instancias.   |
| Escalabilidad | Facilita el crecimiento de programas. |

---

# Limitaciones

| Limitación                 | Descripción                          |
| -------------------------- | ------------------------------------ |
| No contiene comportamiento | Solo almacena datos.                 |
| Requiere definición previa | Debe declararse antes de utilizarse. |

> **Nota:** Más adelante, en Programación Orientada a Objetos, se estudiarán las clases, que permiten combinar datos y comportamiento.

---

# Aplicaciones

Las estructuras se utilizan para representar:

* Estudiantes.
* Productos.
* Empleados.
* Clientes.
* Vehículos.
* Registros de información.

---

# Relación con la memoria

Cada instancia de una estructura reserva memoria para todos sus miembros.

```text
Estudiante alumno

nombre   → "Juan"
edad     → 20
promedio → 85.5
```

---

# Errores comunes

| Error                             | Descripción                            |
| --------------------------------- | -------------------------------------- |
| Olvidar el punto (`.`)            | Impide acceder a los miembros.         |
| Utilizar miembros inexistentes    | Genera errores de compilación.         |
| Confundir estructura con variable | Una estructura define un tipo.         |
| No inicializar los miembros       | Puede producir valores indeterminados. |

---

# Información complementaria

Para conocer la convención utilizada para nombrar estructuras, consulte:

* [Convenciones de nombres](../Anexos/convensiones_nombres.md)

Para comprender los tipos de datos utilizados dentro de una estructura, consulte:

* [Variables y tipos de datos](../Tema02_Datos/1-variables_tipos_datos.md)

---

# Conclusión

Las estructuras permiten agrupar datos relacionados bajo una misma entidad, facilitando la organización y el manejo de información dentro de los programas. Constituyen una herramienta fundamental para representar objetos del mundo real y sirven como base para conceptos más avanzados de programación.

---

# Resumen

| Concepto          | Idea principal                              |
| ----------------- | ------------------------------------------- |
| Estructura        | Agrupa variables relacionadas.              |
| Miembro           | Variable perteneciente a una estructura.    |
| Instancia         | Variable creada a partir de una estructura. |
| Operador `.`      | Permite acceder a los miembros.             |
| Ventaja principal | Organización de datos relacionados.         |
