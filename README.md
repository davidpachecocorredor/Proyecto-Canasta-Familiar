# 🛒 Análisis de Precios de la Canasta Familiar — Dashboard Económico

## Excel | Power Query | Power BI | DAX

📌 Descripción del Proyecto

Este proyecto consiste en el análisis económico de los precios de la canasta familiar en el Eje Cafetero (Colombia).
Se desarrolló un proceso completo de ETL, modelado de datos, creación de indicadores económicos y construcción de un tablero interactivo en Power BI .

El análisis permite entender la evolución de precios, inflación mensual, volatilidad e IPC , para Cuidad , Categoria , Producto y Mercado.

## 🎯 Objetivos 
- Identificar tendencias de precios en el tiempo.

- Medir la inflación mensual y por categoría.

- Detectar productos con alta volatilidad.

- Comparar variaciones entre ciudades y tipos de productos.

- Construir un tablero económico profesional.

📂 Conjunto de datos utilizado

Archivo: Historico_de_Precios_Productos_Canasta_Familiar.csv

Columnas principales:

- Fecha Final

- Ciudad
 
- Mercado
  
- Producto

- Categoria

- Precio Mínimo, Máximo y Medio

## 🔧 Proceso ETL (Power Query)

Las transformaciones principales fueron:

- Limpieza de precios → conversión de texto a número

- Unificación de formato de fecha

- Normalización de nombres de mercados y ciudades.

- Eliminación de duplicados
 
- Construcción de tabla calendario

## 📘 Modelado de Datos

 **Modelo en estrella:**

- Tablas Hechos: Precios_Limpios

- Dimensión: Calendario

- Relación: Calendario[Fecha] → Precios_Limpios[Fecha Final]
(1 a muchos, filtro en ambas direcciones)

## 📊 Indicadores (KPIs) construidos en DAX
🟦 1. Precio Promedio por Mes

🟩 2. Inflación Mensual (Variación % mes a mes)

🟧 3. Media Móvil 30 días

🟥 4. Volatilidad

🟨 5. IPC Base 100

## 📈 Visualizaciones del Dashboard

🔹 Gráfico 1 — Tendencia de Inflación vs Media Móvil

🔹 Gráfico 2 — Mapa por Ciudad (ArcGIS)

🔹 Gráfico 3 — Mapa de calor de Categorías

🔹 Gráfico 4 — Producto por Precio

🔹 Gráfico 5 — Inflación por Producto 
## Opciones de Mejora

- Automatización del proceso ETL con Power Automate

- Implementación de un modelo predictivo en Python

- Análisis más profundo incorporando nuevas variables, por ejemplo:

     1. Cantidades vendidas/registradas

     2. Estandarización de unidades
        - (Ej.: café o leche pueden aparecer con precios altos porque no se especifica unidad → bulto, litro, kilo, etc.)

     3. Ingresos y salidas por cantidades , permitiendo métricas como costos unitarios, márgenes o demanda real
        
## Preguntas y Respuestas propuestas 

1. ¿Qué productos presentan mayor inflación mensual?
- Papaya tainung
- Merkuza filetiada
- Zanahoria
- Yuca
  
2. ¿Cuáles son los más volátiles?
- Arracacha amarilla
- Cilantro
- Menudencias de Pollo
- Mango Tommy
  
3. ¿Qué ciudades muestran los mayores incrementos de precios?
- Ibague
- Manizales
  
4. ¿Qué categorías son menos volatiles?
- Carnes
- Granos y Cereales
  
5. ¿Qué categorías son más Economicas?
-  Verdururas y Hortalizas
-  TUberculos y Raices.
  
6. ¿Cuál es la tendencia general del IPC?
   
- Como índice agregado, el IPC muestra una tendencia creciente natural respecto a su base (100)
  
- Se observa un fuerte aumento entre 2024 y 2025
  
- El crecimiento más reciente es impulsado principalmente por:
    - Pescados
    - Productos Procesados
      
## 📎 Archivos incluidos
[Dataset Link] (https://www.datos.gov.co/Agricultura-y-Desarrollo-Rural/Historico-de-Precios-Productos-de-la-Canasta-Famil/gdqq-rry2/about_data)

[Descargar dataset](DATA)

[Dashboard Power BI (.pbix)](PowerBi)


## 👤 Autor

David Orlando Pacheco Corredor

|Analista de Datos | Econometria | BI | Ciencia de Datos| Economía|
