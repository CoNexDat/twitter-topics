# 75.00 Tesis de grado de Ingenieria en Informática (FIUBA)
## Autores
- Tesista: Tomás Mussi Reyero
- Director: Dr. Ing. Mariano G. Beiró
- Co-director: Dr. Ing. J. Ignacio Alvarez-Hamelin

### Contenido
Este repositorio contiene todo el código utilizado

El objetivo de la presente tesis es analizar un conjunto de datos extraido de Twitter que contiene usuarios y los tweets que publicaron.
A través de los notebooks se puede reproducir todo el proceso


### Notebooks
El trabajo se dividió en seis notebooks, en los cuales detallamos:
- 01 Análisis preliminar: graficamos la cantidad de *tweets* por día capturados.
También observamos la distribución de grados entrante y saliente de la red de usuarios.
- 02 Matriz de coocurrencia de *hashtags*: a partir de los *tweets* que los usuarios publicaron y filtrando contenido, generamos el grafo de coocurrencia de *hashtags*. Luego de aplicar el algoritmo de detección de comunidades OSLOM, obtenemos los tópicos a los que pertenece cada *hashtag*.
- 03 Homofilia temática: luego de obtener los tópicos, pasamos a hacer un análisis sobre los tópicos que utilizaron los usuarios. Analizamos la similitud que hay entre usuarios de la red.
- 04 Evolución de similitud temporal: convertimos la utilización de *hashtags* en la utilización de tópicos, y particionamos la utilización a través del tiempo en múltiples matrices usuario-tópico para la ventana de tiempo bajo análisis. Comparamos la evolución de la similitud entre grupos de usuarios que siguen a un único candidato a presidente dentro de la red.
- 05 Análisis temporal de tópicos: observamos la utilización de ciertos tópicos por parte de los seguidores de los candidatos y detectamos que tópicos son los más específicos dentro de las comunidades.
- 06 Predicción de alineamiento político de los usuarios: clasificamos a los usuarios de acuerdo a si *retweetearon* a un único candidato. Vamos a analizar y extraer matrices para dos períodos, uno el período electoral completo y el otro hasta la primera vuelta. Luego obtenemos dos matrices de *features* para cada período, una con los tópicos obtenidos en el proceso y la otra aplicando reducción de dimensiones sobre la matriz de usuario-*hashtag* para conseguir la misma cantidad de *features* que los tópicos. Finalmente tenemos cuatro matrices a las que utilizamos el clasificador *Random Forest* y verificamos la eficacia para cada una de las cuatro matrices.
