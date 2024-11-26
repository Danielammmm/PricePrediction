# PricePrediction
# **Predicción de Precios de Venta de Vehículos**

## **Descripción**
Este proyecto tiene como objetivo desarrollar un modelo predictivo para estimar los precios de venta de vehículos utilizando un enfoque basado en machine learning. El pipeline abarca desde la limpieza y preparación de datos hasta la implementación y evaluación de modelos avanzados para minimizar el error de predicción.

## **Estructura del Proyecto**
1. **`Proyecto_2_limpieza_de_datos.ipynb`:**  
   Incluye las etapas principales del preprocesamiento, tales como:
   - Identificación y tratamiento de datos faltantes.
   - Detección y manejo de outliers.
   - Transformación de variables categóricas en numéricas.
   - Escalado y normalización de los datos.

2. **`Mejores_intentos.ipynb`:**  
   Documenta experimentos y evaluaciones de modelos predictivos basados en los datos preprocesados. Detalla:
   - Selección de características relevantes.
   - Comparación de modelos como XGBoost, LightGBM y Random Forest.
   - Optimización de hiperparámetros y evaluación del rendimiento.

## **Componentes principales**
### **1. Limpieza de Datos**
Las tareas clave realizadas en `Proyecto_2_limpieza_de_datos.ipynb` incluyen:
- **Tratamiento de datos faltantes:**
  - Imputación con la media, mediana o valores específicos según el contexto.
- **Manejo de outliers:**
  - Identificación visual con gráficos como boxplots.
  - Transformaciones para normalizar distribuciones.
- **Codificación de variables categóricas:**
  - Uso de técnicas como One-Hot Encoding y Label Encoding.
- **Escalado:**
  - Normalización con Min-Max Scaler y estandarización con StandardScaler.

### **2. Modelado Predictivo**
En `Mejores_intentos.ipynb`, se implementan y evalúan modelos como:
- **Regresión Lineal:** Modelo base para comparación.
- **XGBoost:** Modelo principal que logra el menor error.
- **Random Forest:** Para manejo de datos con relaciones no lineales.
- **LightGBM:** Optimización eficiente para grandes datasets.

### **3. Evaluación**
- Métrica principal: **RMSE (Root Mean Squared Error).**
- Mejor RMSE alcanzado: ~8431 en el conjunto de entrenamiento con un modelo **XGBoost** optimizado.

## **Resultados principales**
- Identificación de las variables más relevantes para la predicción, como:
  - `engine_size`
  - `curb_weight`
  - `horsepower`
  - `highway_mpg`
- Reducción significativa del RMSE tras la limpieza y selección de características.

## **Cómo usar este proyecto**
1. **Instala las dependencias:**
   Asegúrate de tener las librerías necesarias instaladas:
   ```bash
   pip install pandas numpy scikit-learn matplotlib seaborn xgboost lightgbm
