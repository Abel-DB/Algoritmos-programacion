# Lectura y escritura de información

## Introducción
La lectura y escritura de información permite que un programa interactúe con el usuario.

- **Lectura (entrada)**: el programa recibe datos
- **Escritura (salida)**: el programa muestra resultados

Sin estas operaciones, un programa no puede comunicarse con el usuario.

---

## 1. Lectura de información (Entrada)

La lectura de información consiste en **recibir datos desde el usuario** durante la ejecución del programa.

Estos datos se almacenan en variables para ser utilizados posteriormente.

---

### Lectura en C++
En C++ se utiliza `cin` para leer datos desde el teclado.

```cpp
    #include <iostream>
    using namespace std;

    int main() {
        int numero;
        cin >> numero;
        return 0;
    }
```

El valor ingresado por el usuario se guarda en la variable `numero`.

---

### Lectura en Python
En Python se utiliza la función `input()`.

```Python
    numero = input("Ingrese un número: ")
```

`input()` siempre devuelve un dato en formato texto.

---

## 2. Escritura de información (Salida)

La escritura de información consiste en **mostrar datos al usuario** en pantalla.

---

### Escritura en C++
Se utiliza `cout` para mostrar información.

```cpp
    #include <iostream>
    using namespace std;

    int main() {
        cout << "Hola mundo";
        return 0;
    }
```

El operador `<<` permite enviar datos a la salida.

---

### Escritura en Python
Se utiliza la función `print()`.

```Python
    print("Hola mundo")
```

---

## 3. Uso combinado de entrada y salida

En la mayoría de los programas se combinan ambas operaciones:
1. Se leen datos
2. Se procesan
3. Se muestran resultados

---

### Ejemplo en C++

```cpp
    #include <iostream>
    using namespace std;

    int main() {
        int numero;
        cin >> numero;
        cout << "El número es: " << numero;
        return 0;
    }
```

---

### Ejemplo en Python

```Python
    numero = input("Ingrese un número: ")
    print("El número es:", numero)
```

---

## 4. Errores comunes

### Error en C++
Uso incorrecto del operador:

```cpp
    cin << numero;
```

Incorrecto, debe ser:

```cpp
    cin >> numero;
```

---

### Error en Python
Olvidar que `input()` devuelve texto:

```Python
    numero = input("Ingrese un número: ")
    print(numero + 5)
```

Puede producir un error o comportamiento incorrecto

---

## Resumen final

- La **lectura** permite recibir datos del usuario  
- La **escritura** permite mostrar información  
- En C++ se usa `cin` y `cout`  
- En Python se usa `input()` y `print()`  

---

## Idea clave

Todo programa básico necesita **leer datos, procesarlos y mostrar resultados**.
