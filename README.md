# 📊 Telecom X – Predicción de Cancelación de Clientes (Churn)

## 📥 Acceso a los Datos

El conjunto de datos utilizado en este proyecto puede descargarse directamente desde el siguiente enlace:


### Ejemplo de carga en Python:

```python
import pandas as pd

url = 'https://raw.githubusercontent.com/HectorCano96/challenge_telecomX_2/refs/heads/main/telecomX_preparado.csv'
datos = pd.read_csv(url)
```

## 🧠 Descripción General

Este proyecto forma parte del desafío **Telecom X – Parte 2**, cuyo objetivo es construir un pipeline de Machine Learning capaz de predecir qué clientes tienen alta probabilidad de cancelar sus servicios. La detección temprana del *churn* permite a la empresa implementar estrategias de retención más efectivas y personalizadas, optimizando recursos y mejorando la experiencia del cliente.

## 🎯 Objetivos del Proyecto

- 🔍 Preprocesar y preparar los datos para el modelado predictivo (limpieza, codificación, normalización).
- 📊 Analizar la correlación entre variables y seleccionar las más relevantes.
- 🤖 Entrenar y evaluar modelos de clasificación para predecir la cancelación de clientes.
- 📈 Interpretar los resultados y la importancia de las variables en los modelos.
- 🧩 Formular recomendaciones estratégicas basadas en los hallazgos del análisis.

## 🧪 Metodología

El proyecto se desarrolla en el notebook `TelecomX_LATAM_2da_parte.ipynb`, e incluye las siguientes etapas:

### 1. Carga y Preprocesamiento de Datos

- Lectura del archivo `telecomX_preparado.csv`.
- Eliminación de columnas irrelevantes como `id_cliente`.
- Codificación de variables categóricas mediante mapeo manual y One-Hot Encoding.
- Estandarización de variables numéricas para modelos sensibles a escalas.

### 2. Análisis Exploratorio

- Estudio de la distribución de la variable objetivo `abandono`.
- Identificación de desbalance de clases y su impacto en el modelado.
- Matriz de correlación para entender relaciones entre variables.

### 3. Modelado Predictivo

- Entrenamiento de dos modelos: Regresión Logística y Random Forest.
- Evaluación con métricas clave: Accuracy, Precisión, Recall, F1-score y ROC-AUC.
- Visualización de matrices de confusión y curvas ROC.
- Ajuste del umbral de clasificación para mejorar el balance entre Precisión y Recall.

### 4. Interpretación y Conclusiones

- Análisis de importancia de variables en ambos modelos.
- Identificación de factores clave que influyen en la cancelación.
- Propuestas de acciones de retención basadas en los resultados.

## 📂 Archivos del Repositorio

| Archivo                          | Descripción                                      |
|----------------------------------|--------------------------------------------------|
| `telecomX_preparado.csv`         | Conjunto de datos preprocesado.                 |
| `TelecomX_LATAM_2da_parte.ipynb` | Notebook principal del proyecto.                |
| `README.md`                      | Documentación del proyecto.                     |

## 🛠️ Tecnologías Utilizadas

- Python (`pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`)
- Jupyter Notebook
- Machine Learning supervisado
- Visualización de datos

## 📌 Conclusión

Este proyecto demuestra cómo aplicar técnicas de ciencia de datos para resolver un problema real de negocio: la predicción de cancelación de clientes. 
A través de un enfoque estructurado, se logra identificar patrones de comportamiento y variables clave que permiten a Telecom X tomar decisiones más informadas y estratégicas.
