# Challenge Telecom X: análisis de evasión de clientes - Parte 2

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/tallonson69/telecom-churn-analisis2/blob/main/analisis_churn.ipynb)

## Objetivo
Desarrollar modelos predictivos para identificar clientes con alta probabilidad de cancelación (churn) en Telecom X.

## Estructura del Repositorio
- `analisis_churn.ipynb`: Notebook principal
- `datos_tratados.csv`: Archivo con los datos procesados
- `README.md`: Este archivo

## Cómo Cargar los Datos en Colab

import pandas as pd
url = "https://raw.githubusercontent.com/tallonson69/telecom-churn-analisis2/main/datos_tratados.csv"
df = pd.read_csv(url)

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

Recomendaciones
    Incentivar contratos anuales
    Programas de retención para clientes nuevos
    Paquetes de servicios con valor agregado

Requisitos
!pip install pandas scikit-learn xgboost imbalanced-learn
