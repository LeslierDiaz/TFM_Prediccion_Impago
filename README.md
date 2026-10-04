# Predicción de impago en tarjetas de crédito mediante Machine Learning

Este repositorio contiene el notebook desarrollado para el Trabajo de Fin de Máster del Máster Universitario en Big Data y Ciencia de Datos de la Universidad Internacional de Valencia (VIU).

**Autora:** Leslier Gabriela Díaz López  
**Año:** 2026

## Objetivo del proyecto

Comparar el desempeño de K-NN, Random Forest y XGBoost en la predicción del incumplimiento de pago de tarjetas de crédito, utilizando un conjunto de datos público y un procedimiento reproducible de preparación, entrenamiento, evaluación e interpretación.

## Conjunto de datos

Se utilizó **Default of Credit Card Clients**, disponible en el repositorio UCI Machine Learning Repository.

El conjunto contiene 30.000 registros de clientes de Taiwán y 23 variables predictoras relacionadas con características sociodemográficas, límites de crédito, estados de pago, importes facturados y pagos realizados.

Los registros describen el comportamiento financiero entre abril y septiembre de 2005. La variable objetivo indica el incumplimiento de pago en el mes siguiente.

**Fuente de los datos:** https://doi.org/10.24432/C55S3H

## Metodología

El proyecto siguió la metodología CRISP-DM y comprendió:

1. Comprensión del problema y de los datos.
2. Limpieza y validación del conjunto de datos.
3. Análisis exploratorio.
4. Creación de variables y preprocesamiento.
5. Entrenamiento y ajuste de K-NN, Random Forest y XGBoost.
6. Evaluación comparativa e interpretación de resultados.

Se utilizó una división estratificada de los datos: 80 % para entrenamiento y 20 % para prueba. Los hiperparámetros y los umbrales de clasificación se ajustaron con los datos de entrenamiento.

El criterio de selección del modelo fue el ROC-AUC medio de validación cruzada. La evaluación también consideró PR-AUC, precisión, exhaustividad, F1, exactitud, exactitud balanceada, puntuación de Brier y matrices de confusión. La interpretación del modelo seleccionado se realizó mediante SHAP.

## Contenido del repositorio

- **Notebook `.ipynb`:** código del proyecto, explicaciones, gráficos y resultados guardados.
- **README.md:** descripción del estudio e instrucciones de uso.

## Cómo ejecutar el notebook

El notebook puede consultarse en GitHub y ejecutarse en Google Colab:

[Abrir el notebook en Google Colab](https://colab.research.google.com/drive/1miHfY4A2UTwwAmAM5lqP-lL7t6J5PLbl?usp=sharing)

Para ejecutarlo:

1. Abre el enlace de Google Colab.
2. Guarda una copia en tu Google Drive si deseas modificarlo.
3. Revisa las instrucciones y las celdas iniciales de instalación y carga de datos.
4. Ejecuta las celdas en orden, desde el inicio hasta el final.

El entrenamiento y la búsqueda de hiperparámetros pueden requerir un tiempo considerable, dependiendo de los recursos disponibles.

## Alcance y limitaciones

Este proyecto tiene una finalidad académica. Los resultados corresponden al conjunto de datos utilizado y no constituyen una validación para clientes ecuatorianos ni una herramienta lista para tomar decisiones crediticias reales.

Su aplicación en otro contexto requeriría datos representativos, validación adicional y revisión de aspectos como sesgos, privacidad y costos de los errores de clasificación.

## Referencia del conjunto de datos

Yeh, I.-C. (2009). *Default of credit card clients* [Conjunto de datos]. UCI Machine Learning Repository. https://doi.org/10.24432/C55S3H
