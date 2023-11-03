Este trabajo consiste en la creación de un modelo de aprendizaje
automático mediante un árbol de decisión, de modo que sea interpretable y
permita predecir la columna 'Rating'. Para ello, partimos de un dataset
sobre el cual debemos construir las variables 'Reviews', 'Followers' y
'Sentimiento'. En particular, una de las partes más interesantes del problema es
la obtención de la columna 'Sentimiento'. Se propuso emplear un modelo LLM para
la consecución de esta tarea. En nuestro caso, no fue eficiente instalar el modelo
LLM en local debido a la falta de capacidad de nuestros ordenadores. Como alternativa,
decidimos usar los servidores GPU de Colab para cargar el modelo. Por otro lado,
para utilizar un modelo en local, se ha empleado Bert para generar otros resultados en 
la columna 'Sentimiento'. Se han creado dos árboles 
de decisión con la finalidad de comparar los resultados que proporcionan los 
modelos, concluyendo que ambos son bastantes similares. La variable 'Sentimiento' 
ostenta la máxima relevancia en los dos modelos, seguida de 'Reviews', si bien su 
relevancia es mucho más reducida. En contraste, la variable 
'Followers' apenas aporta importancia en comparación con las otras dos.