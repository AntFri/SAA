# Arbol de decision Regression

# 1: Fundamentos Teóricos
EL Arbol de Decision de Regresion sirve para predecir valores numeriocos y categorizar un cierta cantidad datos. Para eso tienen que estar los valores utilizados para predecir y los objectivos en valores numericos
Sus limitaciones son cuando se quiere predecir valores categoricos y no numericos, para valores Categoricos se utiliza el Arbol de decision de Clasificacion.

# 2: Análisis Exploratorio de Datos (EDA)
En este ejemplo he mos elegido un dataset que trata sobre peliculas y tiene muchos valores, el valor objectivo o y es Collections, luego los valores dependdientes o X son entre otros, el genero, el rating, cuanto han tardado en producir, cuantos han visto el trailer, etc
esta en formato csv por lo tanto podemos importar directamente con pandas

![data import img](https://github.com/AntFri/SAA/blob/main/Aprendizaje%20Supervisado/Regresi%C3%B3n/Arbol%20de%20decision/msedge_D9nLSzYu8F.png)

# 3: Implementación del Arbol de decision de Regression
1. EN este Dataset teniamos que hacer un cambio en las variables dependientes para que podamos entrenar el Arbol de decision, eso lo hecho utilizando dummies de pandas, el **drop_first=True** nos permite eliminar las columans de string antes de anyadir las columnas creadas por pandas.

![model tree img ](https://github.com/AntFri/SAA/blob/main/Aprendizaje%20Supervisado/Regresi%C3%B3n/Arbol%20de%20decision/msedge_HsYuuU8Wpv.png)

2. Despues de introducir todos los numeros he separado el dataframe en X e y pera luego separar lo en Test y train.

![test train img](https://github.com/AntFri/SAA/blob/main/Aprendizaje%20Supervisado/Regresi%C3%B3n/Arbol%20de%20decision/msedge_3QB1wtkW3q.png)

3. Luego he creado el modelo con: **regtree = tree.DecisionTreeRegressor(max_depth=3)** y lo he entrenado con la funcion: **regtree.fit(X_train, y_train)**.

![fit model img](https://github.com/AntFri/SAA/blob/main/Aprendizaje%20Supervisado/Regresi%C3%B3n/Arbol%20de%20decision/msedge_otdNLWxxFT.png)

4. He predecido con: **y_test_pred = regtree.predict(X_test)** los valores de test para poder haver un score de la libreria sklearn

![predict model img](https://github.com/AntFri/SAA/blob/main/Aprendizaje%20Supervisado/Regresi%C3%B3n/Arbol%20de%20decision/msedge_VYgnHBEnl2.png)

5. Por ultimo he comprobado que precision nos da nuestro modelo con la funcion: **r2_score(y_test, y_test_pred)**

![score model img](https://github.com/AntFri/SAA/blob/main/Aprendizaje%20Supervisado/Regresi%C3%B3n/Arbol%20de%20decision/msedge_EGM6zloi6G.png)
