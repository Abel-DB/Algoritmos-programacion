# Buenas Prácticas en C++

## ¿Qué son las buenas prácticas?

Las **buenas prácticas** son recomendaciones que ayudan a escribir código más claro, mantenible, seguro y fácil de comprender.

No son reglas obligatorias, pero su aplicación mejora significativamente la calidad del software.

---

# Importancia

Aplicar buenas prácticas permite:

* Mejorar la legibilidad del código.
* Facilitar el mantenimiento.
* Reducir errores.
* Favorecer el trabajo en equipo.
* Crear programas más organizados.

---

# Utilizar nombres descriptivos

Los nombres deben reflejar claramente el propósito del elemento.

### Correcto

```cpp
int edad_usuario;
float promedio_final;
```

### Incorrecto

```cpp
int x;
float a;
```

---

# Seguir una convención de nombres

Utilizar una única convención en todo el proyecto.

### Ejemplo

```cpp
int edad_usuario;
float salario_mensual;

void calcularPromedio();
```

> Consulte: [Convenciones de nombres](../Anexos/1-convensiones_nombres.md)

---

# Inicializar variables

Toda variable debe recibir un valor inicial antes de utilizarse.

### Correcto

```cpp
int contador = 0;
float promedio = 0.0f;
```

### Incorrecto

```cpp
int contador;
float promedio;
```

---

# Mantener una indentación consistente

La indentación facilita la lectura y comprensión del código.

### Correcto

```cpp
if (edad >= 18) {

    cout << "Mayor de edad" << endl;

}
```

### Incorrecto

```cpp
if (edad >= 18) {
cout << "Mayor de edad" << endl;
}
```

---

# Utilizar comentarios cuando aporten valor

Los comentarios deben explicar el propósito o la intención del código.

### Correcto

```cpp
// Calcula el promedio final del estudiante
promedio = suma / cantidad;
```

### Incorrecto

```cpp
// Suma dos números
suma = a + b;
```

El código simple suele explicarse por sí mismo.

---

# Evitar código duplicado

Si una misma lógica se repite varias veces, debe reorganizarse para evitar duplicación.

### Incorrecto

```cpp
cout << "Bienvenido" << endl;
cout << "Bienvenido" << endl;
cout << "Bienvenido" << endl;
```

---

# Mantener funciones con una sola responsabilidad

Cada función debería realizar una tarea específica.

### Correcto

```cpp
leerDatos();
calcularPromedio();
mostrarResultado();
```

---

# Utilizar constantes para valores fijos

Los valores que no cambian deben almacenarse como constantes.

### Correcto

```cpp
const double PI = 3.141592;
const int MAX_INTENTOS = 3;
```

### Incorrecto

```cpp
area = 3.141592 * radio * radio;
```

---

# Mantener el código simple

La solución más simple suele ser la mejor.

### Recomendación

* Evitar complejidad innecesaria.
* Resolver el problema paso a paso.
* Priorizar la claridad.

---

# Probar los programas

Antes de considerar terminado un programa:

* Verificar entradas válidas.
* Verificar entradas inválidas.
* Probar casos límite.
* Realizar pruebas de escritorio cuando sea necesario.

> Consulte: [Pruebas de escritorio](../Tema04_resolucion_problemas/4-pruebas_escritorio.md)

---

# Formato recomendado

## Llaves

```cpp
if (condicion) {

    instrucciones;

}
```

---

## Espacios

```cpp
suma = numero1 + numero2;
```

Evitar:

```cpp
suma=numero1+numero2;
```

---

# Recomendaciones generales

| Recomendación                 | Beneficio               |
| ----------------------------- | ----------------------- |
| Utilizar nombres descriptivos | Facilita la comprensión |
| Mantener consistencia         | Mejora la organización  |
| Inicializar variables         | Evita errores           |
| Utilizar constantes           | Aumenta la claridad     |
| Probar el programa            | Reduce fallos           |
| Evitar duplicación            | Facilita mantenimiento  |
| Indentar correctamente        | Mejora la lectura       |

---

# Errores comunes

| Error                     | Consecuencia               |
| ------------------------- | -------------------------- |
| Variables sin inicializar | Valores inesperados        |
| Nombres poco descriptivos | Código difícil de entender |
| Falta de indentación      | Menor legibilidad          |
| Código duplicado          | Mayor mantenimiento        |
| Comentarios innecesarios  | Ruido visual               |
| No realizar pruebas       | Errores en ejecución       |

---

# Información complementaria

Para mantener consistencia en los nombres consulte:

* [Convenciones de nombres](../Anexos/1-convensiones_nombres.md)

Para comprender el proceso de validación de algoritmos consulte:

* [Pruebas de escritorio](../Tema04_resolucion_problemas/4-pruebas_escritorio.md)

---

# Conclusión

Las buenas prácticas ayudan a desarrollar programas más claros, organizados y fáciles de mantener. Adoptarlas desde el inicio favorece la creación de hábitos que serán útiles durante toda la carrera profesional.

---

# Resumen

| Práctica                    | Objetivo      |
| --------------------------- | ------------- |
| Nombres descriptivos        | Claridad      |
| Convenciones consistentes   | Organización  |
| Inicialización de variables | Seguridad     |
| Indentación correcta        | Legibilidad   |
| Uso de constantes           | Mantenimiento |
| Pruebas                     | Calidad       |
| Código simple               | Comprensióne  |
