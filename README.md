# Telecom Churn Prediction Analysis

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/tallonson69/telecom-churn-analisis2/blob/main/analisis_churn.ipynb)

## Objetivo
Desarrollar modelos predictivos para identificar clientes con alta probabilidad de cancelación (churn) en Telecom X.

## Estructura del Repositorio
- `analisis_churn.ipynb`: Notebook principal
- `datos_tratados.csv`: Archivo con los datos procesados
- `README.md`: Este archivo

## Cómo Cargar los Datos en Colab

### Opción 1: Desde GitHub directo
import pandas as pd
url = "https://raw.githubusercontent.com/tallonson69/telecom-churn-analisis2/main/datos_tratados.csv"
df = pd.read_csv(url)

### Opción 2: Subiendo manualmente
    Ejecuta esta celda en Colab:
from google.colab import files
uploaded = files.upload()
    Haz clic en "Seleccionar archivos" y elige datos_tratados.csv
    Lee el archivo:
import pandas as pd
df = pd.read_csv('datos_tratados.csv')

## Proceso de Análisis
    Preprocesamiento:
        Limpieza de datos
        Codificación de variables categóricas
        Balaceo con SMOTE
    Modelado:
        Regresión Logística
        Random Forest
        XGBoost
    Resultados:
        XGBoost obtuvo mejor performance (84% accuracy)
        Variables clave: tipo de contrato, antigüedad, servicios contratados

Requisitos
!pip install pandas scikit-learn xgboost imbalanced-learn

Recomendaciones
    Incentivar contratos anuales
    Programas de retención para clientes nuevos
    Paquetes de servicios con valor agregado
