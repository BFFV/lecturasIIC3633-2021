### Review: Sistemas Recomendadores Basados en Deep Learning: Un Estudio y Nuevas Perspectivas

El paper trata sobre el gran potencial del área del Deep Learning aplicada a los sistemas recomendadores. Se hace una revisión general del estado del arte en estos temas (al menos hasta el 2019), explicando porqué NO existe casi ninguna razón para evitar el uso de estas técnicas en cualquier sistema recomendador de hoy en día.

Las posibles mejoras que entrega el uso de Deep Learning son las siguientes:

* La no linealidad representa mejor las interacciones entre usuarios e ítems que los modelos clásicos (lineales), y el contenido es claramente mejor representado usando Computer Vision (imágenes y videos) y NLP (textos), a diferencia de las representaciones humanas utilizadas en los sistemas content based.
* La generación/extracción de características automática ahorra mucho trabajo, y permite representar mejor la información utilizando el input mismo que reciben los modelos.
* La información secuencial de las interacciones a través del tiempo son perfectas para modelos CNN y RNN, que destacan en su rendimiento al modelar este tipo de datos.
* Gran extensibilidad gracias a frameworks que permiten combinar y trabajar con módulos de redes neuronales.

Algunas críticas al uso de estos modelos son las siguientes:

* Poca interpretabilidad al ser realmente cajas negras, aunque se ha logrado mitigar bastante este problema gracias a los modelos de atención.
* Requieren muchos datos, pero en el contexto de los sistemas recomendadores es relativamente simple generar datasets de forma autómatica.
* Se deben tunear muchos hiperparámetros, aunque algunos modelos recientes de Deep Learning han logrado requerir de casi la misma cantidad que los modelos tradicionales.

Finalmente, se hace una revisión de algunos modelos del estado del arte:

* **MLP (Multilayer Perceptron):** Permite añadir capas neuronales a los modelos tradicionales, de forma que se puedan modelar las interacciones de forma tanto lineal como no lineal. También aprende características de forma eficiente, aunque es preferible utilizar los modelos siguientes para este tipo de tareas.
* **AE (Autoencoder):** Permite reconstruir los datos de entrada utilizando información adicional del usuario o ítem, logrando mitigar problemas tales como alta sparsity y cold start. Además, puede aprender características de forma eficiente, limpiando el ruido de los datos al generar una nueva codificación.
* **CNN (Convolutional Neural Network):** Permite procesar y representar las características de datos multimedia de forma muy eficiente, incluyendo textos, imágenes, audio y video.

Este paper (hasta la sección 3.4) me pareció muy útil, presentando un resumen que permite a los entusiastas del área comenzar a experimentar con modelos de Deep Learning dentro de sus sistemas sin perder mucho tiempo recopilando fuentes de información sobre el área. Las ventajas del Deep Learning parecen claramente vencer a sus contras, considerando que muchas de las críticas realizadas a estos modelos han perdido relevancia gracias a nuevas mejoras que se realizan constantemente (un ejemplo serían los modelos que incluyen auto atención, permitiendo interpretar la representación final de la información a pesar de ser una caja negra).

También me hacen mucho sentido las mejoras al momento de representar la información de las interacciones, ya que efectivamente los modelos tradicionales son lineales, lo que los limita a sólo poder considerar una proyección específica de la información, mientras que la no linealidad logra modelar comportamientos mucho más complejos en cuanto al interés de los usuarios y sus interacciones con los ítems.

La estructura del paper es atractiva, organizando cada sección de forma que sea posible buscar la información deseada de forma ágil dentro de todo el artículo, a pesar de que es extenso. Se nota mucho el esfuerzo de los autores al tener que analizar más de 100 publicaciones y resumirlas en este estudio, permitiendo así una entrada más fácil hacia el mundo del Deep Learning en los sistemas recomendadores modernos.

En cuanto al estado del arte, encuentro toda la razón respecto a la utilidad de las CNN para modelar datos multimedia (por ejemplo en sistemas content based), ya que en el curso de Deep Learning aprendí sobre la gran capacidad de estas redes para aprender características de imágenes o videos (considerándolos como secuencias de imágenes). Aunque no era parte de la lectura de esta semana, puedo decir lo mismo sobre las RNN, que han probado ser esenciales en el procesamiento de textos e información temporal. Encontré curioso el hecho de que las MLP tengan tanto potencial en el área, ya que tenía la idea de que las redes más complejas (CNN, RNN, entre otras) habían sobrepasado completamente a las MLP hoy en día (imagino que en algunos casos es más eficiente usar modelos más simples para que el entrenamiento sea más rápido). Por último, aprendí algo nuevo sobre los Autoencoders, que no conocía hasta ahora, encontrándolos muy útiles para combatir la falta de datos o los datos poco limpios (que suele ser el caso).

Finalmente, recomendaría este paper a cualquier persona que esté comenzando su trabajo en el área de investigación de los sistemas recomendadores, ya que será esencial utilizar estas técnicas a futuro, tanto en el área del Machine Learning general como en la recomendación.
