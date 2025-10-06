# Proyecto: Segmentación y Detección de Anomalías en Pacientes Crónicos con Técnica de Aprendizaje No Supervisado

## 🎯 Objetivo del Proyecto

Aplicar técnicas avanzadas de **Aprendizaje No Supervisado** para identificar grupos de pacientes con condiciones clínicas similares (segmentación) y detectar perfiles atípicos (detección de anomalías) dentro del conjunto de datos **Pima Indians Diabetes Dataset**.

El análisis se centra en la justificación de las decisiones de *clustering* y reducción de dimensionalidad en función de las métricas de evaluación y la interpretabilidad clínica de los resultados.

---

## 💻 Metodología y Técnicas Aplicadas

| Categoría | Métodos Implementados |
| :--- | :--- |
| **Clustering** | K-Means, DBSCAN, HDBSCAN, Clustering Jerárquico |
| **Reducción de Dimensionalidad** | PCA, t-SNE, UMAP |
| **Detección de Anomalías** | Isolation Forest, One-Class SVM |
| **Evaluación** | Coeficiente de Silhouette, Índice de Davies-Bouldin |

---

## ⚙️ Ejecución del Notebook en Google Colab 🚀

Este proyecto se presenta en formato **Jupyter Notebook** (`.ipynb`) para facilitar la ejecución interactiva y la visualización directa de los resultados. **Google Colab** es la plataforma recomendada para correr el archivo sin necesidad de instalaciones locales.

### Ventajas del Formato Notebook:
* **Interactividad:** Permite ejecutar cada sección de código y visualizar los resultados (gráficos, salidas) paso a paso, facilitando la depuración y el entendimiento del proceso.
* **Documentación Integrada:** Combina el código ejecutable con el texto explicativo y las ecuaciones (Markdown), creando un flujo de trabajo claro y completamente documentado en un solo archivo.

### ¿Cómo Ejecutarlo?
1.  Sube el archivo `Segmentacion-anomalias-diabetes.ipynb` a tu Google Drive o ábrelo directamente en Colab.
2.  Una vez abierto, ejecuta las celdas secuencialmente o selecciona **"Entorno de ejecución"** > **"Ejecutar todas las celdas"**.

---

## 📊 Conclusiones y Resultados Clave

* **Mejor Agrupamiento:** La combinación de **UMAP** con **DBSCAN** o **HDBSCAN** permitió una visualización más clara y una mejor definición de *clusters* en el espacio de baja dimensión, superando a PCA para este propósito.
* **Validación de Anomalías:** Los pacientes identificados como atípicos (outliers) por **Isolation Forest** y **One-Class SVM** coincidieron significativamente con los puntos de ruido detectados por DBSCAN. Esto sugiere que estos pacientes presentan perfiles de características clínicas genuinamente inusuales en comparación con la población general del estudio.

---

## 🖼️ Visualización Principal

El siguiente gráfico ilustra la segmentación obtenida después de la reducción de dimensionalidad, mostrando la identificación de *clusters* y los puntos anómalos.

**Gráfico de Segmentación y Detección de Anomalías (Ejemplo)**

![Gráfico del resultado principal que muestra los clústeres de pacientes y los outliers.](proyecto_3.png)

---

## 📝 Conclusión General del Proyecto

El análisis demostró que las técnicas de aprendizaje no supervisado son altamente efectivas para revelar estructuras ocultas en datos clínicos. La elección de **UMAP** como método de reducción de dimensionalidad fue clave para obtener una visualización interpretable de los **agrupamientos de pacientes**. Se confirmó la existencia de un compromiso crítico entre optimizar las métricas puras de *clustering* (como Silhouette) y lograr **segmentos que sean clínicamente relevantes** y bien definidos. La robusta detección de anomalías por múltiples métodos (Isolation Forest y DBSCAN) identifica un subgrupo de pacientes que merecen una **investigación clínica más profunda** debido a sus perfiles de características inusuales.

---

## 📁 Archivos

* `Segmentacion-anomalias-diabetes.ipynb`: El código fuente completo con el preprocesamiento, la aplicación de modelos y el análisis comparativo.
* `Proyecto_3.png`: Archivo con visualización del resultado de un modelo (imagen en la raíz del repositorio).
