

# Churn-prediction-pipeline 🧉📉 (Python + scikit-learn)


<img width="886" height="992" alt="image" src="https://github.com/user-attachments/assets/ed845121-8871-48a6-b968-78c446d1eb4d" />

<img width="816" height="1025" alt="image" src="https://github.com/user-attachments/assets/a5f9eee9-3b29-4bcd-8e0d-c6ecca4bd881" />



Mini proyecto **end-to-end** de Machine Learning en Python para **predecir churn** (probabilidad de que un cliente cancele un servicio).  
Ideal como demo corta para portfolio / LinkedIn: dataset real, pipeline reproducible, métricas y artifacts.

## Qué hace
- Carga un dataset público de *Telco Customer Churn*
- Limpia datos y separa **train/test**
- Preprocesa features en un **Pipeline**:
  - numéricas: imputación (mediana) + escalado
  - categóricas: imputación (más frecuente) + one-hot encoding
- Entrena un modelo baseline explicable: **Logistic Regression** (`class_weight="balanced"`)
- Evalúa con métricas:
  - Accuracy
  - ROC-AUC
  - (opcional) Precision/Recall/F1 para la clase churn
- Genera artifacts:
  - `model_churn.joblib`
  - `metrics.json`

## Cómo correrlo
```bash
pip install -r requirements.txt
python mini_ml_churn.py
