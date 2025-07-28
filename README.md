# Análisis del Mercado Inmobiliario en la comuna de Santiago (Julio 2025)

Este proyecto presenta un análisis exploratorio de datos (EDA) sobre el mercado de venta de departamentos en la comuna de Santiago. Los datos fueron obtenidos mediante técnicas de web scraping del portal **Mercado Libre Inmuebles** durante el día 26 de julio de 2025.

El objetivo principal es transformar datos brutos y no estructurados obtenidos de titulares de anuncios en insights claros y visualizaciones que permitan entender los factores clave (sin tener en cuenta la localización, ni antigüedad, ni materiales de construccion, etc) que influyen en los precios y caracterizar la oferta actual del mercado.

---
##  Objetivo del Análisis

Identificar y cuantificar los factores que más influyen en el precio de venta de los departamentos en Santiago. A través de este análisis, se busca responder a las siguientes preguntas clave:

1.  **¿Cuál es la "fotografía" del mercado actual?** 
2.  **¿En qué rango de precios se concentra la mayor cantidad de propiedades?**
3.  **¿Qué características (superficie, dormitorios, baños) impulsan más el valor de una propiedad?**
4.  **¿Cuál es el valor promedio del metro cuadrado (UF/m²) y cómo se distribuye?**

---
##  Metodología

El proyecto está dividido en dos fases principales, cada una documentada en su propio Jupyter Notebook:

1.  **Parte 1: Web Scraping**
    * Se utilizó **Selenium** para controlar un navegador web y manejar el contenido dinámico del sitio, incluyendo un paso de intervención manual para resolver los pop-ups de ubicación.
    * Se recorrieron las 42 páginas de resultados para obtener una muestra completa.
    * Se aplicó una técnica de "extracción bruta" con **BeautifulSoup** para capturar todo el texto de cada anuncio, asegurando la recolección de datos a pesar de las variaciones en la estructura HTML.
    * El resultado es un archivo CSV con los datos en crudo.

2.  **Parte 2: Limpieza y Análisis Exploratorio (EDA)**
    * Se utilizó la librería **Pandas** para la limpieza y estructuración de los datos.
    * Se aplicaron **Expresiones Regulares (Regex)** para extraer y transformar el texto en bruto en columnas limpias y tipadas (`Precio`, `Dormitorios`, `Superficie_m2`, etc.).
    * Se manejaron los valores nulos y atípicos para asegurar la calidad del conjunto de datos.
    * Se generaron visualizaciones con **Matplotlib** y **Seaborn** para responder las preguntas clave y comunicar los hallazgos.

---
## Tecnologías Utilizadas

* **Python**
* **Librerías Principales:**
    * **Extracción:** Selenium, BeautifulSoup4
    * **Análisis:** Pandas, NumPy
    * **Visualización:** Matplotlib, Seaborn
* **Entorno:** Jupyter Notebook

---
## Estructura del Repositorio

* `Parte 1 - Web scraping Mercadolibre Inmuebles.ipynb` Notebook con el código de extracción de datos.
* `Parte 2 - Limpieza y Analisis Exploratorio.ipynb` Notebook con el proceso de limpieza, análisis y visualización.
* `/data`: Carpeta que contiene los datasets generados.

---
## 📊 Resultados y Visualizaciones Clave

<img width="704" height="432" alt="image" src="https://github.com/user-attachments/assets/f825ad24-014f-413a-9d27-d49ae6fa1436" />



<img width="602" height="434" alt="image" src="https://github.com/user-attachments/assets/cbfbb361-a126-416c-bbd0-ff0591327b3c" />


---
