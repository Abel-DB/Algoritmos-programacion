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

# Conversión entre caracteres y números

Cada carácter posee una representación numérica asociada.

Por ejemplo:

| Carácter | Valor ASCII |
| -------- | ----------- |
| A        | 65          |
| B        | 66          |
| C        | 67          |
| 1        | 49          |
| 2        | 50          |
| 3        | 51          |

Gracias a esta representación, los sistemas informáticos pueden almacenar y procesar texto utilizando valores numéricos.

---

# Relación entre caracteres y números

Los caracteres pueden ordenarse y compararse utilizando sus valores ASCII.

Por ejemplo:

```text
A → 65
B → 66
C → 67
```

Como 66 es mayor que 65, el carácter B se encuentra después de A.

---

# Curiosidades

Debido a que los caracteres poseen valores numéricos asociados, es posible establecer relaciones entre ellos.

| Relación           |
| ------------------ |
| A está antes que B |
| a está antes que b |
| 0 está antes que 1 |

Estas relaciones permiten ordenar texto y realizar comparaciones entre caracteres.

---

# Aplicaciones

El código ASCII se utiliza en:

* Procesamiento de texto.
* Validación de caracteres.
* Conversión de datos.
* Comunicaciones entre sistemas.
* Archivos de texto.
* Ordenamiento de caracteres.

---

# Errores comunes

| Error                              | Descripción                              |
| ---------------------------------- | ---------------------------------------- |
| Confundir caracteres con números   | El carácter 1 es diferente del número 1. |
| Ignorar mayúsculas y minúsculas    | A y a poseen valores distintos.          |
| Utilizar valores ASCII incorrectos | Produce resultados inesperados.          |

---

# Conclusión

El código ASCII es un estándar fundamental para la representación de caracteres en las computadoras. Comprender su funcionamiento facilita el manejo de texto, caracteres y conversiones dentro de algoritmos y sistemas informáticos.

---

# Resumen

| Concepto     | Idea principal                                                          |
| ------------ | ----------------------------------------------------------------------- |
| ASCII        | Sistema de codificación de caracteres.                                  |
| Carácter     | Representado mediante un valor numérico.                                |
| Conversión   | Relación entre caracteres y números.                                    |
| Aplicaciones | Procesamiento y almacenamiento de texto.                                |
| Importancia  | Base para la representación de caracteres en los sistemas informáticos. |
