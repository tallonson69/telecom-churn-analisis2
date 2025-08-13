# telecom-churn-analisis2

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/tallonson69/telecom-churn-analisis2/blob/main/notebooks/analisis_churn.ipynb)

## Objetivo
Desarrollar modelos predictivos para identificar clientes con alta probabilidad de cancelación (churn) en Telecom X, utilizando técnicas de machine learning.

## Estructura del Proyecto
- `data/raw/`: Datos originales en CSV
- `data/processed/`: Datos limpios y balanceados
- `notebooks/`: Cuaderno Jupyter/Colab con el análisis completo

## Proceso de Análisis

### 1. Preparación de Datos
- **Limpieza**: Eliminación de IDs irrelevantes
- **Transformación**: 
  - Expansión de columnas anidadas (JSON/diccionarios)
  - Codificación de variables categóricas (One-Hot Encoding)
- **Balanceo**: Aplicación de SMOTE para equilibrar clases

### 2. Modelado Predictivo
| Modelo | Accuracy | Recall | Precisión |
|--------|----------|--------|-----------|
| Regresión Logística | 0.82 | 0.83 | 0.81 |
| Random Forest | 0.82 | 0.88 | 0.79 |
| XGBoost | 0.84 | 0.86 | 0.84 |

### 3. Hallazgos Clave
![Matriz de Correlación](images/correlation_matrix.png)
*Variables más correlacionadas con el churn*

## Instrucciones de Ejecución

1. Clonar repositorio:
```bash
git clone https://github.com/tallonson69/telecom-churn-analisis2.git
