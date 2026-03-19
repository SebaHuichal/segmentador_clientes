# 🛒 Segmentador Inteligente de Clientes Minoristas

Este proyecto aplica técnicas de Machine Learning no supervisado para resolver un problema de negocio para la consultora **Retail Insights S.A.**: migrar de un marketing masivo genérico a estrategias altamente personalizadas basadas en el comportamiento real de los consumidores.

A través del análisis de una base de datos de 2000 clientes con 11 variables demográficas, de gasto y de interacción digital, el sistema descubre patrones ocultos y agrupa a los usuarios en segmentos accionables.

## 🚀 Objetivo del Proyecto
Desarrollar un modelo escalable de segmentación de clientes utilizando algoritmos de clusterización y reducción de dimensionalidad. El resultado permite optimizar campañas de marketing, gestionar inventarios y diseñar estrategias de fidelización precisas.

## 📁 Estructura del Repositorio
El análisis está dividido en 5 cuadernos (Jupyter Notebooks) secuenciales:

* **`proyecto7_leccion1.ipynb`:** Fundamentos teóricos del aprendizaje no supervisado aplicados al retail.
* **`proyecto7_leccion2.ipynb`:** Evaluación de técnicas de clusterización (K-Means, DBSCAN, Jerárquico).
* **`proyecto7_leccion3.ipynb`:** Preprocesamiento de datos y reducción de dimensionalidad usando PCA (reteniendo >80% de la varianza) y visualización inicial con t-SNE.
* **`proyecto7_leccion4.ipynb`:** Entrenamiento y evaluación de algoritmos. Determinación del número óptimo de clústeres (k=4) usando el Método del Codo y el Coeficiente de Silueta.
* **`proyecto7_leccion5.ipynb`:** Evaluación final, definición de perfiles comerciales y recomendaciones de negocio estratégicas.
* **`clientes_alta_dimension.csv`:** Dataset base utilizado para el entrenamiento de los modelos.

## 🛠️ Tecnologías y Herramientas
* **Lenguaje:** Python
* **Manipulación de Datos:** Pandas, NumPy
* **Machine Learning:** Scikit-learn (PCA, t-SNE, KMeans, DBSCAN, AgglomerativeClustering, silhouette_score)
* **Visualización:** Matplotlib, Seaborn

## 📊 Resultados: Perfiles Identificados
El modelo K-Means segmentó la base en 4 grupos con características claras:
1. **Los VIPs:** Alto nivel de ingresos y gasto. Compran en múltiples categorías y prefieren artículos de alto valor.
2. **Digitales/Tecnológicos:** Fuerte interacción con la app móvil y alta respuesta a promociones digitales. Gasto concentrado en Electrónica.
3. **Ahorradores Recurrentes:** Alta frecuencia de visitas físicas, pero ticket promedio bajo. Enfocados en artículos de primera necesidad (Hogar y Alimentos).
4. **Ocasionales:** Baja lealtad, visitas esporádicas y nivel de gasto mínimo.
