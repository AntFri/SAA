# One Hot Encoding

# 1: Fundamentos Teóricos
Es un methodo de la libreria pandas para crear un valor numero apartir de un string/character, importante aqui es que varia mucho en comparacion con un map de python porque va dando un valor significativo para la Intelegencia Artificial(IA) importante al momento de entrenar y predecir.

# 2: Análisis Exploratorio de Datos (EDA)
En este ejemplo he mos elegido un dataset que trata sobre precios de casa que can variando dependiendo de la grandaria de la casa y la region en la cual estan. y el objectivo es predecir el precios apartir de la grandaria y el sitio en que estan.
esta en formato csv por lo tanto podemos importar directamente con pandas

# 3: Implementación del Arbol de decision de Clasificacion
1. Despues de cargar el Dataset empezamos directamente con los dummies, con el methodo: **dummies = pd.get_dummies(df_home.town)** le pasamos la columna **town** y de eso nos dara un dataframe con los dummies, creara tantas columans que diferentes variables hay.
2. A continuacion vamos a eleminar una columna de ese Dataframe porque tiene la misma informacion en 2 columnas que en 3 columnas porque tener un **0 0 1** y un **0 0** es lo mismoal para la IA.
3. Luego juntamos con el methodo: **merged = pd.concat([df_home, dummies], axis ='columns')** le pasamos los dos Dataframes y en cual direction los anyade y nos devuelve un dataframe que contiene los datos del dataframe original y los dummies.
4. Por ultimo eliminamos con el methodo: **final = merged.drop(['town'], axis='columns')** pasando le la columna que queremos eliminar y nos devuelve un dataframe sin esa columna.
5. Ahora ya podemos separar los dato en X e y para poder entrenar le IA  y luego predecir los precios de casas.