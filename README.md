# 📈Pronóstico del precio de las acciones y análisis de series temporales de Meta

Este proyecto realiza un análisis completo de series temporales y pronóstico del precio de las acciones de Meta Platforms Inc. (META) utilizando enfoques estadísticos clásicos y modelos de machine learning y deep learning.

Se combinan técnicas de análisis exploratorio, modelos ARIMA y NeuralProphet para estudiar tendencias, estacionalidad y realizar predicciones de precios futuros.

## 🧠Objetivos del proyecto

- Analizar el comportamiento histórico del precio de las acciones de Meta.
- Evaluar tendencias, estacionalidad y estacionariedad de la serie temporal.
- Construir y comparar modelos de pronóstico:
- Modelos estadísticos clásicos (ARIMA).
- Modelos de Deep Learning para series temporales (NeuralProphet).
- Generar pronósticos y evaluar su desempeño mediante métricas de error.

## 📊Dataset

El conjunto de datos contiene información histórica de las acciones de Meta Platforms Inc. durante los últimos 12 años.

Columnas principales:
- Date: Fecha de cotización
- Open: Precio de apertura
- High: Precio máximo diario
- Low: Precio mínimo diario
- Close: Precio de cierre
- Adj Close: Precio de cierre ajustado
- Volume: Volumen de negociación

Los datos permiten realizar análisis históricos, estudiar patrones temporales y construir modelos de predicción financiera.

## 🔍Metodología

1️⃣ Análisis Exploratorio de Datos (EDA)
- Visualización de precios históricos.
- Análisis de tendencia y estacionalidad (mensual y anual).
- Diagramas de caja y subseries estacionales.
- Descomposición de la serie temporal.

2️⃣ Análisis de Estacionariedad
- Prueba de Dickey-Fuller Aumentada (ADF).
- Transformaciones logarítmicas.
- Diferenciación de la serie para lograr estacionariedad.
- Análisis ACF y PACF.

3️⃣ Modelos Estadísticos
- Selección automática de parámetros con auto_arima.
- Implementación de modelos ARIMA (1,1,1).
- Diagnóstico de residuos.
- Evaluación con métricas:
- MSE
- MAE
- RMSE
- MAPE

4️⃣ Deep Learning para Series Temporales
- Implementación de NeuralProphet (basado en PyTorch).
- Modelado de:
- Tendencia
- Estacionalidad
- Dependencias temporales no lineales

- Visualización de:
  - Ajuste a datos históricos
  - Predicciones futuras
  - Componentes del modelo

## 🧪Resultados

- Los modelos ARIMA capturan adecuadamente la estructura temporal básica, aunque presentan residuos con heterocedasticidad.
- NeuralProphet permite capturar patrones más complejos y no lineales.
- Se observan indicios de estacionalidad anual, aunque algunos efectos pueden estar influenciados por eventos extraordinarios (COVID-19, reestructuración de Meta, inversiones en VR).

## ⚠️Nota: Este proyecto tiene fines educativos y analíticos. No constituye recomendación financiera.

## 🛠️Tecnologías y Librerías

- Python
- Pandas / NumPy
- Matplotlib / Seaborn
- Statsmodels
- pmdarima
- Scikit-learn
- NeuralProphet (PyTorch)

## 📁Estructura del proyecto

├── Meta Dataset.csv
├── meta_stock_analysis.py
└── README.md

## 📌Próximos pasos / Mejoras posibles

- Incorporar modelos GARCH para modelar volatilidad.
- Comparar con modelos LSTM o Transformers.
- Backtesting más robusto.
- Incorporar variables macroeconómicas externas.

## 👤Autor

Flavia Hepp
Proyecto de análisis y pronóstico de series temporales aplicado a mercados financieros.
