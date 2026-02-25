# 📊 Análisis de Rendimiento Estratégico: AluraStore Latam

## 📝 Descripción del Proyecto
Este proyecto contiene un Análisis Exploratorio de Datos aplicado a la red de sucursales del Sr. Juan. A través del procesamiento de cuatro bases de datos independientes (correspondientes a 4 tiendas distintas), se evaluó el desempeño comercial y logístico de cada sucursal. 

El objetivo final del análisis es proporcionar una recomendación estratégica respaldada por datos para la gerencia (Sr. Juan) sobre **qué sucursal debería ser liquidada o vendida** para maximizar la rentabilidad global del negocio.

## 🛠️ Tecnologías Utilizadas
* **Lenguaje:** Python 3
* **Entorno:** Jupyter Notebook / Google Colab
* **Librerías principales:**
  * `pandas`: Para la manipulación, limpieza y agregación de datos.
  * `matplotlib.pyplot`: Para la creación de visualizaciones estáticas (gráficos de barras, horizontales).

## 📂 Estructura de los Datos
El proyecto consume 4 archivos `.csv` (`tienda_1.csv`, `tienda_2.csv`, `tienda_3.csv`, `tienda_4.csv`). Cada dataset contiene el registro histórico de ventas con las siguientes variables principales:
* `Producto` y `Categoría del Producto`
* `Precio` y `Costo de envío`
* `Fecha de Compra`, `Vendedor` y `Lugar de Compra`
* `Calificación` (Satisfacción del cliente 1-5)
* `Método de pago` y `Cantidad de cuotas`
* `lat` y `lon` (Coordenadas geográficas)

## 📈 Análisis y Visualizaciones Realizadas
Durante el desarrollo del Notebook, se respondieron las siguientes preguntas de negocio creando funciones personalizadas y gráficos comparativos:
1. **Análisis de Facturación:** Cálculo de los ingresos totales (Precio + Costo de envío) por tienda.
2. **Distribución por Categorías:** Conteo de volumen de productos vendidos agrupados por categoría.
3. **Satisfacción del Cliente:** Análisis de la calificación promedio histórica de cada sucursal.
4. **Productos Top & Bottom:** Identificación dinámica de los productos con mayores y menores ventas absolutas utilizando funciones de máximos y mínimos.
5. **Costos Logísticos:** Cálculo del costo de envío promedio asumido por sucursal.

## 💡 Conclusión Principal
Tras el cruce de métricas, el análisis determinó que la **Tienda 4 es la candidata ideal para ser vendida**. A pesar de contar con el costo logístico (envío) más bajo de la red, es la sucursal que genera la **menor cantidad de ingresos totales**. Se recomienda conservar la Tienda 1 (motor financiero principal a pesar de sus altos costos logísticos) y la Tienda 3 (líder en satisfacción del cliente).

## 🚀 Cómo ejecutar este proyecto
1. Clona este repositorio: `git clone [URL_DE_TU_REPOSITORIO]`
2. Asegúrate de tener instalado Python y las librerías requeridas (`pip install pandas matplotlib`).
3. Abre el archivo `AluraStoreLatam.ipynb` en tu entorno preferido (Jupyter o Colab).
4. Ejecuta las celdas en orden secuencial. *Nota: Asegúrate de que las rutas a los archivos `.csv` apunten correctamente a tu directorio local o al repositorio en la nube.*