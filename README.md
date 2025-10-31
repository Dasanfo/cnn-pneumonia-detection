# CNN para Detección de Neumonía en Radiografías

Proyecto de **ciencia de datos aplicada a salud**, enfocado en la detección de **neumonía a partir de imágenes de rayos X**.  
Se implementó una **Red Neuronal Convolucional (CNN)** para clasificar entre pacientes *normales* y *COVID/neumonía*, utilizando técnicas de preprocesamiento, *data augmentation* y balanceo de clases.

## 🎯 Objetivo
Desarrollar un modelo de aprendizaje profundo capaz de reconocer patrones radiológicos asociados a neumonía y COVID-19 en imágenes médicas.

## 🧩 Flujo de trabajo
1. **Carga y limpieza de datos**: eliminación de archivos no válidos y organización del dataset.  
2. **Análisis exploratorio (EDA)**: verificación de dimensiones, balanceo de clases y distribución de datos.  
3. **Preprocesamiento**: normalización, codificación de etiquetas, *submuestreo* y *data augmentation*.  
4. **Modelado**: CNN con capas Conv2D, MaxPooling, Dropout y Dense.  
5. **Entrenamiento y validación**: 80/20 split con optimizador *SGD*, *batch size=8*, *12 epochs*.  
6. **Evaluación**: *accuracy*, *loss* y pruebas visuales de predicción.

## 🧠 Arquitectura del modelo
Conv2D(8) → MaxPooling → Dropout(0.25)
Conv2D(16) → MaxPooling → Dropout(0.25)
Conv2D(32) → MaxPooling → Dropout(0.25)
Flatten → Dense(200, relu) → Dropout(0.4) → Dense(2, sigmoid)

## 🛠️ Tecnologías
Python · TensorFlow/Keras · OpenCV · NumPy · Matplotlib

## 📊 Resultados
- Precisión superior al **90 %** en el conjunto de prueba.  
- Dataset balanceado mediante *augmentation* controlado.  
- Flujo reproducible para otros problemas de clasificación de imágenes médicas.

## 📚 Dataset
[COVID-19 Radiography Database – Kaggle](https://www.kaggle.com/datasets/tawsifurrahman/covid19-radiography-database)

## 👨‍💻 Autor
**Daniel Santiago Forero García**  
**Camilo Andres Ortiz**  
Pontificia Universidad Javeriana – Ciencia de Datos
