# Símbolos de Diagramas de Flujo

| Símbolo | Nombre | Descripción |
|--------|--------|-------------|


graph TD
    A([Inicio]) --> B[/Leer número n/]
    B --> C{¿n > 0?}
    C -- Sí --> D[Imprimir 'Positivo']
    C -- No --> E[Imprimir 'Negativo']
    D --> F([Fin])
    E --> F([Fin])


| ```text
   _________
  /         \
 |  INICIO   |
  \_________/
``` | Óvalo / Terminal | Representa el **inicio** o **fin** del algoritmo. |
| ```text
 ┌───────────┐
 │ Proceso   │
 └───────────┘
``` | Rectángulo | Indica una **operación**, cálculo o instrucción. |
| ```text
   /──────────/
  / Entrada  /
 /__________/
``` | Paralelogramo | Representa **entrada o salida de datos**. |
| ```text
      /\
     /  \
    / ?  \
    \    /
     \  /
      \/
``` | Diamante / Rombo | Representa una **decisión** o condición (`if`, `while`, `switch`). |
| ```text
      ________
     /        \
    /          \
    \          /
     \________/
``` | Hexágono | Representa **preparación / inicialización** (`for`, variables iniciales). |
| ```text
      ________
     /        |
    /         |
    \         |
     \________|
``` | Hexágono lateral | Representación didáctica para ciclo **while**. |
| ```text
 ┌───────────┐
 │ Documento │~
 └───────────┘
``` | Documento | Representa una **salida impresa** o reporte. |
| ```text
      ○
``` | Conector | Une partes del diagrama cuando continúa en otro punto. |
| ```text
────────────►
``` | Flecha / Línea de flujo | Indica la **dirección** del proceso. |
| ```text
   _________
  /         \
 | Subrutina |
 |-----------|
  \_________/
``` | Proceso predefinido | Llamada a una función o procedimiento ya definido. |
| ```text
    _______
   / _____ \
  | |     | |
  | |_____| |
   \_______/
``` | Base de datos / Almacenamiento | Representa almacenamiento de datos o archivos. |

---

# Resumen rápido

| Símbolo | Uso |
|--------|-----|
| Óvalo | Inicio / Fin |
| Rectángulo | Proceso |
| Paralelogramo | Entrada / Salida |
| Diamante | Decisión |
| Hexágono | Inicialización |
| Documento | Reporte |
| Flecha | Dirección |
| Conector | Unión |
| Base de datos | Almacenamiento |

---
