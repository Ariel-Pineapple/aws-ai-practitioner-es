# 02 — Casos de uso de Inteligencia Artificial

## 🎯 Objetivo

Aprender a identificar cuándo un problema puede resolverse mediante Inteligencia Artificial o Machine Learning y qué tipo de solución resulta más apropiada.

---

## 1. Identificación del problema

Antes de elegir una tecnología debemos identificar:

* ¿Qué problema queremos resolver?
* ¿Qué datos tenemos disponibles?
* ¿Qué resultado esperamos obtener?
* ¿Necesitamos predecir, clasificar, recomendar, generar o detectar algo?
* ¿Es realmente necesario utilizar IA?

---

## 2. Casos de uso comunes

### Clasificación

**Objetivo:** asignar una categoría.

Ejemplos:

> Por completar.

### Regresión

**Objetivo:** predecir un valor numérico.

Ejemplos:

> Por completar.

### Clustering

**Objetivo:** encontrar grupos o patrones sin categorías previamente definidas.

Ejemplos:

> Por completar.

### Forecasting

**Objetivo:** predecir valores futuros utilizando información histórica.

Ejemplos:

> Por completar.

### Recomendaciones

**Objetivo:** recomendar elementos relevantes para un usuario.

Ejemplos:

> Por completar.

### Detección de anomalías

**Objetivo:** identificar comportamientos o valores inusuales.

Ejemplos:

> Por completar.

### Procesamiento del lenguaje natural

Casos:

* Clasificación de texto
* Análisis de sentimiento
* Extracción de información
* Traducción
* Resumen

### Computer Vision

Casos:

* Clasificación de imágenes
* Detección de objetos
* Análisis de imágenes y video
* Moderación de contenido

### IA generativa

Casos:

* Generación de texto
* Generación de imágenes
* Resumen
* Asistentes conversacionales
* Generación de código

---

## 3. ¿IA o solución tradicional?

No todos los problemas necesitan Machine Learning.

### Machine Learning puede ser apropiado cuando:

* Existen patrones complejos en los datos.
* Hay suficientes datos disponibles.
* Las reglas serían difíciles de definir manualmente.
* Se necesita realizar predicciones sobre nuevos datos.

### Una solución tradicional puede ser mejor cuando:

* El problema puede resolverse mediante reglas simples.
* El comportamiento debe ser completamente determinista.
* No existen suficientes datos.
* La IA no aporta una ventaja significativa.

---

## 4. Mapa de decisión

```text
¿Qué necesito hacer?

├── Predecir una categoría
│   └── Clasificación
│
├── Predecir un número
│   └── Regresión
│
├── Encontrar grupos sin etiquetas
│   └── Clustering
│
├── Predecir valores futuros
│   └── Forecasting
│
├── Detectar comportamiento inusual
│   └── Detección de anomalías
│
├── Sugerir productos/contenido
│   └── Recomendación
│
└── Crear contenido nuevo
    └── IA generativa
```

---

## 5. Servicios AWS relacionados

| Necesidad       | Servicio AWS       | Notas       |
| --------------- | ------------------ | ----------- |
| Recomendaciones | Amazon Personalize | Por ampliar |
| Imágenes/video  | Amazon Rekognition | Por ampliar |
| NLP             | Amazon Comprehend  | Por ampliar |
| Chatbots        | Amazon Lex         | Por ampliar |
| Texto → voz     | Amazon Polly       | Por ampliar |
| Voz → texto     | Amazon Transcribe  | Por ampliar |
| Documentos      | Amazon Textract    | Por ampliar |
| IA generativa   | Amazon Bedrock     | Por ampliar |

---

## ⚠️ Confusiones frecuentes

### Servicio administrado vs construir un modelo

Cuando el escenario pide:

> **“menor sobrecarga operativa”**

considerar primero si AWS dispone de un servicio administrado diseñado específicamente para ese caso antes de construir o entrenar un modelo personalizado.

---

## ❓ Preguntas para repasar

* [ ] ¿Clasificación o regresión?
* [ ] ¿Cuándo utilizar clustering?
* [ ] ¿Qué problema resuelve forecasting?
* [ ] ¿Cuándo utilizar un sistema de recomendaciones?
* [ ] ¿Cuándo NO utilizar ML?
* [ ] ¿Qué significa “menor sobrecarga operativa” en un escenario AWS?
* [ ] ¿Qué servicios administrados de AWS resuelven casos específicos de IA?

---

> 🚧 Este documento será ampliado conforme avance el estudio y la práctica.
