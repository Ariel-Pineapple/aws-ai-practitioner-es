# 03 — Ciclo de vida de Machine Learning

## 🎯 Objetivo

Comprender las principales etapas necesarias para diseñar, desarrollar, entrenar, implementar y mantener una solución de Machine Learning.

---

## 1. Vista general

Una representación simplificada del ciclo de vida de ML:

```text
Problema de negocio
        ↓
Recopilación de datos
        ↓
Preparación de datos
        ↓
Ingeniería de características
        ↓
Entrenamiento
        ↓
Ajuste de hiperparámetros
        ↓
Evaluación
        ↓
Implementación
        ↓
Inferencia
        ↓
Monitoreo
        ↓
Reentrenamiento
```

El proceso puede ser iterativo.

---

## 2. Definición del problema

### Preguntas clave

* ¿Qué queremos predecir?
* ¿Qué valor aportará el modelo?
* ¿Qué datos necesitamos?
* ¿Cómo mediremos el éxito?

---

## 3. Recopilación de datos

### Objetivo

Obtener los datos necesarios para desarrollar el modelo.

Puede involucrar:

* Diferentes fuentes de datos
* Datos estructurados
* Datos no estructurados
* Etiquetado
* Integración de nuevas fuentes

### Regla de examen

> **Necesitamos obtener más datos o incorporar nuevas fuentes → Data Collection.**

---

## 4. Preparación de datos

Puede incluir:

* Limpieza
* Eliminación de duplicados
* Tratamiento de valores faltantes
* Transformaciones
* Normalización
* Preparación para entrenamiento

---

## 5. Ingeniería de características

La **Feature Engineering** consiste en seleccionar, transformar, extraer o crear características útiles para el modelo.

Puede incluir:

* Feature creation
* Feature transformation
* Feature extraction
* Feature selection

### Regla de examen

> **Crear o transformar variables para mejorar el modelo → Feature Engineering.**

---

## 6. Entrenamiento

Durante el entrenamiento, el algoritmo utiliza los datos disponibles para aprender patrones y generar un modelo.

Conceptos por desarrollar:

* Training dataset
* Validation dataset
* Test dataset

---

## 7. Ajuste de hiperparámetros

Los hiperparámetros controlan aspectos del proceso de aprendizaje.

> **Hyperparameter tuning modifica el comportamiento/configuración del algoritmo; no crea nuevas variables en el dataset.**

---

## 8. Evaluación

Después del entrenamiento debemos medir el rendimiento del modelo.

Ejemplos de métricas:

* Accuracy
* Precision
* Recall
* F1
* MAE
* MSE
* RMSE

Ver:

`04-metricas-evaluacion.md`

---

## 9. Implementación

Una vez validado, el modelo puede implementarse para generar inferencias sobre nuevos datos.

> Pendiente de ampliar.

---

## 10. Monitoreo

Un modelo implementado debe supervisarse.

Conceptos importantes:

* Calidad del modelo
* Calidad de datos
* Data drift
* Model drift
* Bias drift
* Feature attribution drift

> Pendiente de ampliar durante el estudio.

---

## 11. Reentrenamiento

Los modelos pueden necesitar nuevos entrenamientos cuando:

* cambian los datos;
* disminuye el rendimiento;
* aparecen nuevos patrones;
* cambia el problema empresarial.

---

## ⚠️ Diferencias importantes para el examen

| Necesidad                                 | Etapa                 |
| ----------------------------------------- | --------------------- |
| Obtener datos adicionales                 | Data Collection       |
| Crear nuevas variables                    | Feature Engineering   |
| Modificar el comportamiento del algoritmo | Hyperparameter Tuning |
| Saber qué tan bien funciona               | Evaluation            |
| Detectar degradación/cambios              | Monitoring            |
| Actualizar el modelo con nuevos datos     | Retraining            |

---

## ❓ Preguntas para repasar

* [ ] ¿Qué diferencia existe entre Data Collection y Feature Engineering?
* [ ] ¿Qué diferencia existe entre parámetros e hiperparámetros?
* [ ] ¿Cuándo se realiza Model Evaluation?
* [ ] ¿Qué función cumple Model Monitoring?
* [ ] ¿Qué puede provocar la necesidad de reentrenar un modelo?

---

> 🚧 Este documento será ampliado conforme avance el estudio del ciclo de vida de ML.
