# **SVM (Support Verctor Machine**

Después  de ver el video, busca e indica que son:
Adecuado cuando tenemos pocos datos, muchas características y en conjunto con redes neuronales.

- **Vectores de soporte:**
Son los puntos que se encuentra mas cerca al hiperplano y influyen directamente en su orientacion y posicion

- **Hiperplano:**
Es el objectivo al cual se quiere llegar para separar de la mejor forma dos clases, en un espacio bidimencional es una linea en un espacio tridimencional es es un plano.

- **Hard Margin:**
Es el margen maximo posible cuando se quiere separar dos clases con el hiperplano.
  
- **Soft Margin:**
El margen permite un rango de mal clasisficacion para poder generalizar mejor las clases y no tener overfiting.

- **Kernel, tipos:**
  - Lineal: Se utiliza en datos que se pueden separa linealmente.
  - Polinomico: Util para separaciones no lineales y para problemas en que las relaciones entre las caracteristicas son polinomico.
  - RBF o Gaussiana: Se utiliza para problemas en que las relaciones entre las caracteristicas no son lineal.

- **Para que tipo de problemas es adecuada (pon ejemplos), para cuales no.**
  - Adecuado: Muy utili en el procesamiento del lenguaje natural (NLP), reconocimiento de imagenes y voz. Un ejemplo mas especifico seria la classificacion de correos electronico si son spam o no.
  - NO Adecuado: Para conjuntod de datos grandes por la complejidad cuadratica del SVM, tambien depende mucho de la escala de datos, se tendria que ajustar entre 0-1.
