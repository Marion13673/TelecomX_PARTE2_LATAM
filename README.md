**INTRODUCCIÓN** 🚀
<div align='justify'>
La empresa Telecom X enfrenta una alta tasa de cancelaciones y necesita comprender los factores que llevan a la pérdida de clientes (Churn), por lo tanto, requiere desarrollar modelos predictivos capaces de prever qué clientes tienen mayor probabilidad de cancelar sus servicios.

  
##**Características**## ✨

Se extrae información de un archivo: **"datos_tratados.csv"**, donde los datos provienen del proyecto TelecomX, que han sido corregidos y estandarizados.

Los principales objetivos:

* Preparar los datos para el modelado (tratamiento, codificación, normalización).
* Realizar análisis de correlación y selección de variables.
* Entrenar dos o más modelos de clasificación.
* Evaluar el rendimiento de los modelos con métricas.
* Interpretar los resultados, incluyendo la importancia de las variables.
* Crear una conclusión estratégica señalando los principales factores que influyen en la cancelación.

**DESCRIPCIÓN** 🖌️

Para ello se realiza los siguientes pasos para su extracción, transformación, análisis y conclusión:

* ✅ Eliminación de Columnas Irrelevantes: Eliminar columnas que no aportan valor al análisis o a los modelos predictivos, como identificadores únicos (por ejemplo, el ID del cliente). Estas columnas no ayudan en la predicción de la cancelación y pueden incluso perjudicar el desempeño de los modelos.
  
* ✅ Encoding:Transformar las variables categóricas a formato numérico para hacerlas compatibles con los algoritmos de machine learning. Se Utilizó un método de codificación adecuado, como one-hot encoding.
  
* ✅ Verificación de la Proporción de Cancelación (Churn): Calcular la proporción de clientes que cancelaron en relación con los que permanecieron activos. Evalúa si existe un desbalance entre las clases, ya que esto puede impactar en los modelos predictivos y en el análisis de los resultados.
  
* ✅ Balanceo de Clases:Se aplicó técnicas de balanceo como undersampling o oversampling. En situaciones de fuerte desbalanceo, herramientas como SMOTE son útiles para generar ejemplos sintéticos de la clase minoritaria.

* ✅ Matriz de correlación: Visualizar la matriz de correlación para identificar relaciones entre las variables numéricas. Se Prestó especial atención a las variables que muestran una mayor correlación con la cancelación, ya que estas pueden ser fuertes candidatas para el modelo predictivo.

* ✅ Investigar cómo variables específicas se relacionan con la cancelación, tales como:

    - Tiempo de contrato × Cancelación
    - Gasto total × Cancelación

* ✅ Utilizar gráficos como boxplots o scatter plots para visualizar patrones y posibles tendencias.

* ✅ Dividir el conjunto de datos en entrenamiento y prueba para evaluar el rendimiento del modelo. Una división común es 70% para entrenamiento y 30% para prueba.

* ✅ Después de elegir los modelos, realizar el análisis de las variables más relevantes para la predicción de la cancelación:

Regresión Logística: Investiga los coeficientes de las variables, que muestran su contribución a la predicción de cancelación.

KNN (K-Nearest Neighbors): Observa cómo los vecinos más cercanos influyen en la decisión de clasificación. Las variables más impactantes pueden ser aquellas que más contribuyen a la proximidad entre los puntos de datos.

Random Forest: Utiliza la importancia de las variables proporcionada por el modelo. Random Forest calcula la importancia basándose en cómo cada variable contribuye a la reducción de la impureza durante las divisiones de los árboles.

SVM (Support Vector Machine): En el SVM, las variables más relevantes son aquellas que influyen en la frontera de decisión entre las clases. Puedes analizar los coeficientes de los vectores de soporte para entender qué variables tienen mayor impacto.

Otros Modelos: Dependiendo del modelo elegido, considera el análisis de métricas específicas para comprender la relevancia de las variables. Por ejemplo, coeficientes en modelos lineales, pesos en redes neuronales, o la importancia relativa en técnicas de boosting (como XGBoost).
Conclusión
Descripción
Editar
Elaboren un informe detallado, destacando los factores que más influyen en la cancelación, basándose en las variables seleccionadas y en el rendimiento de cada modelo.

Identifiquen los principales factores que afectan la cancelación de clientes y propongan estrategias de retención basadas en los resultados obtenidos.
















