# Estructura de un Programa en C++

## Introducción

Todo programa en C++ sigue una estructura básica compuesta por diferentes elementos que permiten organizar el código y definir el punto de inicio de la ejecución.

Comprender esta estructura facilita la lectura, escritura y mantenimiento de programas.

---

# Programa Básico

```cpp
#include <iostream>

using namespace std;

int main() {
    cout << "Hola Mundo" << endl;

    return 0;
}
```

---

# Estructura General

```text
Directivas
    ↓
Espacios de nombres
    ↓
Función principal (main)
    ↓
Instrucciones
    ↓
Finalización
```

---

# 1. Directivas del Preprocesador

Las directivas indican al compilador qué recursos debe incorporar antes de compilar el programa.

Ejemplo:

```cpp
#include <iostream>
```

### Función

Permite utilizar:

```cpp
cout
cin
endl
```

---

# 2. Espacios de Nombres

Ejemplo:

```cpp
using namespace std;
```

### Función

Permite utilizar:

```cpp
cout
cin
string
```

sin escribir:

```cpp
std::cout
std::cin
std::string
```

---

# 3. Función Principal

Todo programa en C++ comienza su ejecución en la función:

```cpp
int main()
```

Ejemplo:

```cpp
int main() {

}
```

### Importancia

Es el punto de entrada del programa.

Cuando se ejecuta:

```bash
./programa
```

el sistema operativo busca y ejecuta la función `main()`.

---

# 4. Bloque de Código

Las llaves delimitan el cuerpo de una función.

```cpp
int main() {

}
```

Todo lo que se encuentre dentro de las llaves pertenece a la función.

---

# 5. Instrucciones

Las acciones que realiza el programa se escriben mediante instrucciones.

Ejemplo:

```cpp
cout << "Hola Mundo";
```

Cada instrucción normalmente termina con:

```cpp
;
```

---

# 6. Valor de Retorno

Ejemplo:

```cpp
return 0;
```

### Función

Indica que el programa terminó correctamente.

Valor habitual:

```cpp
0
```

---

# Flujo de Ejecución

Cuando se ejecuta un programa:

```text
Sistema Operativo
        ↓
      main()
        ↓
 Ejecutar instrucciones
        ↓
    return 0
        ↓
      Finalizar
```

---

# Ejemplo Comentado

```cpp
#include <iostream>      // Biblioteca estándar

using namespace std;     // Espacio de nombres

int main() {             // Punto de entrada

    cout << "Hola";      // Instrucción

    return 0;            // Finalización correcta
}
```

---

# Errores Comunes

## Falta de punto y coma

```cpp
cout << "Hola"
```

Error:

```text
expected ';'
```

---

## Olvidar las llaves

```cpp
int main()
```

Error:

```text
expected '{'
```

---

## No definir main()

```cpp
#include <iostream>
```

Error durante el enlazado:

```text
undefined reference to main
```

---

# Resumen

| Elemento              | Función                                       |
| --------------------- | --------------------------------------------- |
| `#include`            | Incorporar bibliotecas                        |
| `using namespace std` | Acceder a elementos de la biblioteca estándar |
| `main()`              | Punto de entrada                              |
| `{}`                  | Delimitar bloques                             |
| `;`                   | Finalizar instrucciones                       |
| `return 0`            | Finalizar correctamente                       |

---

# Idea Clave

Todo programa en C++ necesita una función principal llamada:

```cpp
int main()
```

La ejecución comienza en ella y continúa con las instrucciones contenidas dentro de sus llaves.
