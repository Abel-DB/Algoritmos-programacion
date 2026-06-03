# Lectura y Escritura de Información

## ¿Qué es la entrada y salida de datos?

Todo programa necesita interactuar con el exterior para recibir información y mostrar resultados.

Esta comunicación se realiza mediante dos procesos fundamentales:

* **Entrada (Lectura):** recepción de datos.
* **Salida (Escritura):** presentación de resultados.

---

# Importancia

La entrada y salida de datos permiten:

* Interactuar con el usuario.
* Procesar información.
* Mostrar resultados.
* Dar utilidad práctica a los programas.

Sin entrada ni salida, un programa no podría comunicarse con el exterior.

---

# Conceptos fundamentales

| Concepto        | Descripción                             |
| --------------- | --------------------------------------- |
| Entrada (Input) | Datos que ingresan al programa.         |
| Proceso         | Operaciones realizadas sobre los datos. |
| Salida (Output) | Resultados generados por el programa.   |

---

# Modelo Entrada → Proceso → Salida

Todo programa sigue una estructura básica:

```text
Entrada → Proceso → Salida
```

### Descripción

1. Se reciben los datos de entrada.
2. Se realizan operaciones o cálculos.
3. Se muestran los resultados obtenidos.

---

# Ejemplo conceptual

## Problema

Calcular la suma de dos números.

| Etapa   | Información          |
| ------- | -------------------- |
| Entrada | Número A, Número B   |
| Proceso | A + B                |
| Salida  | Resultado de la suma |

---

# Entrada de datos (Lectura)

La lectura consiste en recibir información desde el exterior del programa.

### Ejemplos

* Ingresar una edad.
* Escribir un nombre.
* Introducir una calificación.
* Leer información desde el teclado.

### Tipos de entrada

| Tipo            | Descripción                           |
| --------------- | ------------------------------------- |
| Manual          | Datos ingresados por el usuario.      |
| Archivo         | Datos obtenidos desde un archivo.     |
| Sistema externo | Datos provenientes de otros sistemas. |

---

# Salida de datos (Escritura)

La escritura consiste en mostrar información hacia el exterior.

### Ejemplos

* Mostrar mensajes.
* Imprimir resultados.
* Presentar reportes.
* Visualizar información en pantalla.

### Tipos de salida

| Tipo                | Descripción                                 |
| ------------------- | ------------------------------------------- |
| Pantalla            | Información mostrada al usuario.            |
| Archivo             | Información almacenada en archivos.         |
| Dispositivo externo | Impresoras, pantallas u otros dispositivos. |

---

# Relación con C++

En C++, la entrada y salida básica se realiza mediante:

| Instrucción | Función                          |
| ----------- | -------------------------------- |
| `cin`       | Leer datos desde el teclado.     |
| `cout`      | Mostrar información en pantalla. |

### Ejemplo

```cpp
#include <iostream>

using namespace std;

int main() {
    int edad;

    cout << "Ingrese su edad: ";
    cin >> edad;

    cout << "Su edad es: " << edad << endl;

    return 0;
}
```

---

# Aplicaciones

La entrada y salida de datos están presentes en prácticamente todos los programas:

* Calculadoras.
* Sistemas bancarios.
* Videojuegos.
* Aplicaciones móviles.
* Sistemas de inventario.
* Software empresarial.

---

# Errores comunes

| Error                            | Descripción                                    |
| -------------------------------- | ---------------------------------------------- |
| No solicitar datos correctamente | El usuario no sabe qué ingresar.               |
| Mostrar información confusa      | Los resultados no son claros.                  |
| No validar entradas              | Se aceptan datos incorrectos.                  |
| Omitir resultados                | El programa procesa datos pero no los muestra. |

---

# Conclusión

La lectura y escritura de información son elementos fundamentales en cualquier programa. Permiten recibir datos, procesarlos y comunicar resultados al usuario, constituyendo la base de la interacción entre una aplicación y su entorno.

---

# Resumen

| Concepto    | Idea principal                                  |
| ----------- | ----------------------------------------------- |
| Entrada     | Recepción de datos.                             |
| Proceso     | Transformación de la información.               |
| Salida      | Presentación de resultados.                     |
| C++         | Utiliza `cin` para leer y `cout` para escribir. |
| Importancia | Permite la interacción con el usuario.          |
