# 📊 Telecom Customer Churn & Segmentation Pipeline

Este proyecto desarrolla un enfoque analítico dual para abordar la retención y el valor del cliente en una empresa de telecomunicaciones, utilizando un dataset de más de 7,000 registros (IBM). El pipeline implementa **Segmentación Avanzada** y **Modelado Predictivo** para optimizar las estrategias de Customer Success.

---

## 🚀 Resumen del Enfoque del Proyecto

### 1️⃣ Fase 1: Segmentación Geométrica de Clientes (RFM + K-Means)
A partir de métricas de Antigüedad (*Tenure*), Frecuencia de Servicios y Cargos Mensuales (*Monetario*), escalamos los datos y aplicamos el **Método del Codo** para determinar el número óptimo de clusters ($K = 3$).
* **Segmento VIP / Core:** Clientes de alta lealtad, consumo masivo de servicios y alto margen de ingresos.
* **Segmento Nuevos de Alto Gasto / Riesgo:** Clientes con baja antigüedad pero alta facturación. Representan el foco crítico para la retención preventiva.
* **Segmento Básicos / Low Cost:** Usuarios enfocados en optimizar su presupuesto, con consumo de servicios mínimos esenciales.

### 2️⃣ Fase 2: Predicción de Abandono (Decision Tree Classifier)
Se estructuró un modelo predictivo utilizando un Árbol de Decisión (`max_depth=4` para evitar sobreentrenamiento), logrando una **precisión general del 79.56%** en el set de test.
* El análisis de **Feature Importance** reveló de forma contundente que los dos principales gatillos de fuga son la **Antigüedad del Cliente** y la contratación del servicio de **Fibra Óptica**.

---

## 🛠️ Tecnologías y Librerías Utilizadas

* **Lenguaje:** Python 3.12
* **Manipulación de Datos:** `pandas`, `numpy`
* **Machine Learning / Preprocesamiento:** `scikit-learn` (`StandardScaler`, `KMeans`, `DecisionTreeClassifier`, `train_test_split`)
* **Visualización de Datos:** `matplotlib`, `seaborn` (incluyendo análisis geométrico en 3D)

---

## 📂 Estructura del Repositorio

* `proyecto_churn.ipynb`: Cuaderno de Jupyter estructurado con el pipeline completo de ingeniería de variables, segmentación y modelado predictivo.
* `.gitignore`: Configurado estratégicamente para excluir los archivos de datos crudos (`.xlsx`), manteniendo el repositorio optimizado según las buenas prácticas de desarrollo.

---
_Proyecto desarrollado como pieza estratégica para portafolio profesional en Data Science y Customer Analytics._
