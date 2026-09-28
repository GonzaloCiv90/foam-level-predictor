# Metodología del Proyecto

Este documento describe el enfoque metodológico seguido en el proyecto de predicción de la calidad del espumado, basado en una adaptación de CRISP-DM a un contexto de análisis de datos industriales.

## 1. Comprensión del negocio

- Definir el problema: el espumado excesivo en el llenado de bebidas carbonatadas afecta la eficiencia, genera desperdicio y eleva costos operativos.
- Identificar objetivos: predecir el nivel de espumado antes del llenado para actuar sobre el proceso y disminuir pérdidas.
- Determinar stakeholders: equipo de producción, ingeniería de procesos, calidad y dirección operativa.

## 2. Comprensión de los datos

- Revisión inicial del dataset y estructura de los archivos disponibles.
- Exploración de variables: mediciones de proceso, condiciones de carbonatación, características del producto y la variable objetivo (`nivel de espumado`).
- Evaluación de la calidad de los datos: valores faltantes, duplicados, unidades, rangos anómalos y consistencia temporal.

## 3. Preparación de los datos

- Limpieza:
  - Eliminación o imputación de valores faltantes.
  - Corrección de formatos erróneos o inconsistentes.
  - Tratamiento de registros duplicados.

- Transformación:
  - Escalado o normalización de variables numéricas cuando sea necesario.
  - Codificación de variables categóricas (por ejemplo, tipo de producto).
  - Generación de nuevas características relevantes basadas en el conocimiento del proceso.

## 4. Análisis exploratorio de datos (EDA)

- Análisis univariado: distribución de cada variable y comportamiento de la variable objetivo.
- Análisis bivariado:
  - Correlaciones entre variables explicativas y el nivel de espumado.
  - Identificación de relaciones lineales o no lineales.
- Visualizaciones:
  - Histogramas, diagramas de caja, mapas de calor de correlación y gráficas de dispersión.

## 5. Ingeniería de características

- Selección de características relevantes para el modelado.
- Creación de nuevas variables derivadas del proceso, si aplicable.
- Reducción de dimensionalidad con un criterio orientado al dominio y la interpretabilidad.

## 6. Modelado

- División de los datos en conjuntos de entrenamiento y prueba.
- Prueba de diferentes algoritmos de clasificación adecuados para el problema.
- Modelos evaluados:
  - K-Nearest Neighbors (KNN)
  - Decision Tree
  - Support Vector Machine (SVM)
  - Gaussian Naive Bayes

## 7. Optimización y validación

- Ajuste de hiperparámetros con GridSearchCV.
- Validación cruzada para comprobar la robustez de los modelos.
- Selección final del modelo con mejor balance entre precisión y generalización.

## 8. Evaluación

- Métricas empleadas:
  - Accuracy
  - Precision
  - Recall
  - F1-score
  - Matriz de confusión
- Análisis de resultados y comparación entre modelos.
- Identificación de posibles sesgos y limitaciones.

## 9. Interpretación y comunicación

- Interpretación de la importancia de las variables.
- Comunicación de hallazgos clave a stakeholders técnicos y de negocio.
- Documentación de supuestos y conclusiones.

## 10. Estimación del impacto de negocio

- Evaluación del beneficio potencial al reducir el espumado excesivo.
- Estimación de ahorros en pérdida de producto y costos de operación.
- Propuesta de valor de la implementación del modelo en planta.

## 11. Recomendaciones futuras

- Recolectar nuevos datos para mejorar el alcance del modelo.
- Introducir métricas adicionales de calidad de llenado.
- Incorporar datos en tiempo real para apoyar decisiones de control del proceso.
- Evaluar el despliegue en un entorno productivo y el monitoreo continuo del desempeño.
