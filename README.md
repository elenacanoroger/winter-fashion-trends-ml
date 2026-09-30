# Predicción de tendencias de moda mediante Machine Learning

Proyecto de Data Science y Machine Learning aplicado al sector de la moda. El objetivo es analizar diferentes características de productos de moda de invierno y desarrollar un modelo capaz de predecir su estado de tendencia.

El proyecto se ha realizado utilizando herramientas de AWS como Amazon S3, SageMaker Data Wrangler y SageMaker Canvas.

## Objetivo

El objetivo principal del proyecto es desarrollar un modelo de clasificación capaz de predecir la variable `Trend_Status`, diferenciando entre cuatro posibles categorías:

- Outdated
- Emerging
- Trending
- Classic

Además del entrenamiento del modelo, se realiza un análisis previo de los datos para conocer su calidad, estudiar las variables disponibles y detectar posibles problemas antes del modelado.

##  Dataset

Para realizar el proyecto utilicé el dataset **Winter Fashoin Trends**, disponible en Kaggle y publicado por Ayesha Sehrr.

El conjunto contiene **150 registros y 12 variables** relacionadas con diferentes características de productos de moda de invierno.

🔗 [Dataset utilizado en Kaggle](https://www.kaggle.com/datasets/ayeshaseherr/winter-fashoin-trends)

## Tecnologías utilizadas

- Amazon S3
- AWS SageMaker
- SageMaker Data Wrangler
- SageMaker Canvas
- Machine Learning
- Análisis exploratorio de datos (EDA)
- Feature Engineering

##  Proceso realizado

Durante el proyecto se realizaron las siguientes fases:

1. Importación y almacenamiento del dataset.
2. Análisis de calidad de los datos.
3. Análisis exploratorio de datos (EDA).
4. Análisis de correlaciones.
5. Comprobación de Target Leakage.
6. Análisis de posibles sesgos.
7. Ingeniería de características.
8. Preparación de variables categóricas.
9. Entrenamiento del modelo.
10. Evaluación e interpretación de los resultados.

##  Resultados del modelo

Los resultados obtenidos fueron:

- **Accuracy:** 35,48 %
- **F1:** 26,83 %
- **Precision:** 25,31 %
- **Recall:** 30 %

Las variables con mayor importancia para el modelo fueron **Popularity_Score (18,2 %)** y **Customer_Rating (13,2 %)**, seguidas de Material y Price (USD).

##  Interpretación de los resultados

La matriz de confusión permitió analizar con más detalle el comportamiento del modelo.

La categoría **Outdated** fue la que el modelo consiguió reconocer mejor, mientras que **Emerging** y **Trending** presentaron más confusiones. **Classic** también resultó difícil de identificar correctamente.

Los resultados están condicionados por el tamaño del dataset, ya que únicamente contiene 150 registros y el modelo debe diferenciar entre cuatro categorías.

## Posibles mejoras

Como continuación del proyecto sería interesante:

- Ampliar el número de registros del dataset.
- Conseguir una distribución más equilibrada entre las clases.
- Comparar diferentes algoritmos de Machine Learning.
- Realizar ajuste de hiperparámetros.
- Incorporar información de ventas, stock, descuentos y evolución de la demanda.

Estas mejoras permitirían comprobar si es posible obtener un modelo con mayor capacidad de generalización y más utilidad en un escenario real de retail.

##  Informe completo

En el informe completo se puede consultar todo el desarrollo del proyecto, incluyendo el análisis exploratorio, preparación de los datos, entrenamiento, métricas, matriz de confusión y conclusiones.

**Autora:** Elena Cano Rogero realizado por parte del programa profesional data science y inteligencia artificial realizado en la Universidad Internacional de La Rioja 2025/2026
