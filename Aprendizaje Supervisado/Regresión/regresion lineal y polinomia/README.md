# Regression Lineal

# 1: Fundamentos Teóricos
La regression lineal sirve para poder predicir valores numericos(decimales, enteros) apartir de un entrenamiento previo con valores similares/en el rango. 
Las limitaciones son cuando se quieres predecir categorias o si el modelo entrenado tiene overfitting o underfitting por eso es importante tener un variedad de datos que esten mescladas dependiendo de que tipo de datos es.

# 2: Análisis Exploratorio de Datos (EDA)
En este ejemplo he mos elegido un dataset que trata sobre precios de casas apartir del tamanyo que tenga, es un ejemplo perfecto por que pueden salir valores decimales y enteros dependiendo del tamanyo de la casa
El dataset esta creado en el codigo directamente asique solo creamos und datafram con eso, tambien se podria importar des de un csv directamente con pandas.

![data import](https://github.com/AntFri/SAA/blob/main/Aprendizaje%20Supervisado/Regresi%C3%B3n/regresion%20lineal%20y%20polinomia/msedge_zBjcLFOfA5.png)

# 3: Implementación de la Regression Lineal
1. Primero he visualizado los valores del dataset con la libreria Matplotlib para ver como se van evolucionando

![grapgh img](https://github.com/AntFri/SAA/blob/main/Aprendizaje%20Supervisado/Regresi%C3%B3n/regresion%20lineal%20y%20polinomia/msedge_eAWd9qan4W.png)

2. Despues visualizar los datos los separasmo a X i Y para luego poder entrenar el modelo.

![x y sep img](https://github.com/AntFri/SAA/blob/main/Aprendizaje%20Supervisado/Regresi%C3%B3n/regresion%20lineal%20y%20polinomia/msedge_7THumbhZhj.png)


3. Luego he creado el modelo con: **model = linear_model.LinearRegression()** y lo he entrenado con la funcion: **model.fit(X,y)** el X son las variables dependientes i y los independientes que son los datos del dataframe

![model img](https://github.com/AntFri/SAA/blob/main/Aprendizaje%20Supervisado/Regresi%C3%B3n/regresion%20lineal%20y%20polinomia/msedge_uqjmrpy3vE.png)

4. Por ultimo hago una predicion con la funcion: **model.predict(X)**

![predict model img](https://github.com/AntFri/SAA/blob/main/Aprendizaje%20Supervisado/Regresi%C3%B3n/regresion%20lineal%20y%20polinomia/msedge_spawu6D02J.png)
