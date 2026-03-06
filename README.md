# 🍽️ Gestor de Restaurante (Python + Tkinter + SQLite)

Aplicación de escritorio desarrollada en **Python** utilizando **Tkinter** para la interfaz gráfica y **SQLite** para la base de datos.

El sistema permite gestionar:

- Clientes
- Órdenes
- Ventas
- Estadísticas del restaurante

También permite exportar información a archivos `.txt` y visualizar estadísticas en consola usando **Rich**.

---

# 📌 Características del sistema

## 👤 Gestión de Clientes

El sistema permite administrar clientes del restaurante.

Funciones disponibles:

- Ver clientes
- Agregar clientes
- Eliminar clientes
- Modificar clientes
- Exportar clientes a archivo `.txt`

Datos registrados:

- Nombre del cliente
- Número de orden
- DNI

---

# 🍽️ Gestión de Órdenes

Permite registrar los platos que pide cada mesa.

Funciones disponibles:

- Ver órdenes
- Agregar orden
- Eliminar orden
- Modificar orden
- Exportar órdenes a archivo `.txt`

Datos registrados:

- Número de mesa
- Nombre del plato
- Precio

---

# 💰 Gestión de Ventas

El sistema registra las ventas realizadas en el restaurante.

Funciones disponibles:

- Ver ventas
- Agregar venta
- Eliminar venta
- Exportar ventas a archivo `.txt`

Datos registrados:

- Cliente
- Número de orden
- DNI
- Número de mesa
- Plato solicitado
- Precio

Las ventas se almacenan automáticamente en la base de datos **SQLite**.

---

# 📊 Estadísticas

El sistema incluye algunas estadísticas básicas del restaurante.

### 📋 Ver menú de platos
Muestra en consola el menú disponible con precios.

### 🍛 Lista de clientes por plato
Permite seleccionar un plato y ver los clientes que lo ordenaron.

### 🥇 Plato más vendido
Calcula cuál es el plato más vendido en el restaurante.

### 💵 Total generado por día
Muestra el total de dinero generado durante el día.

El sistema reinicia automáticamente el total cuando detecta un nuevo día.

---

# 🍛 Menú de Platos

| Plato | Precio |
|------|------|
| Lomo saltado | S/30 |
| Ají de gallina | S/26 |
| Arroz con pollo | S/25.45 |
| Pollo a la brasa | S/35.50 |
| Ceviche | S/30 |
| Tallarines rojos | S/21.72 |

---

# 🛠 Tecnologías utilizadas

- **Python**
- **Tkinter** → interfaz gráfica
- **SQLite3** → base de datos
- **Rich** → salida avanzada en consola
- **Tabulate** → exportación de tablas a texto

---

# 📂 Estructura del proyecto

```
GestorRestaurante/
│
├── restaurante.py
├── restaurante2026.db
├── Clientes_restaurante2026.txt
├── Ordenes_clientes2026.txt
├── Ventas_restaurante2026.txt
└── README.md
```

---

# 🗄 Base de Datos

El sistema utiliza una base de datos SQLite con la tabla:

```
Restaurante_tabla2026
```

Columnas de la tabla:

| Campo | Tipo |
|------|------|
| Cliente | TEXT |
| Nro_orden | INT |
| DNI | INT |
| Nro_mesa | INT |
| Nombre_plato | TEXT |
| Precio | DOUBLE |

---

# ▶ Cómo ejecutar el programa

## 1️⃣ Instalar Python

Descargar Python desde:

https://www.python.org

---

## 2️⃣ Instalar dependencias

Ejecutar en la terminal:

```
pip install rich
pip install tabulate
```

---

## 3️⃣ Ejecutar el programa

```
python restaurante.py
```

---

# ⌨ Controles del programa

- **ESC** → cerrar la aplicación

---

# 📁 Archivos generados

El sistema genera automáticamente archivos de texto con información del sistema.

| Archivo | Contenido |
|------|------|
| Clientes_restaurante2026.txt | Lista de clientes |
| Ordenes_clientes2026.txt | Órdenes registradas |
| Ventas_restaurante2026.txt | Ventas del restaurante |

---

# 📈 Posibles mejoras futuras

- Sistema de login para administradores
- Gráficos de ventas
- Reportes mensuales
- Exportación a Excel
- Interfaz más moderna con **CustomTkinter**
- Sistema de facturación automática
- Control de inventario

---

# 👨‍💻 Autor
- Utrilla Solis, Angel Kyle

Proyecto desarrollado en **Python** como sistema de gestión de restaurante utilizando:

- **Interfaces gráficas**
- **Bases de datos**
- **Estadísticas en consola**

---
