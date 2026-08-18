# ⚡ Cheatsheet — Dominio 1: IA y Machine Learning

Resumen rápido para **AWS Certified AI Practitioner (AIF-C01)**.

---

## 🧠 IA → ML → Deep Learning

```text
Artificial Intelligence
└── Machine Learning
    └── Deep Learning
```

---

## 🎓 Tipos de aprendizaje

| Tipo                   | Idea clave             |
| ---------------------- | ---------------------- |
| Supervised             | Datos etiquetados      |
| Unsupervised           | Datos sin etiquetas    |
| Reinforcement Learning | Recompensas y acciones |

---

## 🎯 Tipo de problema

| Necesito...                     | Técnica           |
| ------------------------------- | ----------------- |
| Predecir categoría              | Classification    |
| Predecir número                 | Regression        |
| Encontrar grupos                | Clustering        |
| Predecir futuro                 | Forecasting       |
| Detectar comportamiento extraño | Anomaly Detection |
| Recomendar elementos            | Recommendation    |

---

## 🚨 Overfitting vs Underfitting

**Overfitting**

```text
Low Bias
+
High Variance
```

Aprende demasiado los datos de entrenamiento y generaliza mal.

**Underfitting**

```text
High Bias
+
Low Variance
```

Modelo demasiado simple.

---

## 🔄 Ciclo ML

```text
Data Collection
      ↓
Data Preparation
      ↓
Feature Engineering
      ↓
Training
      ↓
Hyperparameter Tuning
      ↓
Evaluation
      ↓
Deployment
      ↓
Monitoring
```

---

## 🧩 ¿Qué etapa necesito?

| Escenario                            | Respuesta             |
| ------------------------------------ | --------------------- |
| Obtener más datos                    | Data Collection       |
| Crear nuevas variables               | Feature Engineering   |
| Cambiar comportamiento del algoritmo | Hyperparameter Tuning |
| Medir rendimiento                    | Model Evaluation      |
| Detectar drift                       | Model Monitoring      |

---

# 📊 Classification Metrics

### Accuracy

> ¿Cuántas predicciones totales fueron correctas?

### Precision

> De los positivos predichos, ¿cuántos eran realmente positivos?

**Penaliza FP.**

### Recall

> De los positivos reales, ¿cuántos encontré?

**Penaliza FN.**

### F1

> Equilibrio entre Precision y Recall.

---

## 🧠 Regla rápida

```text
False Positive caro
        ↓
    PRECISION

False Negative caro
        ↓
      RECALL
```

---

# 📈 Regression Metrics

| Métrica | Idea                    |
| ------- | ----------------------- |
| MAE     | Error absoluto promedio |
| MSE     | Error² promedio         |
| RMSE    | √MSE                    |
| R²      | Variación explicada     |

---

# ☁️ Servicios rápidos

| Necesidad         | AWS                |
| ----------------- | ------------------ |
| Recomendaciones   | Amazon Personalize |
| Imágenes/video    | Amazon Rekognition |
| NLP               | Amazon Comprehend  |
| Chatbot           | Amazon Lex         |
| Documentos        | Amazon Textract    |
| Voz → texto       | Amazon Transcribe  |
| Texto → voz       | Amazon Polly       |
| Foundation Models | Amazon Bedrock     |

---

# 🚨 Palabras clave del examen

**“Menor sobrecarga operativa”**

→ Buscar primero un servicio AWS administrado diseñado para el caso.

**“Más variables/features”**

→ Feature Engineering.

**“Más datos/fuentes”**

→ Data Collection.

**“Mejorar comportamiento del algoritmo”**

→ Hyperparameter Tuning.

**“Evaluar rendimiento”**

→ Model Evaluation.

**“Detectar cambios después del deployment”**

→ Model Monitoring.

---

## 🎯 Antes de cerrar este dominio debo dominar

* [ ] IA vs ML vs Deep Learning
* [ ] Supervised vs Unsupervised vs Reinforcement Learning
* [ ] Classification vs Regression
* [ ] Overfitting vs Underfitting
* [ ] Bias vs Variance
* [ ] Training vs Inference
* [ ] Data Collection vs Feature Engineering
* [ ] Training vs Hyperparameter Tuning
* [ ] Evaluation vs Monitoring
* [ ] Accuracy
* [ ] Precision
* [ ] Recall
* [ ] F1
* [ ] MAE / MSE / RMSE / R²
* [ ] Casos de uso de servicios AWS
