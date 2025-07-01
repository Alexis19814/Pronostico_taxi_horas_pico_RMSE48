# Pronostico_taxi_horas_pico_RMSE48

🧭1. Definición del problema
Objetivo: Predecir la cantidad de pedidos de taxi para la próxima hora.

Métrica clave: RMSE ≤ 48 en el conjunto de prueba.

Tipo de problema: Regresión sobre series temporales.

📥 2. Carga y remuestreo de datos
Tareas:

Cargar el dataset y convertir la columna de tiempo a formato datetime.

Establecer la columna de tiempo como índice.

Remuestrear los datos a intervalos de 1 hora (resample('1H')).

Herramientas: pandas, datetime, matplotlib.

🔍 3. Análisis exploratorio (EDA)
Tareas:

Visualizar la serie temporal (tendencias, estacionalidad, outliers).

Analizar correlaciones con variables temporales (hora, día, etc.).

Verificar valores nulos o inconsistencias.

Herramientas: seaborn, plotly, statsmodels, pandas_profiling.

🧠 4. Ingeniería de características
Tareas:

Crear variables como: hora del día, día de la semana, feriados, etc.

Aplicar codificación categórica si es necesario.

Escalar variables si el modelo lo requiere.

Herramientas: scikit-learn, holidays, Feature-engine.

🤖 5. Entrenamiento de modelos
Tareas:

Dividir los datos en entrenamiento (90%) y prueba (10%) sin mezclar el orden temporal.

Entrenar múltiples modelos: LinearRegression, RandomForestRegressor, XGBoost, etc.

Ajustar hiperparámetros con GridSearchCV o RandomizedSearchCV.

Herramientas: scikit-learn, xgboost, lightgbm.

📏 6. Evaluación del modelo
Tareas:

Predecir sobre el conjunto de prueba.

Calcular el RMSE y compararlo con el umbral de 48.

Visualizar errores y analizar si hay patrones en las predicciones fallidas.

Herramientas: mean_squared_error, numpy, matplotlib.

📌 7. Conclusión y recomendaciones
Tareas:

Documentar el modelo con mejor desempeño.

Justificar por qué ese modelo es el más adecuado.

Proponer mejoras futuras (más datos, variables externas, modelos secuenciales como LSTM).
