# Código ASCII

## ¿Qué es el código ASCII?

ASCII (*American Standard Code for Information Interchange*) es un estándar que asigna un valor numérico a caracteres, letras, números y símbolos para que puedan ser almacenados y procesados por una computadora.

Cada carácter posee una representación numérica única.

---

# Importancia

El código ASCII permite:

* Representar caracteres mediante números.
* Facilitar el intercambio de información entre sistemas.
* Almacenar texto en memoria.
* Realizar conversiones entre caracteres y valores numéricos.

---

# Funcionamiento

Internamente, las computadoras almacenan información utilizando valores numéricos.

Por ejemplo:

| Carácter | Código ASCII |
| -------- | ------------ |
| A        | 65           |
| B        | 66           |
| C        | 67           |
| a        | 97           |
| b        | 98           |
| c        | 99           |
| 0        | 48           |
| 1        | 49           |
| 2        | 50           |

---

# Estructura básica

| Rango    | Descripción             |
| -------- | ----------------------- |
| 0 - 31   | Caracteres de control   |
| 32       | Espacio                 |
| 48 - 57  | Dígitos (0-9)           |
| 65 - 90  | Letras mayúsculas (A-Z) |
| 97 - 122 | Letras minúsculas (a-z) |
| 127      | Suprimir (DEL)          |

---

# Caracteres de control

Los primeros códigos ASCII fueron diseñados para controlar dispositivos de entrada y salida.

| Código | Significado           |
| ------ | --------------------- |
| 9      | Tabulación (TAB)      |
| 10     | Salto de línea (LF)   |
| 13     | Retorno de carro (CR) |
| 27     | Escape (ESC)          |

---

# Tabla ASCII básica

| Carácter | Valor |
| -------- | ----- |
| A        | 65    |
| Z        | 90    |
| a        | 97    |
| z        | 122   |
| 0        | 48    |
| 9        | 57    |
| Espacio  | 32    |
| !        | 33    |
| @        | 64    |
| #        | 35    |

---

# Relación con C++

En C++, el tipo de dato `char` almacena un carácter utilizando su código ASCII correspondiente.

### Ejemplo

```cpp
#include <iostream>

using namespace std;

int main() {
    char letra = 'A';

    cout << letra << endl;
    cout << (int)letra << endl;

    return 0;
}
```

### Salida

```text
A
65
```

---

# Conversión entre caracteres y números

Los caracteres pueden convertirse a su valor ASCII y viceversa.

### Ejemplo

```cpp
#include <iostream>

using namespace std;

int main() {
    char letra = 'B';

    cout << (int)letra << endl;

    return 0;
}
```

### Resultado

```text
66
```

---

# Aplicaciones

El código ASCII se utiliza en:

* Procesamiento de texto.
* Validación de caracteres.
* Conversión de datos.
* Comunicaciones entre sistemas.
* Archivos de texto.

---

# Errores comunes

| Error                              | Descripción                        |
| ---------------------------------- | ---------------------------------- |
| Confundir caracteres con números   | '1' es diferente de 1              |
| Ignorar mayúsculas y minúsculas    | 'A' y 'a' poseen valores distintos |
| Utilizar valores ASCII incorrectos | Produce resultados inesperados     |

---

# Curiosidades

| Expresión | Resultado |
| --------- | --------- |
| 'A' + 1   | 'B'       |
| 'a' + 1   | 'b'       |
| '0' + 1   | '1'       |

Esto es posible porque los caracteres se almacenan internamente como números.

---

# Conclusión

El código ASCII es un estándar fundamental para la representación de caracteres en las computadoras. Comprender su funcionamiento facilita el manejo de texto, caracteres y conversiones dentro de los programas.

---

# Resumen

| Concepto    | Idea principal                                    |
| ----------- | ------------------------------------------------- |
| ASCII       | Sistema de codificación de caracteres.            |
| Carácter    | Representado mediante un valor numérico.          |
| char        | Tipo de dato utilizado para almacenar caracteres. |
| Conversión  | Permite obtener el valor numérico de un carácter. |
| Importancia | Base para el procesamiento de texto.              |
