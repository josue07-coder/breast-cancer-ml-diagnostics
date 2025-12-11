# 🧠 Breast Cancer ML Diagnostics  
### Diagnóstico de Overfitting y Underfitting en Modelos de Aprendizaje Automático

Este proyecto analiza el dataset **Breast Cancer** utilizando varios modelos de Machine Learning.  
El objetivo principal es **diagnosticar problemas de overfitting/underfitting**, optimizar hiperparámetros y seleccionar el modelo con mejor capacidad de generalización.

---

## 📌 Objetivos del Proyecto

- Entrenar modelos base: Logistic Regression, Decision Tree y KNN.
- Analizar su comportamiento mediante **curvas de aprendizaje**.
- Evaluar impacto de hiperparámetros usando **curvas de validación**.
- Aplicar técnicas para mitigar overfitting y underfitting.
- Seleccionar el mejor modelo según métricas finales.
- Documentar todo el proceso de forma clara y reproducible.

---

## 📊 Modelos Evaluados

- **Logistic Regression**
- **Decision Tree**
- **K-Nearest Neighbors (KNN)**

Se analizaron métricas de:
- Accuracy (train/test)
- F1-score (train/test)

También se realizó diagnóstico de:
- Overfitting  
- Underfitting  
- Bias–variance tradeoff  

---

## 🔍 Archivos incluidos

/notebook/breast_cancer_analysis.ipynb → Notebook principal con análisis completo
/figures/ → Curvas de aprendizaje, validación y gráficas
/data/ → Dataset (opcional)
requirements.txt → Dependencias del proyecto

---

## ✔ Resultados Principales

- **Decision Tree sin regularizar → Overfitting severo**
- **KNN con k pequeño → Alta varianza**
- **Logistic Regression → Modelo estable con baja varianza**
- Ajustes óptimos encontrados:
  - Logistic Regression: **C = 0.1**
  - Decision Tree: **max_depth = 4**
  - KNN: **k = 7**

📌 **Modelo recomendado:**  
**Logistic Regression (C = 0.1)** por su mejor equilibrio entre precisión y generalización.

---

## 🏁 Conclusiones

Este proyecto demuestra la importancia de:
- Analizar curvas de aprendizaje para diagnosticar el comportamiento del modelo.
- Ajustar hiperparámetros basados en evidencia.
- Utilizar métricas en validación para seleccionar el mejor modelo.
- Controlar la complejidad del modelo para evitar overfitting.

---

## 🚀 Cómo ejecutar este proyecto

### 1. Clonar el repositorio
```bash
git clone https://github.com/TU_USUARIO/breast-cancer-ml-diagnostics.git
cd breast-cancer-ml-diagnostics

### 2. Instalar dependencias
pip install -r requirements.txt

3. Abrir el notebook
jupyter notebook notebook/breast_cancer_analysis.ipynb

📦 Requerimientos
numpy
pandas
matplotlib
scikit-learn
seaborn

📚 Dataset

Dataset utilizado: Breast Cancer Wisconsin Diagnostic
Disponible en Scikit-learn:

from sklearn.datasets import load_breast_cancer

👨‍💻 Autor

Proyecto desarrollado por [JOSUE BLANCO BATISTA]
Estudiante de Ingeniería en Sistemas | Data Science | Machine Learning
