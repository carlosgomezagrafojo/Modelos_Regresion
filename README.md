# Modelos_Regresion
# 📈 Fundamentos de Modelado Predictivo: Modelos de Regresión

Este repositorio está dedicado al estudio, implementación y evaluación de algoritmos de **Regresión** utilizando el ecosistema científico de Python (`scikit-learn`, `pandas`, `numpy` y `matplotlib`). El objetivo central es dominar el pipeline de machine learning para variables continuas, abordando desde la regresión lineal simple hasta la regularización y el análisis polinomial.

## 📊 Datasets Utilizados & Casos de Estudio

Para consolidar la teoría, se han desarrollado experimentos prácticos con tres tipos de estructuras de datos:
1. **California Housing (Geográfico/Económico):** Predicción del valor medio de la vivienda basado en características socioeconómicas (20,640 registros).
2. **Diabetes Dataset (Clínico):** Modelado multivariable para predecir la progresión de la enfermedad basándose en factores biomédicos vectorizados.
3. **Simulación de Mercado Automotriz (Sintético):** Creación de un entorno controlado con variables como antigüedad, kilometraje y potencia para analizar la respuesta del modelo ante el ruido estadístico ($R^2 = 0.9426$).

## 🛠️ Pipeline de Aprendizaje Supervisado Implementado

El flujo de trabajo implementado en los cuadernos sigue los estándares de la industria:

*   **División de Datos (Holdout Validation):** Separación estricta en conjuntos de entrenamiento (`train`) y evaluación (`test`) mediante `train_test_split` para garantizar una validación libre de *data leakage* (filtración de datos).
*   **Ingeniería de Características Polinomiales:** Uso de `PolynomialFeatures` acoplado en un `make_pipeline` para capturar relaciones no lineales.
*   **Análisis de Overfitting vs Underfitting:** Evaluación sistemática del coeficiente de determinación ($R^2$) a través de múltiples grados polinomiales, identificando cómo a partir del Grado 15 el modelo degrada críticamente su capacidad de generalización.

## 📐 Métricas de Evaluación Rigurosa

Cada modelo se evalúa mediante un set multidimensional de métricas para entender el comportamiento del error:

*   **MAE (Error Absoluto Medio):** Medición de la magnitud media del error en las unidades de la variable objetivo.
*   **RMSE (Raíz del Error Cuadrático Medio):** Penalización de las desviaciones grandes; clave para entender el impacto de los errores atípicos.
*   **$R^2$ (Coeficiente de Determinación):** Proporción de la varianza explicada por el modelo (alcanzando más del 60% en regresión múltiple para datos inmobiliarios).

