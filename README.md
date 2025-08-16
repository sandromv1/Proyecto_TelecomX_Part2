📊 Proyecto Telecom X
1. Propósito del Análisis

El objetivo de este proyecto es analizar el comportamiento de los clientes de Telecom X con el fin de predecir la cancelación del servicio (churn). Para ello, se aplicaron técnicas de procesamiento de datos, análisis exploratorio y modelado predictivo utilizando distintos algoritmos de machine learning. Finalmente, se seleccionó el modelo KNN con oversampling por su mejor capacidad para identificar a los clientes con mayor riesgo de cancelar, lo que aporta un valor estratégico para diseñar campañas de retención.

2. Estructura del Proyecto

El proyecto está organizado en un notebook principal:

Extracción y transformación de datos: limpieza, estandarización, encoding.

Análisis exploratorio: estadísticas descriptivas, distribución de variables, correlaciones.

Modelado predictivo: comparación de algoritmos (Decision Tree y KNN) con técnicas de balanceo de clases.

Evaluación de modelos: métricas de desempeño (accuracy, precision, recall, F1-score), matrices de confusión e intervalos de confianza.

Importancia de variables: interpretación de factores relevantes para la predicción del churn.

Conclusiones: selección de KNN como modelo final.

3. Ejemplos de Gráficos e Insights

🔹 Distribución de cancelaciones: mostró el desbalance de clases (más clientes que permanecen que los que cancelan).
🔹 Matriz de confusión: evidenció que KNN, aunque con menor exactitud global, detecta mejor a los clientes que cancelan.
🔹 Gráficos de importancia de variables: identificaron que Meses_Contrato, el tipo de plan y los pagos mensuales son factores clave en la predicción.

Ejemplo de insight:
👉 Los clientes con contratos más cortos y pagos mensuales elevados tienen mayor probabilidad de cancelar.

4. Instrucciones para Ejecutar el Notebook

Clonar este repositorio o descargar el archivo TelecomX_Part2.ipynb.

(entre las librerías principales se incluyen: pandas, numpy, matplotlib, seaborn, scikit-learn, imblearn).

Abrir el notebook en VSCode o Google Colab y ejecutar las celdas en orden.

Opcional: actualizar la ruta del dataset si fuese necesario.

📌 Conclusión

Este proyecto demuestra cómo aplicar técnicas de machine learning al sector de telecomunicaciones para reducir la tasa de cancelación de clientes. La documentación y estructura del análisis permiten replicar el flujo de trabajo y extenderlo con nuevos modelos o datasets en el futuro.
