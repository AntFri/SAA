# Datos Entrenamiento y Testing

# 1: Fundamentos Teóricos
EL Arbol de Decision de clasificacion sirve para categorizar los datos apartir de ciertos valor en este ejemplo era que si tienen un salario major de 100k apartir de los valore categoricos, si tiene un master, cual company trabaja, etc.
Sus limitaciones son cuando se trabaja con se quieres predecir valores numerocos y no categorias, para valores numerico estael Arbol de decision de regression.

# 2: Análisis Exploratorio de Datos (EDA)
En este ejemplo he mos elegido un dataset que trata sobre trabajadores que ganan mas de 100k$ al anyo en ciertas companias con diferentes titulos, es un dataset simple pero con variedad para representar las posibilidades del arbold de decision
esta en formato csv por lo tanto podemos importar directamente con pandas

![Data img](https://github.com/AntFri/SAA/blob/main/Tecnicas/Datos%20Entrenamiento%20y%20test/msedge_aJBVLyFv27.png)


# 3: Implementación del Arbol de decision de Clasificacion
1. Leemos y imprimimos el dataset que tenemos
2. con la linea: **from sklearn.model_selection import train_test_split** importamos la libreria des de sklearn
3. A continuacion separamos en X e y que son las variables dependientes e independientes.
4. Luego para separar lo solo tenemos que utilizar la siguiente linea: **X_train, X_test, y_train, y_test = train_test_split(X, y, train_size=0.8)** Lo que esta haciendo es que devulve 4 dataframes con datos esos datos selo pass atravez las dos Cariables X e y y con el **train_size=0.8** hemos definido que el tamanyo de los datos de entreno es del 80% de los datos que le damos.
![BIld](https://github.com/AntFri/SAA/blob/main/Tecnicas/Datos%20Entrenamiento%20y%20test/msedge_mNc9Dj0ANy.png)
5. Por ultimo he imprimodo cada dataframe y he entrenado el model. 
