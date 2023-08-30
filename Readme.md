# Proyecto Estudio de Mercado Automotriz  -  Diosa Medina  - Analista de Datos
​
¡Bienvenidos al proyecto! Durante estos días estoy poniendo en práctica mis habilidades en el campo del análisis de datos. Debo explorar bien los datos, entender la problemática, preparar los datos, para luego experimentar con los modelos de machine learning, usando las métricas correspondientes para medir la performance de los mismos.


### **Planteamiento de la problemática**
​
Asumiré que he sido contratada en el equipo de ciencias de datos de una consultora de renombre. Que me han asignado a un proyecto de estudio de mercado de una importante automotriz china. Nuestro cliente desea ingresar a nuestro mercado de automóviles, por lo que nos ha encomendado analizar las características de los vehículos presentes en el mercado actual. Dado que tienen en su catálogo una amplia colección de modelos de todo tipo, cuyo catálogo está estratificado en gamas según el gusto de cada región, desean saber qué características presentan los vehículos de gama alta y los de gama baja en nuestro mercado, para poder abarcar todo los públicos objetivos ajustándose a toda la demanda y, en base a estos datos, poder cotizar correctamente los vehículos que ofrecerá. 

Para ello, nuestro departamento de datos ha recopilado precios y características de varios de los modelos de vehículos disponibles en nuestro mercado, junto con sus precios de venta al público. Y han armado el siguiente diccionario de datos:


![DiccionarioDatos](https://github.com/jdeiloff/Proyecto-Integrador-M6/raw/main/dic_pi2.jpg)


Nuestro Data Lead me ha recomendado que analice detalladamente los datos, los preprocese debidamente y que diseñe dos modelos predictivos, uno para el precio y otro para distinguir vehículos de gama alta y de gama baja, utilizando la mediana de los precios como punto de corte. 

​
### **Análisis exploratorio de datos, Preparación de datos, Modelamiento y evaluación**
​​
El mercado automotor esta muy ligado a la cultura de cada país, según los gustos de cada uno, el mercado norteamericano, por ejemplo, valora mucho los motores y vehículos muy grandes, el mercado europeo prefiere el bajo consumo, el mercado latinoamericano, los precios finales bajos y asi varía según región, país, nivel socioeconómico y cultura. Un mismo vehículo puede tener un valor muy distinto de un pais al otro, y no solo por los impuestos o costos de producción, sino por cómo cotiza el modelo en el mercado. 

Para la ejecución de este proyecto he utilizado el Lenguaje de Programación Python y algunas de sus librerías, como la librería pandas; la librería numpy; la librería matplotlib con su módulo pyplot; la librería Seaborn; la librería sklearn con sus módulos linear_model (con sus métodos: LinearRegression y LogisticRegression), model_selection (con su método train_test_split), metrics (con sus métodos: r2_score, mean_squared_error y classification_report) y preprocessing (con su método StandarScaler).  

Para el análisis exproratorio y preparación de los datos he utilizado tablas de contingencia que muestran el número de vehículos para las diferentes características que presentan; así como tablas pivote que muestran el precio promedio de los autos para estas características. También, utilicé un pairplot y un análisis de correlación con su correspondiente mapa de calor para determinar el grado de asociación entre las variables numéricas y cuáles de éstas correlaconan con el precio de los vehículos, y de esta manera seleccionar las variables que se utilizan en los modelos de predicción y de clasificación. Además, utilicé gráficas como histogramas con curva de densidad y diagramas de caja y bigotes, que muestran el comportamiento de estas variables a lo largo de su distribución y la existencia o no de valores outliers.

Aparte del análisis detallado de la exploración y preparación de los datos, he considerado para el modelamiento y evaluación, las dos predicciones posibles que les interesaría analizar, por un lado para predecir el precio final de los vehículos y por el otro para clasificar el precio de los vehículos en baratos o gama baja y caros o gama alta:

1. Implementar un modelo de regresión con aprendizaje supervisado que permita predecir el precio final de los vehículos, utilizando los datos que se han puesto a mi disposición.  Para ello he utilizado el Modelo de Regresión Lineal Múltiple, con su correspondiente evaluación de la performance.

2. Implementar un modelo de clasificación con aprendizaje supervisado que permita clasificar el precio de los vehículos en baratos y caros usando la mediana de los precios como punto de corte, utilizando los datos que se han puesto a mi disposición.  Para ello, he utilizado el Modelo de Regresión Logística, con su correspondiente evaluación de la performance.

Todo esto se encuentra en el Jupyter Notebook:  Proyecto_estudioMercAutom.ipynb