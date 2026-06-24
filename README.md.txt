Markdown
# Sistema Multiclase de Predicción de Riesgo de Diabetes

Este repositorio contiene la arquitectura analítica avanzada desarrollada en Python y el cuadro de mando interactivo en Power BI para la detección temprana y simulación epidemiológica del riesgo de diabetes, utilizando el dataset BRFSS 2015 del CDC (253,680 registros).

## 📁 Estructura del Repositorio

* `data/` : Espacio destinado para el almacenamiento local del dataset crudo del CDC.
* `notebooks_scripts/` : Módulos secuenciales en Python para el pipeline de ciencia de datos.
  * `01_preprocesamiento.py` : Limpieza, balanceo y codificación de variables.
  * `02_entrenamiento_comparativo.py` : Modelado analítico (Softmax, XGBoost, MLP).
  * `03_explicabilidad_y_validacion.py` : Extracción de valores SHAP y Validación Cruzada (K=5).
* `dashboard/` : Archivo `.pbix` con la interfaz interactiva desarrollada en Power BI.
* `outputs/` : Almacenamiento de artefactos visuales y gráficos analíticos exportados.
* `requirements.txt` : Archivo de gobernanza y congelamiento de dependencias del entorno.

## 🚀 Instrucciones de Replicación

1. **Clonar o descargar** este repositorio en su estación de trabajo local.
2. **Configurar el entorno virtual:** Desde la consola de Anaconda, instalar las versiones exactas de las librerías ejecutando:
```bash
   pip install -r requirements.txt