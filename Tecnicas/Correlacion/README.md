# Correlacion

# 1: Fundamentos Teóricos
La Correlacion sirve para calcular la dependencia entre cada variable en el dataframe. En este caso hemos utilizado un dataset que trata sobre los ataques/disparos en colegios/institutos en estados unidos y cunatos han muerto y cuantos han sido heridos.
Sus limitaciones son cuando se intenta sacar una relacion de variables que contienen strings, solo funciona con valores numericos.

# 2: Análisis Exploratorio de Datos (EDA)
En este ejemplo he mos elegido un dataset que trata sobre los ataques/disparos en institutos/colegios en estados unidos, solo vamos a ver la relacion entre las muestes y los heridos para este ejemplo pero con OHE se podria utilizar tambien la resta de valores.
esta en formato csv por lo tanto podemos importar directamente con pandas

# 3: Implementación de la Correlacion
1. Hemos importado el dataset con Pandas imprimido para ver todos los datos y la cantidad total de filas
2. luego con la funcion: **corr_matrix = df.corr()** creamos una matriz de correlacion que luego con la libreria **Matplotlib** se puede representar
3. por ultimo con la funcion: **sns.heatmap(corr_matrix, annot=True, cmap='coolwarm', ax=ax)** representamos y configuramso un mapa de calor que nos sirve para representar la matriz de correlacion. 

![Corr img](https://github.com/AntFri/SAA/blob/main/Tecnicas/Correlacion/msedge_n9yv3rGM0k.png)
