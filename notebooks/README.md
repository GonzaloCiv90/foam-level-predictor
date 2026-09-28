# Notebooks

## Descripción

En este directorio se encuentran las notebooks que contienen el código de los modelos de Machine Learning desarrollados
en el proyecto, así como notebooks que ilustran métodos y configuraciones usados para entrenar, evaluar y guardar los
modelos.

## Contenido

- Código para entrenamiento y evaluación de modelos de clasificación/regresión.
- Preprocesamiento de datos y extracción de características.
- Scripts y celdas que muestran cómo guardar y cargar modelos, y reproducer experimentos.

## Formatos y entornos

Las notebooks están preparadas tanto para Jupyter Notebook/JupyterLab como para Google Colab. Algunas celdas incluyen
comentarios o instrucciones específicas para ejecutar en Colab (por ejemplo, montaje de Google Drive o instalación de
dependencias en tiempo de ejecución).

## Requisitos

Instalar las dependencias necesarias en el entorno de ejecución (ejemplo mínimo):

```
pip install -r requirements.txt
```

Si no existe un `requirements.txt`, las dependencias comunes incluyen: `pandas`, `numpy`, `scikit-learn`, `joblib`,
`matplotlib`, `seaborn` y `plotly`.

## Cómo usar

- Para ejecutar localmente: abrir la notebook en Jupyter Notebook/JupyterLab y ejecutar las celdas en orden.
- Para ejecutar en Colab: subir la notebook a Colab o abrirla desde Google Drive; seguir las instrucciones en la primera
  celda para instalar dependencias o montar Drive si es necesario.

## Buenas prácticas

- Revisar la primera celdas de cada notebook donde suelen indicarse requisitos o rutas de datos.
- Ejecutar celdas de preprocesamiento antes de correr las celdas de entrenamiento.

## Contacto

Para dudas sobre las notebooks o reproducibilidad, revisar el archivo principal del proyecto o contactar al autor del
repositorio.
