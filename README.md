# **Aprendizaje automático - Predicción de Ingresos**

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) ![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white) ![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white) ![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white) ![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black) ![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white)

*Universidad de Antioquia - Facultad de INgeniería - Ingeniería de Sistemas*

> [!IMPORTANT]  
> Este es un proyecto con propósitos académicos para el curso de Modelos y Simulación de Sistemas II.

## **Integrantes**

- Daniel Lujan Agudelo
- Juan Pablo Arango Gaviria

## **API**
Se realizó la implementación de una API que entrena y sirve el mejor modelo para realizar predicciones con el modelo.

Repositorio: https://github.com/daniel-lujan/income-prediction-api

## **Descripción Notebooks**

Los notebooks se encuentran enumerados en el orden en el que deben ser ejecutados para reproducir los resultados:

1. **EDA:** Exploración inicial del conjunto de datos (columnas, tipos de datos, análisis multivariable, valores atípicos, datos faltantes, correlación)
2. **Preprocesamiento**: Tratamiento a columnas con datos faltantes, eliminación de columnas equivalentes, codificación de variables categóricas. El conjunto de datos con los tratamientos aplicados se exportaron en forma de binarios a las rutas `/preprocessed-data/basic/X-preprocessed.p` y `/preprocessed-data/basic/y-preprocessed.p`.
3. **Balance de clases**: Se aplicó submuestreo para balancear las clases. El conjunto de datos con las clases balanceadas se guardaron en forma de binarios en las rutas `/preprocessed-data/final/X-preprocessed.p` y `/preprocessed-data/final/y-preprocessed.p`.
4. **Entrenamiento de modelos**: Aplicación de 3 tipos de modelos: LogisticRegression, RandomForestClassifier y KMeans. Las predicciones de clase generadas por todos los modelos fueron guardadas como binarios en el directorio `model_results`.
5. **Red neuronal**: Se implementó una red neuronal. Se realizó una busqueda de mejor configuración de capas ocultas y se almacenaron de igual forma los resultados.
6. **Análisis de resultados**: Cálculo de métricas de evaluación y comparación entre los resultados de los modelos.
