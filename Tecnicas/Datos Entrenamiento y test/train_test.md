# Datos Entrenamiento y Testing

# 1: Fundamentos Teóricos
La separacion de datos en partes de entrenamiento y testing es muy util para comprobar la precision de nuestro modelo con datos que aun no ha visto nuestro modelo, asi no tenemos que tener 2 csv sino tenemos uno y vamos separando lo dinamicamente.
La funcion escoje aleatoriamente datos del dataset hasta tener el porcentaje que le hemos dicho, esa aleatoridad se puede quitar poniendo:  **random_state=1** eso es como una semilla que siempre va a partir los datos igual, el 1 se puede poner a cualquier valor, importante tiene que serun valor numerico.

# 2: Análisis Exploratorio de Datos (EDA)
En este ejemplo he mos elegido un dataset que trata sobre si una persona ha comprado un seguro o no con la edad que tiene, eso es util para ver cual es el grupo ideal en el mercado.
esta en formato csv por lo tanto podemos importar directamente con pandas

![Data img](https://github.com/AntFri/SAA/blob/main/Tecnicas/Datos%20Entrenamiento%20y%20test/msedge_aJBVLyFv27.png)


# 3: Implementación del Test y Train
1. Leemos y imprimimos el dataset que tenemos
2. con la linea: **from sklearn.model_selection import train_test_split** importamos la libreria des de sklearn
3. A continuacion separamos en X e y que son las variables dependientes e independientes.
4. Luego para separar lo solo tenemos que utilizar la siguiente linea: **X_train, X_test, y_train, y_test = train_test_split(X, y, train_size=0.8)** Lo que esta haciendo es que devulve 4 dataframes con datos esos datos selo pass atravez las dos Cariables X e y y con el **train_size=0.8** hemos definido que el tamanyo de los datos de entreno es del 80% de los datos que le damos.

![BIld](https://github.com/AntFri/SAA/blob/main/Tecnicas/Datos%20Entrenamiento%20y%20test/msedge_mNc9Dj0ANy.png)

5. Por ultimo he imprimodo cada dataframe y he entrenado el model.
