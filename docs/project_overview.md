# Project Overview

## Proyecto 001 | Predicción de la Calidad del Espumado mediante Machine Learning

Este proyecto de Ciencia de Datos busca optimizar el proceso de embotellado de bebidas carbonatadas mediante un modelo predictivo que estime el nivel de espumado durante el llenado.

## Objetivo

Predecir el nivel de espumado a partir de variables operativas del proceso productivo para reducir pérdidas, mejorar la eficiencia y apoyar decisiones de producción.

## Problema de negocio

El espumado excesivo durante el embotellado provoca:

- Disminución de la velocidad de producción.
- Aumento del desperdicio de producto.
- Incremento de los costos operativos.
- Reducción de la rentabilidad.

Un modelo predictivo puede ayudar a anticipar el espumado y a ajustar el proceso antes de que se generen pérdidas.

## Dataset

El conjunto de datos contiene variables del proceso de carbonatación y llenado, entre las que se incluyen:

- O₂ ingreso carbonatador
- Set Factor CO₂
- Volumen CO₂
- Temperatura del carbonatador
- Temperatura de la botella
- Presión de bomba
- Tipo de producto (Sin Azúcar)

### Variable objetivo

- Nivel de espumado

## Metodología

El proyecto sigue una metodología inspirada en CRISP-DM:

1. Comprensión del problema de negocio.
2. Comprensión del conjunto de datos.
3. Preparación y limpieza de datos.
4. Análisis exploratorio de datos (EDA).
5. Ingeniería de características.
6. Entrenamiento y validación de modelos.
7. Optimización con GridSearchCV.
8. Evaluación.
9. Estimación del impacto en el negocio.

## Modelos evaluados

Se entrenaron y compararon varios algoritmos de clasificación, entre ellos:

- K-Nearest Neighbors (KNN)
- Decision Tree
- Support Vector Machine (SVM)
- Gaussian Naive Bayes

## Métricas de evaluación

Los modelos se comparan con métricas estándar de clasificación:

- Accuracy
- Precision
- Recall
- F1-Score
- Matriz de confusión
- Classification report

## Impacto esperado

El proyecto también incluye una estimación del beneficio económico potencial derivado de la implementación del modelo, evaluando:

- Incremento de producción.
- Reducción del desperdicio.
- Comparación de costos.
- Beneficios operativos.

## Estructura del proyecto

- `data/`
  - `raw/`
  - `processed/`
  - `external/`
- `notebooks/`
- `src/`
- `models/`
- `reports/`
  - `executive/`
  - `figures/`
- `dashboards/`
- `docs/`

## Cómo usar este proyecto

1. Clonar el repositorio.
2. Instalar dependencias con `pip install -r requirements.txt`.
3. Abrir el notebook en `notebooks/Proyecto_Final_Espumado.ipynb`.

---

Este archivo ofrece una visión general del proyecto y su enfoque principal para la predicción de la calidad del espumado.
