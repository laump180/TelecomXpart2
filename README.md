# 📊 Análisis de Cancelación de Clientes (Churn) – Telecom X

## 📑 Índice

1. [Descripción del proyecto](#descripción-del-proyecto)
2. [Objetivo](#objetivo)
3. [Dataset](#dataset)
4. [Metodología](#metodología)
5. [Análisis exploratorio de datos](#análisis-exploratorio-de-datos)
6. [Modelado predictivo](#modelado-predictivo)
7. [Resultados](#resultados)
8. [Conclusiones](#conclusiones)
9. [Recomendaciones](#recomendaciones)
10. [Tecnologías utilizadas](#tecnologías-utilizadas)




# Descripción del proyecto

La cancelación de clientes (Churn) representa uno de los principales desafíos para las empresas de telecomunicaciones, ya que implica la pérdida directa de ingresos y mayores costos de adquisición de nuevos clientes.

Este proyecto analiza los factores asociados a la cancelación de clientes en **Telecom X**, utilizando técnicas de análisis exploratorio de datos y modelos de machine learning para identificar patrones y predecir el comportamiento de los clientes.



# Objetivo

Analizar las variables que influyen en la cancelación de clientes y desarrollar modelos predictivos capaces de identificar clientes con alto riesgo de churn, con el fin de apoyar estrategias de retención basadas en datos.



# Dataset

El dataset contiene información sobre clientes de Telecom X, incluyendo características demográficas, servicios contratados y comportamiento de facturación.

Entre las variables disponibles se encuentran:

* Información demográfica del cliente
* Servicios contratados
* Tipo de contrato
* Método de pago
* Cargos mensuales
* Cargos totales
* Variable objetivo **Churn**, que indica si el cliente canceló o no el servicio

Este conjunto de datos permite analizar patrones de comportamiento asociados a la cancelación.



# Metodología

El análisis se desarrolló siguiendo las siguientes etapas:

1. Carga y exploración inicial del dataset
2. Limpieza y preprocesamiento de datos
3. Análisis exploratorio de datos (EDA)
4. Transformación de variables categóricas mediante **one-hot encoding**
5. División del dataset en conjuntos de entrenamiento y prueba
6. Escalamiento de variables numéricas
7. Entrenamiento de modelos de clasificación
8. Evaluación de desempeño mediante métricas y matriz de confusión



# Análisis exploratorio de datos

Durante el análisis exploratorio se identificaron patrones relevantes en el comportamiento de los clientes.

Se observó que:

* Los clientes con **menor antigüedad** presentan mayor probabilidad de cancelar el servicio.
* Los clientes con **mayor permanencia** generan mayores cargos totales y presentan menor tasa de cancelación.
* Algunos tipos de contrato y métodos de pago muestran mayor relación con el churn.

Estos hallazgos permitieron comprender mejor el comportamiento de los clientes antes de aplicar modelos predictivos.



# Modelado predictivo

Se evaluaron diferentes modelos de clasificación para predecir la cancelación de clientes:

* Modelo baseline
* Árbol de decisión
* Regresión logística

Los modelos fueron entrenados utilizando los datos de entrenamiento y evaluados sobre el conjunto de prueba para medir su capacidad de generalización.



# Resultados

Los resultados muestran que la **regresión logística** presentó el mejor desempeño general entre los modelos evaluados.

El modelo logró identificar patrones importantes asociados a la cancelación, permitiendo distinguir entre clientes con alta y baja probabilidad de abandonar el servicio.

El análisis de la matriz de confusión permitió evaluar el comportamiento del modelo al clasificar correctamente clientes que cancelan y clientes que permanecen en la empresa.



# Conclusiones

El análisis realizado permitió identificar factores relevantes asociados a la cancelación de clientes en Telecom X.

Variables como **la antigüedad del cliente, los cargos acumulados y ciertas características del servicio contratado** tienen una influencia significativa en la probabilidad de churn.

El modelo de regresión logística demostró ser una herramienta útil para identificar clientes con riesgo de cancelación, lo que puede ayudar a la empresa a tomar decisiones preventivas.



# Recomendaciones

A partir de los resultados obtenidos se proponen las siguientes acciones:

* Implementar estrategias de retención durante los primeros meses del cliente
* Diseñar programas de fidelización para clientes con mayor antigüedad
* Utilizar modelos predictivos para identificar clientes en riesgo
* Analizar servicios y estructuras de costos asociadas a mayor tasa de cancelación
* Aplicar estrategias de marketing dirigidas a clientes con alta probabilidad de churn



# Tecnologías utilizadas

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Google Colab





* Evaluar modelos más avanzados como Random Forest o Gradient Boosting
* Aplicar técnicas de balanceo de clases
* Incorporar nuevas variables relacionadas con comportamiento del cliente
* Desarrollar dashboards interactivos para monitoreo del churn
