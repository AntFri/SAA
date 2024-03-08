# Regresion Logistica

# 1: Fundamentos Teóricos
La Regresion logistica es un modelo para predecir valores categoricas dependiendo de los datos entrenados y dados, los cuales tienen que ser valores numericos. Eso al mismo tiempo es un incoveninte de la regresion Logistica, hay que tranformar todos los valores categoricos a numeros para poder predecir y luego para tener una predicion entendible tranformar lo a las categorias otravez.

# 2: Análisis Exploratorio de Datos (EDA)
En este ejemplo he mos elegido un dataset que trata sobre si una persona ha comprado un seguro o no con la edad que tiene, eso es util para ver cual es el grupo ideal en el mercado.
esta en formato csv por lo tanto podemos importar directamente con pandas

![Data img](https://github.com/AntFri/SAA/blob/main/Tecnicas/Datos%20Entrenamiento%20y%20test/msedge_aJBVLyFv27.png)


# 3: Implementación de datos entrenamiento y testing
1. Importamos el dataset des de un csv y lo imprimimos, tambien representamos un grafico para ver n poco la correlacion
2. Luego lo separamos en test y train para poder comprobar si nuestro modelo esta bien entrenado
3. Representamos todas las tablas de test y train
4. A continuacion creamos un modelo con: **model = LogisticRegression()**

![model create img](https://github.com/AntFri/SAA/blob/main/Aprendizaje%20Supervisado/Clasificaci%C3%B3n/Regresion%20Logistica/msedge_EeNM4HOzao.png)

5. Despues entrenamos el modelo con: **model.fit(X_train, y_train)** con los valores train de la separacion

![model fit](https://github.com/AntFri/SAA/blob/main/Aprendizaje%20Supervisado/Clasificaci%C3%B3n/Regresion%20Logistica/msedge_ASwy6RYlRE.png)

6. Por ultimo hacemos una predicion con: **y_predict = model.predict(X_test)** eso nos permite comprobar nuestro modelo.

![model predict](https://github.com/AntFri/SAA/blob/main/Aprendizaje%20Supervisado/Clasificaci%C3%B3n/Regresion%20Logistica/msedge_SIotE6UKIN.png)

7. Comprobamos la precision: **model.score(X_test, y_test)** y nos da un 83,3% de precision

![model score](https://github.com/AntFri/SAA/blob/main/Aprendizaje%20Supervisado/Clasificaci%C3%B3n/Regresion%20Logistica/msedge_miSIsjJZpU.png)
