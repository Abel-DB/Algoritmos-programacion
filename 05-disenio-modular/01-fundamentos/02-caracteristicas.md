# Características del Diseño Modular

## Introducción

El diseño modular divide un programa en módulos independientes que colaboran para resolver un problema.

Para que esta metodología sea efectiva, los módulos deben cumplir ciertas características que favorecen la organización, comprensión y mantenimiento del software.

---

# Importancia

Las características del diseño modular permiten:

- Organizar mejor los programas.
- Reducir la complejidad de los problemas.
- Facilitar el mantenimiento.
- Mejorar la reutilización del código.
- Favorecer el trabajo colaborativo.

---

# Características principales

## 1. División del problema

Un problema complejo se divide en problemas más pequeños y manejables.

Cada módulo se encarga de resolver una parte específica del problema general.

### Ejemplo

```text
Sistema de Ventas
│
├── Gestión de Clientes
├── Gestión de Productos
├── Facturación
└── Reportes
```

---

## 2. Independencia

Cada módulo debe funcionar de manera relativamente independiente de los demás.

Esto permite modificar un módulo sin afectar significativamente al resto del sistema.

### Ejemplo

```text
Módulo Clientes
```

puede modificarse sin necesidad de cambiar:

```text
Módulo Facturación
```

---

## 3. Responsabilidad única

Cada módulo debe realizar una única tarea o responsabilidad específica.

### Correcto

```text
calcularPromedio()
```

### Incorrecto

```text
calcularPromedioYGuardarYMostrar()
```

Mientras más específica sea la tarea, más fácil será mantener el módulo.

---

## 4. Reutilización

Un módulo puede utilizarse varias veces dentro de un mismo programa o incluso en otros programas.

### Ejemplo

```text
calcularIVA()
```

puede utilizarse en:

- Sistema de ventas.
- Sistema de inventario.
- Sistema de facturación.

---

## 5. Comunicación entre módulos

Los módulos no trabajan aislados; necesitan intercambiar información.

La comunicación se realiza mediante datos de entrada y resultados de salida.

### Ejemplo

```text
leerNotas()
        ↓
calcularPromedio()
        ↓
mostrarResultado()
```

---

## 6. Organización jerárquica

Los módulos suelen organizarse en distintos niveles.

Generalmente existe un módulo principal que coordina la ejecución de los demás.

### Ejemplo

```text
Programa Principal
│
├── Módulo A
├── Módulo B
└── Módulo C
```

---

## 7. Facilidad de mantenimiento

Al estar dividido en módulos, los errores pueden localizarse y corregirse con mayor facilidad.

### Ejemplo

Si existe un error en:

```text
calcularPromedio()
```

solo es necesario revisar ese módulo.

---

# Relación con funciones y procedimientos

Las funciones y procedimientos son herramientas que permiten implementar módulos.

```text
Diseño Modular
        │
        ▼
Funciones y Procedimientos
        │
        ▼
Módulos
```

Más adelante se estudiará cómo construir módulos utilizando funciones y procedimientos.

---

# Ejemplo práctico

Supongamos un sistema académico.

```text
Programa Principal
│
├── Registrar Estudiantes
├── Registrar Notas
├── Calcular Promedio
└── Mostrar Reporte
```

Cada módulo tiene una responsabilidad específica y trabaja junto a los demás para resolver el problema completo.

---

# Buenas prácticas

- Asignar una responsabilidad clara a cada módulo.
- Evitar módulos demasiado grandes.
- Mantener independencia entre módulos.
- Reutilizar módulos cuando sea posible.
- Diseñar módulos fáciles de mantener.

---

# Conclusión

El diseño modular se caracteriza por dividir un programa en módulos independientes, organizados y especializados. Estas características permiten desarrollar software más claro, reutilizable y fácil de mantener.

---

# Resumen

| Característica | Descripción |
|----------------|-------------|
| División del problema | Separa el problema en partes más pequeñas. |
| Independencia | Los módulos funcionan de forma relativamente autónoma. |
| Responsabilidad única | Cada módulo realiza una tarea específica. |
| Reutilización | Los módulos pueden utilizarse varias veces. |
| Comunicación | Intercambian información entre sí. |
| Organización jerárquica | Existe coordinación entre módulos. |
| Mantenimiento | Facilita correcciones y mejoras. |
