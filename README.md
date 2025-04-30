# Análisis de Desempeño de Tiendas para Identificar Oportunidad de Nueva Apertura

## Propósito del Análisis

El objetivo principal de este proyecto es evaluar el desempeño comercial y operativo de cuatro tiendas existentes utilizando un conjunto de datos de ventas detallado. El análisis busca comprender las fortalezas y debilidades de cada ubicación actual en términos de facturación, popularidad de productos y categorías, satisfacción del cliente y costos logísticos (envío). La finalidad es utilizar estos insights para fundamentar la decisión estratégica sobre la ubicación más prometedora y potencialmente más rentable para establecer un nuevo negocio.

## Estructura del Proyecto y Organización de Archivos

El proyecto se basa en el repositorio clonado de GitHub `alura-es-cursos/challenge1-data-science-latam`. La estructura de archivos relevante es la siguiente:
/challenge1-data-science-latam/
├── base-de-datos-challenge1-latam/
│   ├── tienda_1.csv
│   ├── tienda_2.csv
│   ├── tienda_3.csv
│   ├── tienda_4.csv
└── Analisis_Tiendas.ipynb  # O el nombre de tu notebook de Colab
└── README.md           # Este archivo

* `base-de-datos-challenge1-latam/`: Esta carpeta contiene los archivos CSV con los datos de ventas de cada una de las cuatro tiendas.
* `tienda_X.csv`: Archivo CSV con los datos de ventas de cada tienda (donde X es 1, 2, 3 o 4).
* `Analisis_Tiendas.ipynb`: El notebook de Jupyter (o Colab) que contiene el código Python para cargar, limpiar, analizar y visualizar los datos. (Asegúrate de reemplazar `Analisis_Tiendas.ipynb` por el nombre real de tu archivo si es diferente).
* `README.md`: Este archivo, que describe el proyecto.

## Análisis Realizado e Insights Obtenidos

El análisis se llevó a cabo en un notebook de Python utilizando la librería `pandas`. Los pasos incluyeron la carga y combinación de los datos de las cuatro tiendas, exploración inicial de la estructura de los datos y el cálculo de métricas clave por tienda.

Las métricas analizadas fueron:

1.  **Facturación Total por Tienda:** Suma de los precios de venta por cada tienda.
2.  **Volumen Total de Transacciones por Tienda:** Conteo del número de ventas por cada tienda (proxy de popularidad/actividad).
3.  **Categorías más Populares:** Identificación de las categorías de producto con mayor volumen de ventas (a nivel general y por tienda).
4.  **Productos más y menos Vendidos:** Identificación de los productos con mayor y menor volumen de ventas (a nivel general y por tienda/categoría).
5.  **Promedio de Calificación de Clientes por Tienda:** Cálculo de la calificación promedio recibida por cada tienda.
6.  **Costo Promedio de Envío por Tienda:** Cálculo del costo promedio de envío asociado a las ventas de cada tienda.
7.  **Facturación Promedio por Venta por Categoría y Tienda:** Análisis del precio promedio por artículo vendido dentro de cada categoría en cada tienda.

**Insights Clave:**

Se realizó un ranking comparativo de las tiendas basado en las métricas calculadas. Los hallazgos principales incluyen:

* La **Tienda 1** lidera en **Facturación Total**, pero presenta la menor **Calificación Promedio** y el mayor **Costo Promedio de Envío**.
* Las **Tiendas 1, 2 y 3** tienen un **Volumen de Transacciones** muy similar y significativamente mayor que la Tienda 4.
* La **Tienda 3** tiene la **mayor Calificación Promedio** de clientes y un buen ranking en **Costo Promedio de Envío**, a pesar de no ser la número uno en facturación bruta.
* La **Tienda 4** tiene el menor **Costo Promedio de Envío** pero el menor volumen de actividad (Facturación y Transacciones).

El análisis sugiere que la **Tienda 3** podría representar un mercado interesante para una nueva apertura, dada su alta satisfacción del cliente y eficiencia logística, lo cual son factores importantes para la rentabilidad a largo plazo.

## Cómo Ejecutar el Notebook

Este proyecto se puede ejecutar fácilmente en Google Colab (o cualquier entorno compatible con Jupyter Notebooks).

1.  Abre Google Colab en tu navegador web.
2.  Haz clic en "Archivo" -> "Subir notebook" y selecciona el archivo `Analisis_Tiendas.ipynb` desde tu máquina local.
3.  Una vez abierto el notebook en Colab, asegúrate de que el entorno de ejecución esté configurado correctamente (Runtime -> Change runtime type -> Python 3).
4.  Ejecuta cada celda del notebook secuencialmente (puedes usar Shift + Enter o el botón de "Ejecutar celda"). El notebook incluye los pasos para cargar los datos directamente desde el repositorio de GitHub, realizar los cálculos y mostrar los resultados.

## Requisitos

El análisis utiliza principalmente la librería `pandas` de Python, que está preinstalada en Google Colab.

## Datos

Los datos utilizados en este análisis provienen del repositorio de GitHub `https://github.com/alura-es-cursos/challenge1-data-science-latam.git`. Consisten en registros de ventas detallados de cuatro tiendas, incluyendo información sobre producto, precio, envío, fecha, ubicación, calificación, método de pago y coordenadas geográficas.

## Autor

Borja Félix Rojas
