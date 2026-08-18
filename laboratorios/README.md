# Intelligent Document to Speech

Laboratorio práctico para construir un flujo serverless en AWS capaz de extraer texto de documentos mediante servicios de inteligencia artificial y convertir el contenido extraído en audio.

## 🎯 Objetivo

Implementar una arquitectura que permita:

1. Almacenar un documento en Amazon S3.
2. Procesarlo mediante AWS Lambda.
3. Extraer su contenido utilizando Amazon Textract.
4. Convertir el texto extraído en voz mediante Amazon Polly.
5. Almacenar el archivo de audio resultante en Amazon S3.

## 🏗️ Arquitectura

```text
Documento
    │
    ▼
Amazon S3
    │
    ▼
AWS Lambda
    │
    ├────► Amazon Textract
    │          │
    │          ▼
    │      Texto extraído
    │          │
    │◄─────────┘
    │
    ├────► Amazon Polly
    │          │
    │          ▼
    │       Audio MP3
    │          │
    │◄─────────┘
    │
    ▼
Amazon S3
```

## ☁️ Servicios AWS utilizados

| Servicio          | Función                                                     |
| ----------------- | ----------------------------------------------------------- |
| Amazon S3         | Almacenamiento de documentos de entrada y archivos de audio |
| AWS Lambda        | Orquestación serverless del procesamiento                   |
| Amazon Textract   | Extracción automática de texto de documentos                |
| Amazon Polly      | Conversión de texto a voz                                   |
| AWS IAM           | Control de permisos entre los servicios                     |
| Amazon CloudWatch | Logs y monitoreo de la función Lambda                       |

## 🔐 Seguridad

La función Lambda utiliza un IAM Execution Role con los permisos mínimos necesarios para:

* Leer el documento desde Amazon S3.
* Invocar las operaciones necesarias de Amazon Textract.
* Utilizar Amazon Polly para sintetizar audio.
* Escribir el archivo generado en Amazon S3.
* Generar logs en Amazon CloudWatch.

No se almacenan credenciales de AWS dentro del código fuente.

## 🧠 Conceptos estudiados

Este laboratorio permite practicar:

* Servicios de IA administrados de AWS.
* Intelligent Document Processing (IDP).
* Optical Character Recognition (OCR).
* Text-to-Speech (TTS).
* Arquitecturas serverless.
* Integración de servicios mediante APIs.
* Roles y políticas de IAM.
* Principio de mínimo privilegio.
* Monitoreo mediante CloudWatch.
* Administración de datos mediante Amazon S3.

## 🎓 Relación con AWS Certified AI Practitioner

El laboratorio ayuda a distinguir servicios especializados de IA de AWS:

* **Amazon Textract:** extracción de información de documentos.
* **Amazon Polly:** conversión de texto a voz.
* **Amazon Transcribe:** conversión de voz a texto.
* **Amazon Comprehend:** procesamiento y análisis de lenguaje natural.
* **Amazon Rekognition:** análisis de imágenes y video.

También demuestra que una solución de IA en AWS no necesariamente requiere entrenar o administrar un modelo de machine learning.

## ⚠️ Consideraciones

Esta implementación tiene fines educativos y debe revisarse antes de utilizarse con información sensible o en ambientes productivos.

Para escenarios empresariales deben considerarse adicionalmente controles de acceso, cifrado, clasificación de información, auditoría, monitoreo, retención de datos y cumplimiento normativo.

