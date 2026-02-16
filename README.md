# Proyecto BI: Análisis de Ventas de Tienda Online

## Objetivo del proyecto
Desarrollar un dashboard ejecutivo que permita analizar el rendimiento de ventas, clientes y productos de una tienda online.  
El proyecto utiliza un KPIs estratégicos y visualizaciones interactivas para tomar decisiones informadas sobre inversión en productos, fidelización de clientes y estrategias de marketing.

## KPIs principales
- **Ventas Totales:** Ingresos globales de la tienda.  
- **Ticket Promedio:** Promedio de gasto por compra.  
- **Clientes:** Número de clientes adquiridos en el periodo.    
- **Ventas por Categoría / Producto:** Identificación de productos más demandados.  

## Insights clave
- La categoría **Accesorios** impulsa la mayor parte del crecimiento de ventas.  
- El país **España** muestra mayor crecimiento en ventas que México, sugiriendo expansión de marketing.  
- Productos estrella identificados permiten ajustar inventario y promociones estratégicas.Más vendido son los sombreros  


## Decisiones clave según insights

Categoría Accesorios impulsa ventas → aumentar stock, lanzar campañas específicas, evaluar proveedores.

Clientes recurrentes aportan 30% ingresos → crear programas de fidelización, ofertas personalizadas, diseñar packs para aumentar ticket promedio.

España con mayor crecimiento → invertir en marketing, optimizar logística, explorar nuevas categorías.

Productos estrella identificados → priorizar inventario, promociones cruzadas, ajustar precios estratégicamente.

Picos de ventas en fechas clave → planificar promociones, asegurar stock, optimizar campañas de marketing.

## Cómo replicarlo
1. Descargar los datasets (`ventas.csv`, `clientes.csv`, `productos.csv`).  
2. Abrir **Power BI Desktop**.  
3. Importar los datasets y crear relaciones:  
   - `Ventas` → `Clientes` (cliente_id)  
   - `Ventas` → `Productos` (producto_id)    
4. Crear las medidas DAX para los KPIs:  
   - Ventas Totales: `SUM(Ventas[total_venta])`  
   - Ticket Promedio: `AVERAGE(Ventas[total_venta])`  
   - Clientes: `DISTINCTCOUNT(Ventas[cliente_id])`  
5. Crear gráficos y dashboards siguiendo la jerarquía:  
   - Arriba → KPIs  
   - Centro → Tendencias  
   - Abajo → Detalle  
6. Interpretar insights y tomar decisiones estratégicas según los hallazgos.


## Herramientas utilizadas
- **Power BI Desktop**  
- **Python (pandas, matplotlib, seaborn)** para análisis previo opcional  
- **Excel / CSV** como datasets de entrada


