# Proyecto de Machine Learning para el Consumo Eléctrico

## Descripción

Este proyecto utiliza un dataset de consumo eléctrico para desarrollar y evaluar modelos de machine learning con el objetivo de predecir el consumo futuro. El notebook incluye un análisis exploratorio de los datos (EDA), visualización de series de tiempo y la implementación de varios algoritmos de predicción.

## Características

* **Carga y Exploración de Datos (EDA):** Carga de datos de entrenamiento y prueba, conversión de fechas y análisis descriptivo inicial.
* **Visualización de Datos:** Gráficos del consumo eléctrico total y por subestación para entender tendencias y patrones.
* **Análisis de Series de Tiempo:**
    * Test de Dickey-Fuller Aumentado para verificar la estacionariedad de las series.
    * Gráficos de autocorrelación (ACF y PACF) para identificar la estructura de la serie de tiempo.
* **Modelos de Machine Learning:**
    * SARIMAX
    * XGBoost
    * Redes Neuronales Recurrentes (LSTM)
* **Evaluación de Modelos:** Comparación del rendimiento de los modelos utilizando métricas como MAE, MSE, RMSE y R2-Score.
* **Persistencia de Modelos:** Uso de `pickle` para guardar y cargar los modelos entrenados.

## Guía de Instalación

Sigue estos pasos para tener el proyecto corriendo en tu máquina local.

### Prerrequisitos

Asegúrate de tener instalado lo siguiente:
* Python 3.8 o superior
* pip (manejador de paquetes de Python)
* Jupyter Notebook o JupyterLab

### 1. Clonar el Repositorio

bash
git clone <URL-DEL-REPOSITORIO> cd <NOMBRE-DEL-DIRECTORIO>

### 2. Crear un Entorno Virtual (Recomendado)

python -m venv venv
source venv/bin/activate  # En Windows usa `venv\Scripts\activate`

### 3. Instalar Dependencias
Este proyecto requiere las siguientes librerías de Python. Puedes instalarlas usando pip:

pip install pandas numpy matplotlib scikit-learn xgboost tensorflow seaborn statsmodels

O, si se proporciona un archivo requirements.txt:

pip install -r requirements.txt

### 4. Estructura de Directorios
Asegúrate de que los datos estén en la siguiente estructura de directorios dentro del proyecto:

.
├── Dataset/
│   ├── train.csv
│   └── test.csv
├── Gráfico_de_Autocorrelación/
├── Proyecto_II_Consumo_Electrico.ipynb
└── README.md

### 5. Ejecutar el Notebook

Finalmente, inicia Jupyter Notebook o JupyterLab y abre el archivo Proyecto_II_Consumo_Electrico.ipynb.

jupyter notebook

