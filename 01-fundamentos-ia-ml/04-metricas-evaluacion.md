# 04 — Métricas de evaluación de Machine Learning

## 🎯 Objetivo

Comprender cómo evaluar el rendimiento de diferentes tipos de modelos de Machine Learning y seleccionar la métrica adecuada según el problema.

---

# 1. Clasificación

## Matriz de confusión

|               | Predicción positiva | Predicción negativa |
| ------------- | ------------------: | ------------------: |
| Real positivo |  True Positive (TP) | False Negative (FN) |
| Real negativo | False Positive (FP) |  True Negative (TN) |

---

## Accuracy

**Pregunta que responde:**

> ¿Qué proporción total de predicciones fue correcta?

```text
Accuracy = (TP + TN) / (TP + TN + FP + FN)
```

### Útil cuando

> Por completar.

### Problema

> Por completar.

---

## Precision

**Pregunta mental:**

> De todo lo que el modelo dijo que era positivo, ¿cuánto realmente lo era?

```text
Precision = TP / (TP + FP)
```

### Importante cuando:

Los **False Positives** son especialmente costosos.

---

## Recall

También llamado **Sensitivity**.

**Pregunta mental:**

> De todos los positivos reales, ¿cuántos encontró el modelo?

```text
Recall = TP / (TP + FN)
```

### Importante cuando:

Los **False Negatives** son especialmente costosos.

---

## F1 Score

Combina **Precision y Recall**.

```text
F1 = 2 × (Precision × Recall) / (Precision + Recall)
```

Puede ser útil cuando necesitamos equilibrar ambas métricas.

---

# 2. Regresión

## MAE — Mean Absolute Error

> Por completar.

```text
MAE = promedio(|valor real - predicción|)
```

---

## MSE — Mean Squared Error

> Por completar.

```text
MSE = promedio((valor real - predicción)²)
```

---

## RMSE — Root Mean Squared Error

> Por completar.

```text
RMSE = √MSE
```

---

## R² — Coefficient of Determination

> Por completar.

---

# 3. Cómo elegir una métrica

```text
¿Qué problema tengo?

├── Clasificación
│
│   ├── Clases balanceadas / error similar
│   │       └── Accuracy
│   │
│   ├── Me preocupan los False Positives
│   │       └── Precision
│   │
│   ├── Me preocupan los False Negatives
│   │       └── Recall
│   │
│   └── Necesito equilibrio Precision/Recall
│           └── F1
│
└── Regresión
    │
    ├── Error absoluto interpretable
    │       └── MAE
    │
    ├── Penalizar errores grandes
    │       └── MSE / RMSE
    │
    └── Variación explicada
            └── R²
```

---

# 4. Métrica vs objetivo empresarial

La mejor métrica no depende únicamente del algoritmo.

También depende del **costo empresarial de equivocarse**.

### Ejemplo conceptual

Si un **False Negative** es particularmente peligroso:

→ priorizar **Recall**.

Si un **False Positive** es particularmente costoso:

→ priorizar **Precision**.

---

# 5. Conceptos pendientes de estudiar

* [ ] ROC
* [ ] AUC
* [ ] Specificity
* [ ] Métricas para datasets desbalanceados
* [ ] Métricas de regresión
* [ ] Selección de métricas según escenarios AWS

---

## ❓ Preguntas para repasar

* [ ] ¿Qué mide Accuracy?
* [ ] ¿Qué diferencia existe entre Precision y Recall?
* [ ] ¿Cuándo priorizar Recall?
* [ ] ¿Cuándo priorizar Precision?
* [ ] ¿Por qué Accuracy puede ser engañosa?
* [ ] ¿Qué métrica penaliza más los errores grandes en regresión?
* [ ] ¿Qué diferencia existe entre MAE, MSE y RMSE?

---

> 🚧 Este documento será ampliado durante el estudio de métricas y evaluación.
