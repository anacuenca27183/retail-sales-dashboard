# Bussines Analysis de Superstore.

Dashboard interactivo desarrollado en Power BI Desktop para analizar el desempeño de ventas de la empresa Superstore durante el período 2014–2017. El proyecto simula el trabajo de un analista de datos en el sector retail, respondiendo preguntas clave de negocio mediante visualizaciones interactivas y medidas DAX.

# 📊 Retail Sales Dashboard — Superstore Sales Analysis
 
## Descripción del proyecto
 
Dashboard interactivo desarrollado en **Power BI Desktop** para analizar el desempeño de ventas de la empresa Superstore durante el período 2014–2017. El proyecto simula el trabajo de un analista de datos en el sector retail, respondiendo preguntas clave de negocio mediante visualizaciones interactivas y medidas DAX.
 
---
 
## 🛠️ Herramientas y tecnologías
 
- **Power BI Desktop** — modelado de datos, DAX y visualización
- **Power Query** — limpieza y transformación de datos
- **DAX** — medidas calculadas para análisis temporal y financiero
- **Dataset:** [Superstore Sales Dataset — Kaggle](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final)
 
---
 
## 🗂️ Estructura del proyecto
 
### Modelo de datos

<img width="1134" height="705" alt="Modelo estrella" src="https://github.com/user-attachments/assets/f370fef7-191e-45a7-b929-746a97b92c35" />

El proyecto utiliza un **modelo estrella** con 4 tablas relacionadas:
 
- **ORDENES** — tabla de hechos con ventas, ganancias, descuentos y cantidades
- **CLIENTES** — dimensión con segmento, región, estado y ciudad
- **PRODUCTOS** — dimensión con categoría y subcategoría
- **CALENDARIO** — tabla de fechas para análisis temporal
 
### Medidas DAX desarrolladas
- `Total de Ventas` — suma total de ventas
- `Total de Ganancia` — suma total de ganancias
- `Margen` — rentabilidad como porcentaje de ventas
- `Órdenes Totales` — conteo de órdenes únicas
- `Ventas Año Anterior` — ventas del período equivalente del año anterior
- `Crecimiento YoY` — variación porcentual año sobre año
 
---
 
## 📋 Páginas del dashboard
 
### Página 1 — Resumen Ejecutivo
- 5 tarjetas KPI: Ventas, Ganancia, Margen, Órdenes Totales y Crecimiento YoY
- Gráfico de líneas: tendencia de ventas por mes y año
- Segmentadores interactivos por año y categoría
 
### Página 2 — Análisis de Ventas
- Gráfico de barras: ventas totales por categoría

### Página 3 — Ventas por Estado
- Mapa ArcGIS: ventas por estado
- Matriz: ventas y margen por categoría y año
 
### Página 4 - Ventas por Cliente y Producto
- Clientes y Productos
- Top 10 productos más vendidos
- Gráfico de dona: ventas por segmento de cliente
- Scatter plot: rentabilidad por subcategoría (ventas vs ganancia)

### Página 5 - 
- Scatter plor: ganancias vs descuentos
---
 
## 📈 Principales hallazgos
 
### Desempeño general (2014–2017)

<img width="1414" height="807" alt="1 Resumen ejecutivo" src="https://github.com/user-attachments/assets/4668dbb1-45df-4111-afd6-450dfea7db43" />


- Más de **5,000 órdenes** procesadas en el período
- **$2.30 millones** en ventas totales con una ganancia de **$286.40 mil** y un margen de **12.5%**
- Los meses con mayores ventas son **marzo, septiembre, noviembre y diciembre**. Esto podría ser consecuencia de que en el Q4 las ventas aumentan por temporada de regresoescolar y temporada navideña.
 
### Análisis por año
| Año | Ventas | Ganancia | Margen | Crecimiento YoY |
|-----|--------|----------|--------|-----------------|
| 2014 | $484.25 mil | $49.54 mil | 10.2% | NA |
| 2015 | $470.53 mil | $61.62 mil | 13.1% | -2.8% |
| 2016 | $609.21 mil | $81.80 mil | 13.4% | 29.5% |
| 2017 | $733.22 mil | $93.44 mil | 12.7% | 20.4% |
 
- **2017** fue el año de mayor desempeño, con el doble de órdenes (~2,000) respecto a años anteriores (~1,000)
- **2015** fue el año con peor desempeño, registrando un decrecimiento del 2.8% YoY

### Análisis por categoría del periodo
<img width="1408" height="801" alt="2 Analisis de ventas" src="https://github.com/user-attachments/assets/569fd503-bd32-4a18-a6bc-07eb6df6778e" /> 

