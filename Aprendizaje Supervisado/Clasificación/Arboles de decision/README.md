# Arbol de desicion clasificacion

# 1: Fundamentos Teóricos
EL Arbol de Decision de clasificacion sirve para categorizar los datos apartir de ciertos valor en este ejemplo era que si tienen un salario major de 100k apartir de los valore categoricos, si tiene un master, cual company trabaja, etc.
Sus limitaciones son cuando se trabaja con se quieres predecir valores numerocos y no categorias, para valores numerico estael Arbol de decision de regression.

# 2: Análisis Exploratorio de Datos (EDA)
En este ejemplo he mos elegido un dataset que trata sobre trabajadores que ganan mas de 100k$ al anyo en ciertas companias con diferentes titulos, es un dataset simple pero con variedad para representar las posibilidades del arbold de decision
esta en formato csv por lo tanto podemos importar directamente con pandas

![Data Import](https://github.com/AntFri/SAA/blob/main/Aprendizaje%20Supervisado/Clasificaci%C3%B3n/Arboles%20de%20decision/msedge_3xKMMEhXZq.png)

# 3: Implementación del Arbol de decision de Clasificacion
1. EN este Dataset teniamos que hacer un cambio en las variables dependientes para que podamos entrenar el Arbol de decisiones, eso lo hecho con el LabelEncoder que codifica el string a un numero y he cambiado todo asi a numeros

![label Encoder img](https://github.com/AntFri/SAA/blob/main/Aprendizaje%20Supervisado/Clasificaci%C3%B3n/Arboles%20de%20decision/msedge_ccz8F7pEfN.png)

2. Despues de introducir todos los numeros he eleminado(drop) las columnas con strings para tener und dataframe limpio y organizado.

![drop img](https://github.com/AntFri/SAA/blob/main/Aprendizaje%20Supervisado/Clasificaci%C3%B3n/Arboles%20de%20decision/msedge_eO5Kj58S2W.png)

3. Luego he creado el modelo con: **model = tree.DecisionTreeClassifier()** y lo he entrenado con la funcion: **model.fit(inputs_n, target)** el input_n son las variables dependientes y target los independientes que son los datos del dataframe

![model fit](https://github.com/AntFri/SAA/blob/main/Aprendizaje%20Supervisado/Clasificaci%C3%B3n/Arboles%20de%20decision/msedge_gyF3Je3v3N.png)

4. Por ultimo he comprobado que precision nos da nuestro modelo con la funcion: **model.score(inputs_n, target)**

![model score](https://github.com/AntFri/SAA/blob/main/Aprendizaje%20Supervisado/Clasificaci%C3%B3n/Arboles%20de%20decision/msedge_BJrEB8XrN3.png)
