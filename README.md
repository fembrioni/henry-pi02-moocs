# Este es el readme del proyecto integrador 2 de Henry

Alumno: Fernando Embrioni.

Junio de 2023.

Este proyecto requiere tres entregables.

- EDA sobre alguno de los datasets provistos en relacion con la industria de MOOCs (Massive Online Open Courses), incluyendo un wordcloud de los títulos.

- Análisis y consecuente Dashboard que permita a un nuevo incumbente ingresar a la industria de forma eficiente.

- Presentación del análisis y dashboard.

# Instalación

Clonar este repositorio en la ubicación que usted defina.

Encontrará la siguiente estructura de directorios:

- Raiz : Contiene este archivo que usted está leyendo y un archivo con las dependencias que deben ser instaladas. Para instalarlas, ejecute "pip install -r requirements.txt".

- ./data : Este directorio contiene los archivos de datos. Cabe destacar que los archivos no forman parte de esta distribución por lo que deben ser copiados aquí desde la siguiente url https://drive.google.com/drive/folders/1TS76ok6giW7D_l5vc-zu5-cBU_dH3P5H .

- ./code : Este directorio contiene los archivos de EDA y Dashboard. El EDA está realizado con Jupyter Notebook (Extensión ipynb) y el Análisis y Dashboard están realizados con Power BI (Extensión pbix).

# EDA

El EDA realizado sobre información de Udemy está autodocumentado. Sin embargo, cabe destacar lo siguiente:

- Se incluyen wordclouds para los títulos de los cursos gratuitos, como así también para los títulos de los cursos pagos.

- Se analizan correlaciones entre variables numéricas.

- Se analizan series de tiempo. P.Ej. Promedio de suscriptores por mes de publicación, y se obtienen conclusiones.

- Se detecta el idioma de cada curso con el fin de analizar esa dimensión.

# Dashboard y análisis

El análisis de Udemy y el dashboard para el nuevo incumbente se encuentran en el archivo "./code/Dashboard.pbix".

Para destacar:

- Se utlizó power query para procesar el dataset de Udemy y como uno de sus pasos, se incluye un script python que permite identificar el idioma de cada curso.

- Se provee un dashboard con cuatro KPIs.

# KPIs

## KPI 1 : Tasa de conversión a suscriptores pagos

- Medida : Cantidad de suscriptores a cursos pagos / Cantidad de suscriptores a cursos gratuitos.

- Periodo : Anual.

- Objetivo : Valor de la medida para el año anterior incrementado en 15%.

- Nota : Para una mejor visualización en el dashboard, se evita multiplicar por 100.

## KPI 2 : Precio promedio de cursos

- Medida : Suma del precio de los cursos pagos / Cantidad de cursos pagos.

- Periodo : Anual.

- Objetivo : Igualar o superar los $ 150.

## KPI 3 : Cursos pagos en Inglés

- Medida : Cantidad de cursos pagos en Inglés / Cantidad de cursos pagos.

- Periodo : Anual.

- Objetivo : Debe superar el 75%.

## KPI 4 : Promedio de reviews por curso pago cuyo precio supera los $ 150

- Medida : Cantidad de reviews de los cursos cuyo precio supera los usd 150  / Cantidad de cursos cuyo precio supera los usd 150.

- Periodo : Anual.

- Objetivo : Igualar o superar las 500 reviews en promedio por curso cuyo precio supera los $ 150.
