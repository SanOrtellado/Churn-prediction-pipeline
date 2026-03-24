

# Churn-prediction-pipeline 🧉 (Python + scikit-learn)


<img width="600" height="660" alt="image" src="https://github.com/user-attachments/assets/b0a7ef05-98ad-4c77-9b0d-03fed0ed2318" />

RESULTADO_ OUTPUT


<img width="522" height="621" alt="image" src="https://github.com/user-attachments/assets/62164dec-0931-4088-9c69-cd1a7907c7f2" />


Mini proyecto **end-to-end** de Machine Learning en Python para **predecir churn** (probabilidad de que un cliente cancele un servicio).  

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
¿Para qué sirve en la vida real?
Para anticiparse a la baja de clientes: detectar perfiles con alto riesgo de churn y priorizar acciones de retención (soporte, promociones, mejoras), evitando trabajar “a ciegas”.

- Genera artifacts:
  - `model_churn.joblib`
  - `metrics.json`

## Cómo correrlo
```bash
pip install -r requirements.txt
python mini_ml_churn.py
