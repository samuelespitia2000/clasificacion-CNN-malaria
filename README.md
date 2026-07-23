# Clasificación de Malaria con Redes Neuronales Convolucionales

![Python](https://img.shields.io/badge/Python-3.x-3776AB?logo=python&logoColor=white)
![License](https://img.shields.io/badge/license-MIT-green)

Actividad grupal del Máster en Bioinformática (UNIR) sobre inteligencia artificial con Python: comparación de algoritmos clásicos de machine learning y diseño de una red neuronal convolucional (CNN) para clasificación de imágenes médicas.

## Contenido

**1. Algoritmos de Machine Learning (dataset Iris)**
Implementación y comparación de SVM (kernel RBF), Random Forest y Naive Bayes para clasificación multiclase, con métricas de precisión, recall, F1-score y accuracy (~0.97 con SVM).

**2. Red Neuronal Convolucional para clasificación de malaria**
Diseño y entrenamiento de una CNN (TensorFlow/Keras) para distinguir células sanguíneas **infectadas** vs. **sanas** a partir de imágenes de microscopía:
- Preprocesamiento y `data augmentation` sobre el pipeline de entrada.
- Arquitectura CNN con activación `sigmoid` en la capa final (clasificación binaria).
- Evaluación en conjunto de prueba: **90.6% de accuracy**, pérdida de 0.457.
- Curva Precision-Recall con **Average Precision de 0.967**.
- Análisis de predicciones correctas e incorrectas sobre el conjunto de test.

## Dataset

Imágenes de células sanguíneas (infectadas/sanas) del dataset público de malaria del NIH ([Malaria Cell Images Dataset](https://lhncbc.nlm.nih.gov/LHC-downloads/downloads.html#malaria-datasets), también disponible en [Kaggle](https://www.kaggle.com/datasets/iarunava/cell-images-for-detecting-malaria)). El dataset de imágenes (~350 MB) no se incluye en este repositorio por su tamaño; el notebook contiene las instrucciones de carga.

## Estructura del repositorio

```
├── notebook/
│   └── Actividad_3_Python.ipynb   # Notebook completo (Google Colab)
├── LICENSE
└── README.md
```

## Herramientas

Python · TensorFlow/Keras · Scikit-learn (SVM, Random Forest, Naive Bayes) · Google Colab

## Autoría

Samuel David Espitia Contreras.

## Licencia

Distribuido bajo licencia MIT — ver [LICENSE](LICENSE).
