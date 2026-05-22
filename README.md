# pronosticos_predicciones
Este proyecto ayuda a una cadena de gimnasios a determinar cuando hay posibilidades de riesgo, determinar cuales de sus usuarios mas vulnerables a presindir del servicio.
Descripción del proyecto

La cadena de gimnasios Model Fitness busca desarrollar una estrategia de interacción basada en análisis de datos para reducir la pérdida de clientes (churn).

La cancelación de clientes representa un problema importante para gimnasios y servicios por suscripción, ya que afecta ingresos, crecimiento y costos de adquisición. El objetivo de este proyecto es utilizar técnicas de análisis exploratorio, aprendizaje automático y segmentación para identificar patrones asociados con la pérdida de clientes y generar recomendaciones de negocio.

Objetivos

Este proyecto tiene los siguientes objetivos principales:

Predecir la probabilidad de cancelación de clientes para el próximo mes.
Identificar perfiles típicos de usuarios mediante segmentación.
Analizar factores que influyen en la pérdida de clientes.
Proponer estrategias para mejorar la retención y reducir la tasa de cancelación.
Metodología
1. Análisis Exploratorio de Datos (EDA)

Se realizó:

Identificación de valores ausentes y duplicados.
Estadísticas descriptivas mediante describe().
Comparación de medias entre clientes que cancelaron y quienes permanecieron.
Visualización de distribuciones e histogramas.
Matriz de correlación para detectar relaciones entre variables.
2. Construcción de modelos predictivos

Se desarrollaron dos modelos de clasificación binaria:

Regresión logística
Entrenamiento con LogisticRegression
Evaluación mediante:
Accuracy
Precision
Recall

Bosque aleatorio
Entrenamiento con RandomForestClassifier
Evaluación mediante:
Accuracy
Precision
Recall

Se comparó el desempeño de ambos modelos para seleccionar la mejor alternativa predictiva.

3. Segmentación de clientes

Se aplicaron técnicas de clustering para identificar grupos de usuarios con comportamientos similares:

Proceso
Estandarización de variables (StandardScaler)
Creación de matriz de distancias con linkage()
Construcción de dendrograma
Implementación de K-Means con:

n_clusters = 5

Posteriormente se analizaron:

Características promedio por clúster
Distribuciones de variables
Tasa de cancelación por grupo
Herramientas utilizadas
Python
Pandas
NumPy
Matplotlib
Seaborn
Scikit-Learn
SciPy
