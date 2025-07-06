# 🏡 Análisis de Datos Airbnb: Tipos de Propiedad y Precios

Este proyecto aplica un flujo de trabajo completo de análisis de datos sobre una base de alojamientos de Airbnb, utilizando Python y pandas. A partir de un dataset sin procesar, se limpiaron los datos, se analizaron tendencias por tipo de propiedad, y se exportó un dataset depurado para análisis posteriores.

---

## 🎯 Objetivo

Transformar y analizar una base de datos de Airbnb para obtener insights clave sobre precios por tipo de alojamiento, presencia de valores nulos y distribución de categorías.

---

## 🛠️ Herramientas utilizadas

- **Python**  
- **pandas** para limpieza y transformación de datos  
- **Jupyter Notebook** para desarrollo interactivo  
- Dataset original en formato `.csv` (sample_airbnb.listingsAndReviews) exprotado desde Mongo DB : https://cloud.mongodb.com/v2/67e2c94e43ddf247bebedd12#/metrics/replicaSet/686863db4248094273395418/explorer/sample_airbnb/listingsAndReviews/find.

---

## 📊 Descripción del análisis o solución

- **Extracción**: Carga de un archivo `.csv` con más de 5.000 alojamientos.
- **Transformación**:
  - Identificación y eliminación de registros con valores nulos en las columnas `price` y `review_scores.review_scores_rating`.
  - Conversión a DataFrame y análisis de estructura.
- **Análisis**:
  - Cálculo del precio promedio por `property_type`.
  - Identificación de los 5 tipos de propiedad más comunes.
- **Exportación**:
  - Guardado del DataFrame limpio en un nuevo archivo: `airbnb_cleaned.csv`.

---

## 📈 Resultados o hallazgos

- Se eliminaron **1.474 filas** con valores nulos, quedando un total de **4.081 registros limpios**.
- El **precio promedio** por noche varía ampliamente entre propiedades: desde alojamientos básicos como *Campsite* (USD 25) hasta opciones premium como *Houseboat* (USD 2.999).
- El tipo de propiedad más común es el **Apartment**, con **2.681 registros**.
- Se logró una base más precisa para análisis futuros y visualizaciones.

---

## 🧠 Aprendizajes clave

- Limpieza de datos real aplicando filtros con pandas.
- Agrupaciones eficientes con `groupby()` para obtener métricas por categoría.
- Buenas prácticas de exportación y documentación del proceso de transformación.
- Refuerzo del enfoque **ETL** (Extract, Transform, Load) en un caso real.

---

## 📎 Recursos adicionales

> Gráfico de barras "Top 5 tipos de propiedades más comunes en Airbnb". 

![Top 5 propiedades más comunes de Airbnb](https://github.com/user-attachments/assets/3340b0c0-41b0-4ac9-82d2-1b97891536bb)


## El script principal se encuentra en https://github.com/Fabiloz/Procesamiento-ETL-con-Pandas-y-MongoDB-Atlas-Airbnb-/blob/master/etl_airbnb.ipynb

---

## 👤 Autora

**Fabiola Lozano**  
Ingeniera Industrial | Analista de Datos | Optimización

💼 https://www.linkedin.com/in/fabiolalozano

📧 flozano0515@gmail.com

🔗 https://github.com/Fabiloz
