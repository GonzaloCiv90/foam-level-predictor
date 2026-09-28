# Data Dictionary

Este documento describe las variables disponibles en el conjunto de datos procesados `data/processed/foam_quality_dataset_processed.csv`.

## Variables

### Fecha

- Tipo: Fecha
- Descripción: Fecha en la que se recogió el registro del proceso de llenado.

### Control

- Tipo: Entero o texto
- Descripción: Identificador de la unidad de control o del ciclo de producción dentro del día.

### Producto

- Tipo: Categórico
- Descripción: Código del producto o variante de bebida carbonatada procesada.

### O2 desaireador

- Tipo: Numérico (float)
- Descripción: Concentración de oxígeno medida en el desaireador.
- Unidad: generalmente en porcentaje o en ppm según la unidad de medición del proceso.

### O2 cwc

- Tipo: Numérico (float)
- Descripción: Concentración de oxígeno en el circuito CWC (probablemente relacionado con el tratamiento o conservación del agua/carbonatación).

### O2 ing carbo

- Tipo: Numérico (float)
- Descripción: Cantidad de oxígeno en el ingreso al carbonatador.

### Set factor CO2

- Tipo: Numérico (float)
- Descripción: Factor o valor de ajuste configurado para el CO2 durante el proceso de carbonatación.

### Volumen CO2

- Tipo: Numérico (float)
- Descripción: Volumen de dióxido de carbono aplicado o presente en el proceso.

### Temp botella

- Tipo: Numérico (float)
- Descripción: Temperatura de la botella antes o durante el llenado.
- Unidad: grados Celsius.

### Temp Carbo

- Tipo: Numérico (float)
- Descripción: Temperatura del carbonatador o del proceso de carbonatación.
- Unidad: grados Celsius.

### Pres bomba

- Tipo: Numérico (float)
- Descripción: Presión de la bomba en el circuito de llenado o carbonatación.
- Unidad: generalmente bar o kg/cm² según el contexto del proceso.

### Azucar

- Tipo: Binario/entero
- Descripción: Indicador de si el producto contiene azúcar.
- Valores posibles: 1 = Sí, 0 = No.

### JMAF

- Tipo: Binario/entero
- Descripción: Indicador de una variante de endulzante (Jarabe de maíz de alta fructosa) o una categoría de producto. Puede referirse a una formulación específica.
- Valores posibles: 1 = Sí, 0 = No.

### Sin Azucar

- Tipo: Binario/entero
- Descripción: Indicador de que el producto es sin azúcar.
- Valores posibles: 1 = Sí, 0 = No.

### Vel_llenado \_botellas/ horas

- Tipo: Entero o numérico
- Descripción: Velocidad de llenado de botellas medida en botellas por hora.
- Nota: en el nombre de la columna hay un espacio y barra; puede ser útil normalizar este campo para análisis futuros.

### Nivel de espumado

- Tipo: Entero/objetivo
- Descripción: Clasificación del nivel de espumado del producto durante el llenado.
- Valores posibles: categorías numéricas que representan grados de espumado.
- Uso: variable objetivo principal para el modelado de clasificación.

## Observaciones

- El archivo procesado tiene 171 registros según el análisis del dataset.
- Algunos campos binarios (`Azucar`, `JMAF`, `Sin Azucar`) se utilizan para diferenciar variantes de producto o formulaciones.
- Antes de usar el dataset en modelos predictivos es recomendable validar las unidades de medida y normalizar nombres de columnas para evitar inconsistencias.
