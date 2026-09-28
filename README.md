````markdown
# 🍺 Proyecto 001 | Predicción de la Calidad del Espumado mediante Machine Learning

> Proyecto de Ciencia de Datos orientado a optimizar el proceso de embotellado de bebidas carbonatadas mediante modelos de clasificación y análisis del impacto económico.

---

# 📌 Resumen

En la industria de bebidas carbonatadas, el exceso de espumado durante el proceso de llenado provoca pérdidas de producto, disminución de la velocidad de producción y aumento de los costos operativos.

Este proyecto desarrolla un modelo de **Machine Learning** capaz de predecir el nivel de espumado utilizando variables del proceso productivo. Además, se realiza una estimación del impacto potencial que tendría la implementación del modelo sobre indicadores clave del negocio (KPIs).

---

# 🎯 Objetivos

- Comprender el problema de negocio.
- Analizar y preparar los datos históricos del proceso.
- Identificar las variables con mayor influencia sobre el nivel de espumado.
- Entrenar y optimizar diferentes algoritmos de clasificación.
- Comparar el desempeño de los modelos mediante métricas de evaluación.
- Estimar el beneficio económico potencial derivado de la implementación del modelo.

---

# 🏭 Problema de negocio

El espumado excesivo durante el embotellado genera:

- Disminución de la velocidad de producción.
- Incremento del desperdicio de producto.
- Aumento de los costos operativos.
- Reducción de la rentabilidad.

El objetivo del proyecto es demostrar cómo un modelo predictivo puede apoyar la toma de decisiones para mejorar la eficiencia del proceso.

---

# 📊 Dataset

El conjunto de datos contiene variables operativas relacionadas con el proceso de carbonatación y llenado.

### Variables utilizadas

- O₂ ingreso carbonatador
- Set Factor CO₂
- Volumen CO₂
- Temperatura del carbonatador
- Temperatura de la botella
- Presión de bomba
- Tipo de producto (Sin Azúcar)

**Variable objetivo**

- Nivel de espumado

---

# 🛠 Tecnologías utilizadas

- Python
- Pandas
- NumPy
- Plotly
- Matplotlib
- Scikit-Learn
- Joblib
- Google Colab

---

# 📚 Metodología

El proyecto sigue una metodología inspirada en **CRISP-DM**.

1. Comprensión del problema de negocio.
2. Comprensión del conjunto de datos.
3. Preparación de los datos.
4. Análisis Exploratorio de Datos (EDA).
5. Ingeniería de características.
6. Entrenamiento de modelos.
7. Optimización mediante GridSearchCV.
8. Evaluación.
9. Impacto para el negocio.

---

# 🤖 Modelos evaluados

Se entrenaron y optimizaron cuatro algoritmos de clasificación utilizando **GridSearchCV** con validación cruzada de cinco particiones.

| Modelo | Optimización |
|---------|--------------|
| K-Nearest Neighbors (KNN) | ✅ GridSearchCV |
| Decision Tree | ✅ GridSearchCV |
| Support Vector Machine (SVM) | ✅ GridSearchCV |
| Gaussian Naive Bayes | ✅ GridSearchCV |

---

# 📈 Evaluación

Los modelos fueron comparados utilizando las siguientes métricas:

- Accuracy
- Precision
- Recall
- F1-Score
- Matriz de Confusión
- Classification Report
- Beneficio económico estimado

---

# 📊 Principales hallazgos

El análisis exploratorio permitió identificar que las variables con mayor influencia sobre el nivel de espumado fueron:

- Temperatura del carbonatador
- Temperatura de la botella
- Volumen de CO₂
- O₂ de ingreso al carbonatador
- Set Factor CO₂
- Tipo de producto

Estas variables representan los principales factores que afectan el comportamiento del proceso de llenado.

---

# 💰 Impacto para el negocio

Además del desempeño predictivo de los modelos, se desarrolló una simulación financiera para estimar el beneficio potencial de implementar una herramienta de apoyo basada en Machine Learning.

Se analizaron indicadores como:

- Incremento de la producción.
- Reducción del desperdicio.
- Comparación de costos.
- Beneficio económico esperado.
- KPIs operativos.

> Los resultados económicos corresponden a un escenario de simulación basado en supuestos operativos y tienen fines ilustrativos.

---

# 📁 Estructura del proyecto

```text
project-001-foam-quality-prediction/
│
├── data/
│   ├── raw/
│   ├── processed/
│   └── external/
│
├── notebooks/
│   └── 01_foam_quality_prediction.ipynb
│
├── src/
├── models/
├── reports/
│   ├── executive/
│   └── figures/
│
├── dashboards/
├── docs/
├── tests/
│
├── README.md
├── requirements.txt
├── environment.yml
├── LICENSE
└── CHANGELOG.md
```

---

# 🚀 Cómo ejecutar el proyecto

1. Clonar el repositorio.

```bash
git clone https://github.com/tu-usuario/project-001-foam-quality-prediction.git
```

2. Instalar las dependencias.

```bash
pip install -r requirements.txt
```

3. Abrir el notebook:

```text
notebooks/01_foam_quality_prediction.ipynb
```

---

# 📷 Contenido del notebook

El notebook incluye:

- Comprensión del negocio.
- Análisis Exploratorio de Datos (EDA).
- Ingeniería de características.
- Optimización de hiperparámetros.
- Comparación de modelos.
- Matrices de confusión.
- Importancia de variables.
- Dashboard de KPIs.
- Simulación del impacto económico.

---

# 🔮 Próximos pasos

- Incorporar nuevos registros históricos.
- Validar el modelo con datos de producción en tiempo real.
- Desarrollar una API para realizar predicciones.
- Implementar un dashboard interactivo para monitoreo continuo.
- Automatizar el proceso de reentrenamiento del modelo.

---

# 👨‍💻 Autor

**Gonzalo Civita**

Proyecto desarrollado como parte de un portafolio profesional de Ciencia de Datos enfocado en aplicaciones de Machine Learning para procesos industriales.

---

# 📄 Licencia

Este proyecto se distribuye bajo la licencia MIT.
````
