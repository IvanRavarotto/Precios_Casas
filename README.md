# Predicción de Precios de Casas (Supervisado - Regresión)

## Descripción del Proyecto

Este proyecto tiene como objetivo desarrollar un modelo de Machine Learning supervisado de regresión para predecir el precio de casas basándose en sus características principales. Se utiliza un conjunto de datos que incluye variables como `metros_cuadrados`, `habitaciones`, `banos`, `antiguedad` y `ubicacion`.

## Metodología

1.  **Carga y Preparación de Datos**: Se carga el conjunto de datos de precios de casas. Se realiza un preprocesamiento de las características, incluyendo la codificación one-hot para la variable categórica `ubicacion`.
2.  **División de Datos**: El conjunto de datos se divide en conjuntos de entrenamiento y prueba para evaluar el rendimiento del modelo.
3.  **Entrenamiento del Modelo**: Se emplea un `GradientBoostingRegressor` de `sklearn` para entrenar el modelo predictivo.
4.  **Evaluación del Modelo**: El rendimiento del modelo se mide utilizando el coeficiente de determinación (R-squared) en el conjunto de prueba. El modelo alcanzó un R-squared de 99.51%, lo que indica una alta precisión en las predicciones.
5.  **Predicción de Nuevas Casas**: Se implementa una funcionalidad para predecir el precio de una 'casa nueva' con características definidas por el usuario, demostrando la aplicabilidad práctica del modelo.

## Resultados

El modelo `GradientBoostingRegressor` ha demostrado una gran efectividad en la predicción de precios de casas, con un R-squared superior al 99%. Esto sugiere que el modelo es robusto y confiable para la estimación de valores de propiedades.

## Cómo usar

Para replicar y experimentar con este proyecto, siga los pasos:

1.  Asegúrese de tener todas las librerías necesarias instaladas (pandas, scikit-learn, matplotlib, seaborn).
2.  Ejecute las celdas del notebook en orden para cargar los datos, entrenar el modelo y realizar predicciones.
3.  Modifique los parámetros en la celda de `casaNueva` para predecir el precio de una casa con características diferentes.
