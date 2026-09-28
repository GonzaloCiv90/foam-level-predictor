# Models

Este directorio contiene los archivos de modelos entrenados y los metadatos del proyecto de predicción del nivel de espumado.

## Archivos incluidos

- `best_model.pkl` — Modelo seleccionado como el mejor para la predicción del nivel de espumado.
- `decision_tree.pkl` — Modelo Decision Tree entrenado.
- `grid_decision_tree.pkl` — Resultado de GridSearchCV para Decision Tree.
- `grid_knn.pkl` — Resultado de GridSearchCV para K-Nearest Neighbors.
- `grid_naive_bayes.pkl` — Resultado de GridSearchCV para Gaussian Naive Bayes.
- `grid_svm.pkl` — Resultado de GridSearchCV para Support Vector Machine.
- `knn.pkl` — Modelo K-Nearest Neighbors entrenado.
- `naive_bayes.pkl` — Modelo Gaussian Naive Bayes entrenado.
- `svm.pkl` — Modelo Support Vector Machine entrenado.
- `feature_names.json` — Lista de características utilizadas por el modelo seleccionado.
- `model_metadata.json` — Metadatos del experimento y resultados de la optimización.

## Metadatos principales

- Proyecto: Foam Quality Prediction
- Autor: Gonzalo Civita
- Variable objetivo: Nivel de espumado
- Optimización: GridSearchCV
- Validación cruzada: 5 pliegues
- Modelo seleccionado: Decision Tree

## Características usadas en el modelo final

- O2 ing carbo
- Set factor CO2
- Volumen CO2
- Temp botella
- Temp Carbo
- Sin Azucar

## Resumen de resultados de GridSearchCV

- KNN: `n_neighbors=7`, `weights=distance`, mejor score 0.89846
- Decision Tree: `max_depth=20`, `min_samples_split=2`, mejor score 0.89877
- SVM: `C=10`, `kernel=linear`, mejor score 0.85908
- Naive Bayes: `var_smoothing=1e-07`, mejor score 0.72646

## Uso

Carga el modelo en Python con `joblib.load` o `pickle.load` y aplica el preprocesamiento correspondiente a las características listadas en `feature_names.json`.

> Nota: Asegúrate de utilizar el mismo orden y las mismas transformaciones de las características que se emplearon durante el entrenamiento.