| Categoría | Subcategorías más vendidas |
|-----------|---------------------------|
| **Tecnología** (mayor margen: 18.4%) | Celulares ($330K), Máquinas ($189K), Accesorios ($167K) |
| **Mobiliario** (margen: 17%)| Sillas ($328K), Tablas ($207K), Estanterías ($115K) |
| **Suministros de oficina** (margen: 2.5%) | Almacenamiento ($224K), Carpetas ($203K), Electrodomésticos ($108K) |

### Análisis geográfico
<img width="1433" height="804" alt="3 Ventas por estado" src="https://github.com/user-attachments/assets/8b0b1e83-2e5e-4659-89b6-edb7bc9efe9c" />

Los 5 estados con mayores ventas:
1. California — $451,036
2. New York — $279,549
3. Texas — $192,758
4. Pennsylvania — $142,838
5. Washington — $133,177

- Este grupo representa el **52% de las ventas totales del periodo**
- Hay una concentración geográfica hacia el Este.

Los 5 estados con menores ventas:
1. Nevada — $1,214
2. Maryland — $1,588
3. Kansas — $1,727
4. District of Columbia — $2,198
5. South Dakota — $2,339

### Segmentos de clientes
<img width="1424" height="807" alt="Clientes y productos" src="https://github.com/user-attachments/assets/8c4ae648-3d74-48fd-87b5-952eb2410056" />

La distribución de ventas de Superstore es la siguiente:

- **Consumo:** 50% de las ventas
- **Corporativo:** 30.74%
- **Home Office:** 18.7%
 
### Top 5 productos más vendidos
1. Canon imageCLASS 2200
2. Fellowes PB500
3. Cisco TelePresence System
4. HON 5400 Series Task
5. GBC DocuBind TL300 Electric Bin

### Rentabilidad por Subcategoría

- **Las subcategorías con mayor rentabilidad son los teléfonos celulares y las sillas con un total de ganancia de $44,515 mil y $26,590 mil respectivamente**
- **Aquellos productos con rentabilidad negativa encontramos las tablas, estanterías y suministros.**

### Ganancia vs Descuentos por subcategoría
<img width="1406" height="803" alt="4 Ganancia total y descuentos promedio por producto" src="https://github.com/user-attachments/assets/023a49d3-70f7-4102-9735-e6b3eeee8cb8" />

- **Como era de esperarse, Tablas, Estanterías y Maquinas son las subcategorías con mayores descuentos aplicados. 




---
 
## 💡 Recomendaciones de negocio
 
### Productos con alta rentabilidad ✅
**Celulares** ($44,515 en ganancia) y **Sillas** ($26,590) son las subcategorías más rentables. Se recomienda mantener e intensificar estrategias de marketing para estos productos.
 
### Productos con rentabilidad negativa ❌
- **Tablas** y **Estanterías** — a pesar de ser los productos más vendidos en Mobiliario, generan pérdidas. Se recomienda reconsiderar su comercialización a menos que funcionen como productos ancla que impulsen la venta de otros artículos complementarios.
- **Suministros** — también presentan rentabilidad negativa. Se sugiere aumentar el precio final, reducir descuentos o negociar con proveedores alternativos.
 
### Productos en zona de alerta ⚠️
**Máquinas, Cierres y Sobres** presentan ganancias marginales positivas. Se recomienda revisar su estructura de costos, incrementar precios o explorar proveedores más competitivos.

### Concentración geográfica hacia el Este 
** Esto podría representar un riesgo para el negocio. ** Se sugiere una estrategia de expansión hacia estados con menor penetración para diversificar el riesgo.

### Impacto de los descuentos en la rentabilidad 🔍
El análisis de descuento promedio por subcategoría revela que **Tables, Bookcases y Machines** son las subcategorías con mayores descuentos aplicados. Esto explica directamente su rentabilidad negativa o marginal — no es un problema de demanda sino de política de precios.
 
**Recomendación:** Reducir o eliminar los descuentos en Tables y Bookcases como primera medida antes de considerar descontinuar su venta. Dado que estos productos tienen alto volumen de ventas, una reducción de descuentos podría mejorar significativamente el margen sin afectar la demanda.
 
---
 
## 🚀 Cómo visualizar el dashboard
 
1. Descarga el archivo `superstore_dashboard.pbix`
2. Ábrelo en **Power BI Desktop** (descarga gratuita en microsoft.com/power-bi)
3. Interactúa con los segmentadores de año y categoría para explorar los datos
 
---
 
## 👩‍💻 Sobre la autora
 
Economista con especialización en análisis cuantitativo y estadística, en transición hacia roles de **Data Analyst** y **Business Intelligence**. Este proyecto forma parte de un portfolio de análisis de datos enfocado en el mercado mexicano.
