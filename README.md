# Telecom X – Predicción de Cancelación de Clientes (Churn)

## Descripción del proyecto

Este proyecto forma parte del **Challenge Telecom X – Parte 2**, cuyo objetivo es desarrollar modelos de **Machine Learning capaces de predecir la cancelación de clientes (churn)**.

La cancelación de clientes representa un problema crítico para las empresas de telecomunicaciones, ya que adquirir nuevos clientes suele ser más costoso que retener a los existentes. Mediante el uso de análisis de datos y modelos predictivos, este proyecto busca identificar **los factores que influyen en la cancelación** y anticipar qué clientes presentan mayor riesgo de abandonar el servicio.

El análisis se desarrolla utilizando **Python, Pandas, Scikit-learn y herramientas de visualización**, siguiendo un flujo de trabajo completo de ciencia de datos.

---

# Objetivos del análisis

El proyecto tiene los siguientes objetivos principales:

- Preparar los datos para el modelado predictivo.
- Analizar la relación entre diferentes variables y la cancelación de clientes.
- Construir modelos de Machine Learning capaces de predecir churn.
- Evaluar el desempeño de los modelos utilizando métricas de clasificación.
- Identificar las variables más importantes en la predicción.
- Generar conclusiones estratégicas para mejorar la retención de clientes.

---

# Tecnologías utilizadas

Este proyecto utiliza las siguientes herramientas y bibliotecas:

- Python 3
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook / Google Colab

---

# Estructura del proyecto

El repositorio está organizado de la siguiente manera:
TelecomX-Churn-Prediction/
│
├── data/
│ └── telecom_datos_tratados.csv
│
├── notebook/
│ └── TelecomX_Churn_Prediction.ipynb
│
└── README.md


### Descripción de carpetas

**data/**  
Contiene el dataset utilizado para el análisis y modelado.

**notebook/**  
Incluye el notebook principal con todo el flujo del proyecto:

- limpieza de datos
- análisis exploratorio
- preparación para Machine Learning
- entrenamiento de modelos
- evaluación
- conclusiones

**images/**  
Gráficos generados durante el análisis que ayudan a explicar los resultados.

---

# Flujo de análisis

El proyecto sigue un pipeline clásico de ciencia de datos:

1. **Carga de datos**
2. **Limpieza y preparación**
3. **Eliminación de variables irrelevantes**
4. **Transformación de variables categóricas**
5. **Análisis de correlación**
6. **Análisis exploratorio dirigido**
7. **División entrenamiento / prueba**
8. **Entrenamiento de modelos**
9. **Evaluación de modelos**
10. **Análisis de importancia de variables**
11. **Conclusiones estratégicas**

---

# Análisis exploratorio

Durante el análisis se investigaron diversos factores asociados al churn.

## Distribución de cancelación

Se analizó la proporción de clientes que cancelan el servicio frente a los que permanecen activos.

Esto permite detectar posibles **problemas de desbalance de clases**, lo cual puede afectar el rendimiento de los modelos predictivos.

---

## Análisis de correlación

Se construyó una **matriz de correlación** para identificar las variables más asociadas con la cancelación.

Entre los factores más relevantes destacan:

- Tipo de contrato
- Tiempo de permanencia del cliente (tenure)
- Gasto mensual
- Gasto total
- Método de pago

---

## Análisis dirigido

Se realizaron análisis específicos entre variables clave y churn, por ejemplo:

- Tenure vs cancelación
- TotalCharges vs cancelación
- MonthlyCharges vs cancelación
- Tipo de contrato vs cancelación

Estos análisis permitieron identificar patrones importantes en el comportamiento de los clientes.

---

# Modelos de Machine Learning

Se entrenaron dos modelos de clasificación para predecir churn:

### 1. Regresión Logística

Este modelo permite interpretar cómo cada variable influye en la probabilidad de cancelación.

Se aplicó **estandarización de variables** debido a que este algoritmo es sensible a la escala de los datos.

---

### 2. Random Forest

Random Forest es un modelo basado en árboles que:

- no requiere normalización
- captura relaciones no lineales
- suele tener buen desempeño en problemas de clasificación.

Además permite obtener la **importancia de variables**, lo cual ayuda a interpretar el modelo.

---

# Evaluación de modelos

Los modelos fueron evaluados utilizando las siguientes métricas:

- Accuracy
- Precision
- Recall
- F1-score
- Matriz de confusión

Estas métricas permiten medir la capacidad del modelo para identificar correctamente a los clientes que cancelarán el servicio.

En problemas de churn, **recall y F1-score son especialmente importantes**, ya que el objetivo es detectar a los clientes en riesgo de cancelación.

---

# Variables más importantes

El análisis de importancia de variables permitió identificar los principales factores asociados al churn.

Entre los más relevantes se encuentran:

- Tipo de contrato
- Tiempo de permanencia (tenure)
- Cargos mensuales
- Método de pago
- Servicios de internet y soporte técnico

Estos factores influyen significativamente en la probabilidad de cancelación.

---

# Conclusiones estratégicas

A partir del análisis y los modelos predictivos se identificaron varias oportunidades estratégicas para Telecom X.

### Principales hallazgos

Los clientes con mayor probabilidad de cancelación suelen:

- tener **contratos mensuales**
- presentar **menor tiempo de permanencia**
- tener **cargos mensuales elevados**
- utilizar ciertos **métodos de pago**
- no contar con servicios adicionales como soporte técnico o seguridad.

---

### Recomendaciones

Telecom X podría implementar estrategias como:

- Incentivar contratos de mayor duración.
- Diseñar campañas de retención durante los primeros meses del cliente.
- Ofrecer paquetes de servicios adicionales (seguridad, soporte técnico).
- Detectar clientes de alto riesgo mediante modelos predictivos y aplicar acciones preventivas.

---

# Cómo ejecutar el proyecto

## 1. Clonar el repositorio

```bash
git clone https://github.com/tuusuario/telecomx-churn-prediction.git

pip install pandas numpy matplotlib seaborn scikit-learn

TelecomX_Churn_Prediction.ipynb

