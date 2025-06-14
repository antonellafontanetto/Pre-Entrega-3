# 🛢️ Proyecto 4x4 YPF - Análisis de Vaca Muerta
# Pre-Entrega 3 - Data Science
# Grupo 3 - Fundación YPF / Programa Ingenias+

# Introducción

El proyecto 4x4 de YPF tiene como objemtivo principal cuadruplicar la producción de la compañía en los próximos 4 años, enfocándose en la eficiencia operativa, la generación de valor y la concentración de esfuerzos en los activos más rentables a corto plazo, como Vaca Muerta, la principal cuenca petrolera del país.

Este trabajo busca analizar el crecimiento de la producción de petróleo y gas en la cuenca neuquina desde el año 2021 en adelante, considerando exclusivamente los datos correspondientes a YPF S.A.. El análisis se basa en indicadores clave como la producción no convencional, las principales 5 áreas de concesiones y el subtipo de recurso producido, ya sea shale o tight en los últimos años.

En el análisis, se busca aportar evidencia empírica sobre la evolución y proyección del potencial de expansión de YPF en Vaca Muerta, en línea con los objetivos planteados en su plan estratégico 4x4.

# Objetivo

El objetivo del proyecto es analizar y predecir el crecimiento de la producción de petróleo y gas por parte de YPF S.A. en la cuenca neuquina, evaluando el impacto de diferentes variables relacionadas con la actividad extractiva y operativa.

# Integrantes - Grupo 3

Este proyecto fue desarrollado por el Grupo 3 del curso de Data Science de Fundación YPF en el marco del programa Ingenias+, que busca incorporar más mujeres al mundo de la programación.

* Cyntia Nasabun – Diplomada en Análisis de Datos e IA, IFES, Neuquén. 

* Antonella Fontanetto – Licenciada en Economía, Universidad de Buenos Aires

# Datasets utilizados

Los datos provienen de fuentes públicas oficiales del Gobierno Nacional y de la Provincia del Neuquén:

* Producción de Pozos de Petróleo y Gas http://datos.energia.gob.ar/dataset/produccion-de-petroleo-y-gas-por-pozo

Mapas y documentos complementarios:

* Mapa Energía Río Negro https://mapa.rionegro.com.ar/energia

* Distribución de Fluidos – Energía Neuquén https://www.energianeuquen.gob.ar/distribucion-de-fluidos/

* Línea estratégica YPF 4x4 https://www.rystadenergy.com/news/vaca-muerta-smashes-crude-output-record-in-3q

* Presentación IR Day 2025 – YPF https://inversores.ypf.com/documents/presentaciones/YPF-IR-DAY-2025-presentation.pdf

* YPF – Mayo 2024 – IAméricas https://iamericas.org/2024/05/YPF_Horacio-Marin_Mesa-Redonda_Mayo-8-presentation.pdf

* Análisis potencial exportador de Vaca Muerta – La Nación  https://www.lanacion.com.ar/el-potencial-exportador-vaca-muerta-el-planparaalcanzarlos30milmillonesdedolares

# Estructura del repositorio

📁

├── data/           # Datasets originales y procesados

├── notebooks/      # Notebooks (diferentes versiones estudiadas)

├── README.md       # Este archivo

# Metodología

La metodología implementada en el proyecto está relacionada con la búsqueda minuciosa de información relevante para el desarrollo del mismo, en función de las respuestas a nuestro modelo predictivo. Teniendo como eje principal la proyección de la producción de petróleo y gas en Vaca Muerta por parte de YPF S.A. para los próximos años.

En el análisis se implementaron varios modelos de aprendizaje supervisado, es decir, modelos que aprenden de datos etiquetados del pasado para luego hacer predicciones, de esta manera estos modelos nos permiten dar soporte a decisiones estratégicas para la compañía.

Los modelos utilizados fueron:

* Regresión Lineal: La regresión lineal es un modelo supervisado que predice un valor numérico continuo a partir de una o más variables independientes, asumiendo una relación lineal entre ellas. Su función principal es estimar la tendencia de los datos y realizar predicciones cuantitativas.

* Random Forest: Random Forest es un modelo supervisado basado en múltiples árboles de decisión que trabajan en conjunto para mejorar la precisión y evitar el sobreajuste. Funciona combinando las predicciones de varios árboles para obtener un resultado más robusto y confiable.

* Support Vector Machine: es un modelo supervisado que busca encontrar el hiperplano óptimo que separa las clases en un espacio de características. Es especialmente eficaz en problemas de clasificación, incluso cuando los datos no son linealmente separables.

* XGBoost: XGBoost es un modelo supervisado de tipo boosting que construye árboles de decisión de manera secuencial para mejorar el rendimiento en cada iteración. Es altamente eficiente, preciso y muy utilizado en competencias y proyectos de machine learning por su capacidad para manejar grandes volúmenes de datos y prevenir el sobreajuste.

* Prophet: es un modelo supervisado desarrollado por Facebook para realizar pronósticos de series temporales de forma automática y precisa. Es ideal para datos con tendencias, estacionalidades y eventos especiales, y permite a usuarios no expertos hacer predicciones fácilmente.

Además por cada modelo se implementó la utilización y cálculo de métricas para corroborar que tan bien el modelo podía predecir nuestro objetivo. Las métricas utilizadas fueron:

* MAE (Error Absoluto Medio):
Mide el promedio de las diferencias absolutas entre los valores reales y los predichos.
Indica cuánto se equivoca en promedio el modelo, sin considerar la dirección del error.

* MSE (Error Cuadrático Medio):
Calcula el promedio de los errores al cuadrado entre valores reales y predichos.
Penaliza más los errores grandes, siendo útil para detectar desviaciones fuertes.

* R² (Coeficiente de determinación):
Indica qué proporción de la variabilidad en los datos es explicada por el modelo.
Un valor cercano a 1 significa que el modelo ajusta bien los datos.

# Herramientas utilizadas 

Lenguaje: Python 3.10+

Librerías:

Tercera entrega

* Análisis exploratorio de datos: Nunpy, Pandas

* Modelado: RandomForestRegressor,SVR, XGBRegressor,GridSearchCV, MultiOutputRegressor, Prophet, train_test_split, mean_absolute_error

* Visualización: matplotlib, seaborn, plotly, contextily, scipy

* Otros: jupyter, openpyxl, google colab, GitHub
