# Challenge Telecom X: Análisis de Evasión de Clientes - Parte 2

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/tallonson69/telecom-churn-analisis2/blob/main/analisis_churn.ipynb)

## Objetivo
Desarrollar modelos predictivos para identificar clientes con alta probabilidad de cancelación (churn) en Telecom X.

## Estructura del Repositorio
- `analisis_churn.ipynb`: Notebook principal con el análisis completo
- `datos_tratados.csv`: Dataset procesado para el modelado
- `README.md`: Documentación del proyecto

## Carga de Datos en Colab
```python
import pandas as pd
url = "https://raw.githubusercontent.com/tallonson69/telecom-churn-analisis2/main/datos_tratados.csv"
df = pd.read_csv(url)

Proceso de Análisis
    Preprocesamiento:
        Limpieza y transformación de datos
        Codificación de variables categóricas
        Balanceo de clases con SMOTE
    Modelado:
        Regresión Logística (baseline)
        Random Forest (optimizado)
        XGBoost (mejor performance)
    Resultados:
        Accuracy máximo: 84% (XGBoost)
        Variables más influyentes:
            Tipo de contrato
            Antigüedad del cliente (tenure)
            Servicios adicionales contratados

Recomendaciones Estratégicas
    Conversión de contratos mensuales a anuales
    Programas de onboarding para clientes nuevos (<12 meses)
    Paquetes de servicios con valor agregado

Requisitos Técnicos
!pip install pandas scikit-learn xgboost imbalanced-learn

Cómo Contribuir
    Clona el repositorio
    Abre el notebook en Colab usando el botón superior
    Ejecuta el análisis paso a paso
