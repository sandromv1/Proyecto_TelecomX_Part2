📊 Proyecto Telecom X - Parte 2
1. Propósito del análisis

El objetivo principal de este proyecto es predecir la cancelación de clientes (churn) en la empresa Telecom X, a partir de un conjunto de variables relevantes relacionadas con el contrato, el tipo de servicio y la facturación.
El análisis busca identificar qué clientes presentan mayor probabilidad de cancelar, con el fin de proponer estrategias de retención y mejorar la gestión del negocio.

2. Estructura del proyecto y organización de los archivos

El proyecto se compone de:

TelecomX_Part2.ipynb: cuaderno principal con todo el flujo de trabajo.
TelecomX_Data.json: arhivo en formato Json que tiene los datos que analizaremos, se puede descargar desde el siguiente link:
https://github.com/alura-cursos/challenge2-data-science-LATAM/blob/main/TelecomX_Data.json


3. Descripción del proceso de preparación de los datos

Clasificación de variables:

Categóricas: tipo de contrato, método de pago, servicio de internet, etc.

Numéricas: meses de contrato, cargos mensuales, cargos totales.

Transformaciones aplicadas:

Codificación de variables categóricas mediante OneHotEncoder.

Normalización de variables numéricas usando Min-Max Scaling (fundamental para KNN).

Balanceo de clases:

Se aplicó SMOTE para oversampling de la clase minoritaria (clientes que cancelan).

También se probó NearMiss (undersampling), aunque con resultados menos favorables.

Separación de datos:

Datos divididos en train y test, asegurando proporción balanceada de la variable objetivo.

Justificación de decisiones:

La normalización se aplicó exclusivamente para KNN, ya que este modelo depende de distancias.

El uso de oversampling se priorizó por mejorar el recall de la clase positiva.

4. Ejemplos de gráficos e insights obtenidos

Distribución de cancelaciones (Churn): confirmó un desbalance de clases, con más clientes que permanecen que los que cancelan.

Matriz de confusión:

Árbol de decisión: alto desempeño en la clase negativa, bajo en la positiva.

KNN: mejor recall para la clase positiva, aunque con menor exactitud global.

Importancia de variables:

Meses_Contrato, tipo de plan y cargos mensuales destacan como factores clave para explicar la cancelación.

5. Instrucciones para ejecutar el cuaderno

- Clonar este repositorio o descargar los archivos.

- Abrir el cuaderno TelecomX_Part2.ipynb en Google Colab o VSCode.

✅ Conclusión

Tras la comparación de modelos, se determinó que KNN con oversampling y normalización Min-Max es la mejor opción para predecir cancelaciones. Aunque no logra la mayor exactitud global, ofrece un mejor recall en la clase positiva, lo cual es crítico para identificar clientes en riesgo y diseñar estrategias de retención.
