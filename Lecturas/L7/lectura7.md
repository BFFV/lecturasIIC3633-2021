### Review: Sistemas Recomendadores Interactivos: Un Estudio del Estado del Arte y Desafíos y Oportunidades Futuras de Investigación

Este paper presenta un estudio sobre los sistemas recomendadores modernos, que están enfocados en mejorar la experiencia del usuario al interactuar directamente con este por medio de herramientas de visualización de información. Se reconocen los siguientes desafíos que deben ser superados para que estos sistemas logren explotar su máximo potencial:

- **Cold Start:** No se logran realizar recomendaciones efectivas para usuarios nuevos o en base a ítems nuevos que no poseen suficiente relevancia.
- **Caja Negra:** Es difícil explicar el razonamiento detrás de las recomendaciones, lo que lleva a pérdida de confianza de los usuarios en caso de que estas fallen.
- **Interacción con el Usuario:** La naturaleza de los sistemas evita que los usuarios interactúen directamente con el proceso de recomendación, lo que ayudaría a guiar los intereses del usuario inferidos por el sistema recomendador de forma más ágil.

Se propone un **framework interactivo**, compuesto por los siguientes nodos:

- **Datos del Usuario:** Ratings, historial e información sobre las interacciones del usuario con los ítems.
- **Contexto:** Información contextual sobre el usuario, por ejemplo su localización e intereses personales, entre otros.
- **Motor Recomendador:** Recibe la información de los datos del usuario y contexto, generando a los nodos de medios y de recomendaciones.
- **Medios:** Datos inferidos de la información de entrada y contexto, representando los elementos que afectan las recomendaciones entregadas.
- **Recomendaciones:** Las recomendaciones entregadas al usuario.

Con esta propuesta se busca cumplir con los siguientes objetivos:

- **Transparencia:** Explicar la lógica interna del sistema al momento de realizar las recomendaciones.
- **Justificación:** Entregar la razón de las recomendaciones entregadas, sin explicar el proceso interno utilizado para generarlas.
- **Controlabilidad:** Permitir al usuario controlar directamente el proceso de recomendación mediante una interfaz de ajustes.
- **Diversidad:** Entregar recomendaciones que cubran una gran parte del espacio total disponible de ítems para recomendar (evitar sesgo).
- **Cold Start:** Atacar el problema de los nuevos usuarios o ítems que no entregan suficiente información para poder recomendar eficientemente.
- **Información Contextual:** Integrar la información contextual en el proceso de recomendación de forma flexible (por ejemplo, considerar la emoción que siente el usuario actualmente).

A continuación se revisa el cumplimiento de estos objetivos en 24 sistemas recomendadores interactivos, encontrando que el enfoque principal se encuentra en mejorar la transparencia y controlabilidad, y que esta metodología de interacción con el usuario por medio de visualización de información efectivamente logra mejorar el rendimiento percibido en la práctica. También se evidencia que predominan las visualizaciones por medio de nodos y enlaces, seguidas de las radiales y las basadas en conjuntos.

Finalmente, se indica que los desafíos pendientes incluyen lo siguiente: 

- Atacar más los objetivos del Cold Start, la diversidad, novelty y serendipity (recomendaciones inesperadamente buenas o poco conocidas).
- Adaptar el nivel de complejidad de algunas técnicas de visualización de forma que el usuario no tenga problemas en entenderlas.
- Formalizar métodos de evaluación de estos sistemas, que permitan determinar las mejores visualizaciones y herramientas según su contexto y uso en la práctica.

En mi opinión el paper es de gran calidad, presentando un estudio muy completo que analiza el estado del arte en cuanto al nuevo nivel que están alcanzando los sistemas recomendadores hoy en día.
