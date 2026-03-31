# Cadenas (Strings)

---

## ¿Qué es una cadena?

Una **cadena** es una secuencia de caracteres que pueden ser:

* Letras
* Números
* Símbolos

Ejemplos:

```
"Hola"
"Juan123"
"@correo.com"
```

---

## ¿Cómo funciona una cadena?

Una cadena funciona como un **arreglo de caracteres**, donde cada posición tiene un índice.

```
Posición:   0   1   2   3
           ┌───┬───┬───┬───┐
Cadena:    │ H │ O │ L │ A │
           └───┴───┴───┴───┘
```

- cadena[0] → H
- cadena[3] → A

---

## Características

* Es una secuencia ordenada
* Se accede por índice
* Empieza en 0
* Tiene longitud (tamaño)

---

# Operaciones con cadenas

---

## 1. Recorrer una cadena

Permite mostrar cada carácter.

---

### Diagrama de flujo

```
        ┌───────────┐
        │  INICIO   │
        └─────┬─────┘
              │
        ┌────────────┐
        │ i = 0      │
        └─────┬──────┘
              │
        ┌──────────────┐
        │ ¿i < tamaño? │
        └───┬────┬─────┘
            │    │
           Sí    No
            │    │
   ┌──────────────────┐
   │ Mostrar cadena[i]│ ← Salida (documento)
   └─────┬────────────┘
         │
   ┌──────────────┐
   │ i = i + 1    │
   └─────┬────────┘
         │
         └────────────── (regresa)
              │
        ┌───────────┐
        │   FIN     │
        └───────────┘
```

---

### Prueba de escritorio

Cadena = "HOLA"

| Paso        | i | cadena[i] |
| ----------- | - | --------- |
| Inicializar | 0 | -         |
| Mostrar     | 0 | H         |
| Incremento  | 1 | -         |
| Mostrar     | 1 | O         |
| Incremento  | 2 | -         |
| Mostrar     | 2 | L         |
| Incremento  | 3 | -         |
| Mostrar     | 3 | A         |

---

## 2. Longitud de una cadena

Cantidad de caracteres.

Ejemplo:

```
"HOLA" → 4
```

---

### Prueba de escritorio

| Paso    | Cadena | Tamaño |
| ------- | ------ | ------ |
| Leer    | ANA    | -      |
| Contar  | ANA    | 3      |
| Mostrar | ANA    | 3      |

---

## 3. Comparar cadenas

Permite saber si dos cadenas son iguales.

Ejemplo:

```
"hola" == "hola" → Verdadero
"hola" == "HOLA" → Falso
```

---

### Prueba de escritorio

| cadena1 | cadena2 | Resultado  |
| ------- | ------- | ---------- |
| hola    | hola    | Iguales    |
| hola    | HOLA    | Diferentes |

---

## 4. Concatenar cadenas

Unir cadenas.

Ejemplo:

```
"Hola" + " Mundo" → "Hola Mundo"
```

---

### Prueba de escritorio

| cadena1 | cadena2 | Resultado  |
| ------- | ------- | ---------- |
| Hola    | Mundo   | Hola Mundo |

---

## 5. Acceder a un carácter

Permite obtener una letra específica.

Ejemplo:

```
Cadena = "HOLA"
cadena[1] → O
```

---

### Prueba de escritorio

| Paso    | Posición | Resultado |
| ------- | -------- | --------- |
| Leer    | 1        | -         |
| Mostrar | 1        | O         |

---

## 6. Modificar una cadena

Permite cambiar un carácter.

Ejemplo:

```
"HOLA" → "MOLA"
```

---

### Prueba de escritorio

| Cadena | Posición | Letra | Resultado |
| ------ | -------- | ----- | --------- |
| HOLA   | 0        | M     | MOLA      |

---

## 7. Contar vocales

Ejercicio clásico.

---

### Prueba de escritorio

Cadena = "HOLA"

| Paso | i | Letra | ¿Vocal? | cont |
| ---- | - | ----- | ------- | ---- |
| 1    | 0 | H     | No      | 0    |
| 2    | 1 | O     | Sí      | 1    |
| 3    | 2 | L     | No      | 1    |
| 4    | 3 | A     | Sí      | 2    |

---

## 8. Relación con ASCII

Cada carácter tiene un valor numérico interno.

Ejemplo:

* 'A' → 65
* 'a' → 97

Permite comparar y manipular texto.

---

## 9. Errores comunes

* Pensar que empieza en 1
* Confundir mayúsculas y minúsculas
* Salirse del tamaño
* Comparar mal cadenas

---

## 10. Aplicaciones

* Nombres
* Correos
* Validaciones
* Procesamiento de texto

---

## Conclusión

Las cadenas permiten trabajar con texto y son fundamentales en programación.

Se pueden:

* Recorrer
* Comparar
* Modificar
* Analizar

---

## Resumen

* Una cadena es un conjunto de caracteres
* Funciona como un arreglo
* Se usa para manejar texto
* Permite múltiples operaciones

---
