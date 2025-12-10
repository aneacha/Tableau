# 📊 Easy Loans – Loan Analysis Dashboard (Tableau)

Este repositorio contiene el dashboard interactivo desarrollado como parte del caso práctico **Easy Loans**, cuyo objetivo es analizar las operaciones de préstamos realizadas durante el año 2023 y ofrecer insights relevantes para la toma de decisiones estratégicas.

Puedes visualizar el dashboard directamente aquí:  
👉 **[Ver en Tableau Public]([[https://public.tableau.com/shared/F6YPDRQ9W?:display_count=n&:origin=viz_share_link])**

---

## 📝 Descripción del Proyecto

Easy Loans es una empresa financiera que concede préstamos para la adquisición de productos en distintos comercios.  
El objetivo del análisis es:

- Identificar tendencias y comportamientos clave en las operaciones.
- Evaluar la calidad de los préstamos y los reembolsos.
- Destacar riesgos, anomalías y oportunidades de mejora.
- Presentar información clara y accionable mediante visualizaciones interactivas.

El dashboard se creó aplicando **técnicas avanzadas de análisis y visualización con Tableau**, siguiendo buenas prácticas de diseño y usabilidad.

---

## 🧩 Fuentes de Datos

El análisis se basa en el dataset **Easy Loans Operaciones 2023**, compuesto por tres tablas:

- **Orders**: información principal de cada operación (importe, fecha, país, comercio…).
- **Refunds**: registro de reembolsos asociados a órdenes.
- **Merchants**: listado de comercios y sus identificadores.

---

## 🛠️ Modelado de Datos

Se construyó un modelo conectado por relaciones entre:

- `Orders` ↔ `Merchants` (merchant_id)  
- `Orders` ↔ `Refunds` (order_id)

Además:
- Se filtraron las operaciones para incluir solo **países europeos**, excluyendo Marruecos.
- El trabajo se exportó en formato **.twbx** para garantizar su portabilidad.

---

## 📈 Elementos del Dashboard

El proyecto incluye las siguientes visualizaciones clave:

### ✔️ KPIs Principales
Se muestran métricas globales como:
- Valor acumulado  
- Promedio  
- Promedio total (FIXED)  
- Máximo y mínimo  
- Total de comercios  
- Total de reembolsos  

### ✔️ Mapa por País  
Mapa coloreado en función del promedio de los préstamos, permitiendo comparar el rendimiento por regiones.

### ✔️ Gráfico de Áreas  
Evolución del valor acumulado diario, segmentada por país.

### ✔️ Desviaciones  
Visualización que muestra qué préstamos están por encima o por debajo del promedio global.

### ✔️ Parámetro “Valor Préstamo Mínimo”
Incluye:
- Parámetro interactivo  
- Campo calculado para filtrado dinámico  
- Integración con todas las visualizaciones del dashboard  

### ✔️ Filtros Globales
Aplicados a todo el dashboard:
- País  
- Fecha de creación  
- Límite de préstamo mínimo (valor TRUE)

### ✔️ Acciones de Dashboard
Interacción: al hacer clic en un país del mapa, el resto de visualizaciones se resaltan y actualizan.

---

## 🎨 Diseño y Usabilidad

Se aplicaron buenas prácticas de diseño:
- Visualizaciones claras y consistentes  
- Títulos descriptivos  
- Colores y escalas adecuadas  
- Layout limpio y fácil de navegar  

Además, se desarrolló un dashboard alternativo con mejoras de usabilidad y funciones extra.

---

## 📂 Contenido del Repositorio

- `EasyLoans_Dashboard.twbx` — Libro de trabajo empaquetado con todas las visualizaciones  
- `/img` (opcional) — Capturas para previsualización  
- `/data` (opcional) — Dataset si es público  

---

## 🚀 Cómo Abrir el Dashboard

1. Descarga el archivo `.twbx`.
2. Ábrelo en **Tableau Desktop** o **Tableau Public Desktop**.
3. Explora las visualizaciones interactuando con filtros y parámetros.



