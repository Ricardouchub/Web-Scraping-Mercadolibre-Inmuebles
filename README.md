# Análisis del Mercado Inmobiliario en la comuna de Santiago 

<p align="left">
  <img src="https://img.shields.io/badge/Proyecto_Completado-%E2%9C%94-2ECC71?style=flat-square&logo=checkmarx&logoColor=white" alt="Proyecto Completado"/>
  <img src="https://img.shields.io/badge/Python-3.9%2B-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python"/>
  <img src="https://img.shields.io/badge/Scrapy-Web_Scraping-23A1D1?style=flat-square&logo=scrapy&logoColor=white" alt="Scrapy"/>
  <img src="https://img.shields.io/badge/BeautifulSoup-Parsing_HTML-8B4513?style=flat-square&logo=beautifulsoup&logoColor=white" alt="BeautifulSoup"/>
  <img src="https://img.shields.io/badge/Seaborn-Visualización-4C72B0?style=flat-square&logo=seaborn&logoColor=white" alt="Seaborn"/>
</p>

#### [Notebook Parte 1: Web Scrapping](https://github.com/Ricardouchub/Web-Scraping-Mercadolibre-Inmuebles/blob/main/Parte%201%20-%20Web%20scraping%20Mercadolibre%20Inmuebles.ipynb)
#### [Notebook Parte 2: Analisis](https://github.com/Ricardouchub/Web-Scraping-Mercadolibre-Inmuebles/blob/main/Parte%202%20-%20Limpieza%20y%20Analisis%20Exploratorio%20de%20Datos%20(EDA).ipynb)

Este es un proyecto enfocado en demostrar el ciclo de vida completo de un proyecto de datos: desde la extracción (Web Scraping) y limpieza, hasta el análisis exploratorio (EDA) y la visualización de hallazgos.

Se analiza una pequeña parte del mercado de venta de departamentos en la coimuna de Santiago de la última semana de julio utilizando datos de Mercado Libre para identificar patrones y factores clave que influyen en los precios. **Es importante destacar que este es un ejercicio para demostrar habilidades técnicas y no constituye un estudio de mercado inmobiliario exhaustivo ni profundo.**

El objetivo principal es transformar datos brutos y no estructurados obtenidos de titulares de anuncios en insights claros y visualizaciones que permitan entender los factores clave (sin tener en cuenta la localización, ni antigüedad, ni materiales de construccion, etc) que influyen en los precios y caracterizar la oferta actual del mercado.

---
##  Objetivo 

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
    * Se recorrieron las 42 páginas de resultados para obtener una muestra completa. (con mas de 2000 anuncios)
    * Se aplicó una técnica de "extracción bruta" con **BeautifulSoup** para capturar todo el texto de cada anuncio, asegurando la recolección de datos a pesar de las variaciones en la estructura HTML.
    * El resultado es un archivo CSV con los datos en crudo.

2.  **Parte 2: Limpieza y Análisis Exploratorio (EDA)**
    * Se utilizó la librería **Pandas** para la limpieza y estructuración de los datos.
    * Se aplicaron **Expresiones Regulares (Regex)** para extraer y transformar el texto en bruto en columnas limpias y tipadas (`Precio`, `Dormitorios`, `Superficie_m2`, etc.).
    * Se manejaron los valores nulos y atípicos para asegurar la calidad del conjunto de datos.
    * Se generaron visualizaciones con **Matplotlib** y **Seaborn** para responder las preguntas clave y comunicar los hallazgos.

---
## Herramientas

* **Lenguaje Python**
* **Librerías Principales:**
    * **Extracción:** Selenium, BeautifulSoup4
    * **Análisis:** Pandas, NumPy
    * **Visualización:** Matplotlib, Seaborn

---
## Estructura del Repositorio

* `Parte 1 - Web scraping Mercadolibre Inmuebles.ipynb` Notebook con el código de extracción de datos.
* `Parte 2 - Limpieza y Analisis Exploratorio.ipynb` Notebook con el proceso de limpieza, análisis y visualización.
* `/data`: Carpeta que contiene los datasets generados.

---
## Visualizaciones preliminares
<img width="822" height="738" alt="image" src="https://github.com/user-attachments/assets/98924419-3cbb-42be-ae45-45ec77881646" />


<img width="704" height="432" alt="image" src="https://github.com/user-attachments/assets/f825ad24-014f-413a-9d27-d49ae6fa1436" />


<img width="602" height="434" alt="image" src="https://github.com/user-attachments/assets/cbfbb361-a126-416c-bbd0-ff0591327b3c" />


---
