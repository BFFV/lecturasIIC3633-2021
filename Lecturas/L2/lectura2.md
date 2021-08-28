### Review: Sistemas Recomendadores Basados en Filtrado Colaborativo

El paper trata sobre el extenso tema del filtrado colaborativo (en el contexto del año 2007), comenzando por explicar el gran protencial de información 
que se encuentra en las comunidades de usuarios de plataformas digitales, y cómo se pueden utilizar los ratings y atributos de usuarios/items dentro de estas plataformas
para alimentar a un sistema recomendador y entregar predicciones/recomendaciones. Se revisan de forma detallada las posibles utilidades de estos sistemas (revisando distintos contextos sobre los que se pueden aplicar), 
los algoritmos más utilizados para implementarlos (probabilísticos y no-probabilísticos), las métricas a utilizar para evaluar el rendimiento (accuracy, confidence, novelty), así como un análisis sobre las tendencias actuales, el futuro 
de estos tipos de sistemas y los desafíos que se deben trabajar con mayor prioridad actualmente (privacidad y seguridad, confianza, transparencia de las recomendaciones).

Encuentro que el paper fue bastante útil para tener una mirada más detallada de los temas vistos en las clases del curso, permitiendo además revisar el estado de esta tecnología 
hace ya más de una década. Me pareció interesante la sección donde se habla de las 2 soluciones propuestas en los años 90, ya que a diferencia de la fecha de publicación de este paper, 
las técnicas de inteligencia artificial de hoy en día han logrado suficientes avances como para dar origen a modelos que en aquellos tiempos no eran posibles, como lo es el campo del deep learning 
(que está entre los temas que veremos en este curso).

También me llamó la atención la distinción que existe entre "predecir" y "recomendar", en donde lo primero suele ser mucho más costoso en los cálculos a realizar, debido a que al recomendar se suele 
usar un subconjunto de los datos disponibles en vez de su totalidad. Esto se puede percibir como ligeramente contra-intuitivo a primera vista, dado que predecir sólo entrega el output para 1 ítem, mientras que recomendar 
entrega un ranking de varios items, pero aún así suele ser menos costoso debido a la naturaleza de la actividad misma y los "atajos" que los algoritmos pueden utilizar para ahorrar procesamiento y memoria.

Por último, creo que las predicciones realizadas sobre el futuro de estos sistemas se han cumplido en gran parte, ya que personalmente he visto páginas web que son más transparentes en el uso de su sistema recomendador, 
permitiendo ver fácilmente las reviews y perfiles de otros usuarios que aportan al sistema. Eso sí, los temas de seguridad siguen siendo un desafío hoy en día, el mal uso de estos sistemas para intentar sesgar las recomendaciones 
sigue siendo un campo de investigación activo en la actualidad, por dar un ejemplo.
