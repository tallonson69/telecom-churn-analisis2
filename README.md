# Telecom Churn Prediction Analysis

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/tallonson69/telecom-churn-analisis2/blob/main/analisis_churn.ipynb)

## Objetivo
Desarrollar modelos predictivos para identificar clientes con alta probabilidad de cancelación (churn) en Telecom X, utilizando técnicas de machine learning en Google Colab.

## Estructura del Proyecto
- `analisis_churn.ipynb`: Notebook principal con el análisis completo
- `data/`: Carpeta para archivos de datos (opcional)

## Proceso de Análisis

### 1. Preparación de Datos
- Limpieza de datos y manejo de valores nulos
- Codificación de variables categóricas (One-Hot Encoding)
- Balanceo de clases con SMOTE

### 2. Modelado Predictivo
| Modelo | Accuracy | Recall | Precisión |
|--------|----------|--------|-----------|
| Regresión Logística | 0.82 | 0.83 | 0.81 |
| Random Forest | 0.82 | 0.88 | 0.79 |
| XGBoost | 0.84 | 0.86 | 0.84 |

### 3. Hallazgos Clave
- Factores que más influyen en el churn:
  1. Tipo de contrato (mes a mes vs anual)
  2. Antigüedad del cliente
  3. Servicios adicionales contratados

## Cómo Usar este Proyecto

1. Haz clic en el botón "Open in Colab" arriba
2. Conecta el notebook a tu entorno de Google Colab
3. Ejecuta las celdas secuencialmente

## Requisitos
El notebook incluye todas las instalaciones necesarias, pero estas son las principales dependencias:
```python
!pip install pandas scikit-learn xgboost imbalanced-learn

### Resultados

Los modelos identificaron que los clientes con:

    Contratos mensuales

    Menos de 12 meses de antigüedad

    Servicio Fiber Optic sin soporte técnico

Tienen hasta 3x más probabilidad de cancelar.
Estrategias Recomendadas

    Programas de fidelización para contratos anuales

    Atención especial durante los primeros 12 meses

    Paquetes de servicios con valor agregado
