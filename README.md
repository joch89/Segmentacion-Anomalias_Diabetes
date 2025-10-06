# Evaluación Modular 6: Segmentación y Detección de Anomalías en Pacientes Crónicos

## 🎯 Objetivo del Proyecto

Aplicar técnicas avanzadas de **aprendizaje no supervisado** para identificar grupos de pacientes con condiciones clínicas similares (segmentación) y detectar perfiles atípicos (detección de anomalías) dentro del conjunto de datos **Pima Indians Diabetes Dataset**.

El análisis se centra en la justificación de las decisiones de *clustering* y reducción de dimensionalidad en función de las métricas de evaluación y la interpretabilidad clínica de los resultados.

## 💻 Metodología y Técnicas Aplicadas

| Categoría | Métodos Implementados |
| :--- | :--- |
| **Clustering** | K-Means, DBSCAN, HDBSCAN, Clustering Jerárquico |
| **Reducción de Dimensionalidad** | PCA, t-SNE, UMAP |
| **Detección de Anomalías** | Isolation Forest, One-Class SVM |
| **Evaluación** | Coeficiente de Silhouette, Índice de Davies-Bouldin |

---

## 📊 Conclusiones y Resultados Clave

* **Mejor Agrupamiento:** La combinación de **UMAP** con **DBSCAN** o **HDBSCAN** permitió una visualización más clara y una mejor definición de *clusters* en el espacio de baja dimensión, superando a PCA para este propósito.
* **Validación de Anomalías:** Los pacientes identificados como atípicos (outliers) por **Isolation Forest** y **One-Class SVM** coincidieron significativamente con los puntos de ruido detectados por DBSCAN. Esto sugiere que estos pacientes presentan perfiles de características clínicas genuinamente inusuales en comparación con la población general del estudio.

## 🖼️ Visualización Principal

El siguiente gráfico ilustra la segmentación obtenida después de la reducción de dimensionalidad, mostrando la identificación de *clusters* y los puntos anómalos.

**Gráfico de Segmentación y Detección de Anomalías (Ejemplo)**

![Gráfico del resultado principal que muestra los clústeres de pacientes y los outliers.](Proyecto_3.png)

## 📁 Archivos

* Segmentacion-anomalias-diabetes.ipynb: El código fuente completo con el preprocesamiento, la aplicación de modelos y el análisis comparativo.
* `Proyecto_3`: Archivo con visualización del resultado de un modelo.
