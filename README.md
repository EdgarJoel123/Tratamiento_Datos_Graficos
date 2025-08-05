## ENTREGA EJERCICIO PRÁCTICO CLASE 3
# Dataset Netflix Data Analysis

# Descripción del propósito del dataset
Este conjunto de datos trata sobre películas y series de Netflix. Consta de 12 columnas con algunos valores nulos. Para su análisis se utilizan las bibliotecas Numpy, Pandas, Matplotlib.pyplot, Seaborn y Wordcloud. El proceso de análisis se dividió en varias partes para un análisis paso a paso y para responder las preguntas con gráficos.

# Explicación de los pasos de limpieza y transformación
<br/>
Datos faltantes
Existen diversas representaciones de datos faltantes, como valores nulos y valores faltantes, no se encontro valores duplicados. Utilicé algunos métodos del proceso de análisis de datos para eliminar los valores faltantes dropna.
<br/>
Extracción de datos
<br/>
Conversión de fechas
En la columna date_added, eliminamos los espacios en blamnco al inicio y final, y al convertir un tipo de objeto en objetos de tipo de datos con la función to_datetime, obtenemos un objeto Datatime que permite extraer diversas partes de los datos, como el año, el mes y el día.

# Principales hallazgos del análisis

¿Qué tipo de contenido predomina en el catálogo de Netflix: películas (Movie) o series (TV Show)?

Gráfico de barras verticales con sns.countplot que muestran el número de tipo de contenido (Movie o TV Show), el resultado de la gráfica muestra el predominio de las peliculas en el catálogo de Netflix. 

¿Cuál es la cantidad de títulos en Netflix por clasificación de contenido (rating)?

Gráfico de barras verticales con sns.countplot que muestran el numero de tipo de rating, se ordena las clasificaciones por frecuencia, Las clasificaciones más comunes son TV-MA (contenido para adultos) y TV-14, lo que indica que gran parte del contenido está dirigido a audiencias maduras, hay menos contenido infantil en comparación con otras plataformas.

¿Qué tipo de contenido clasificado es más común en Netflix?

La representación de este gráfico es en porcentaje a la pregunta anterior, que por tratarse con muchas clasificaciones se visualiza mejor en barras horizontales con sns.barplot a diferencia de un  gráfico en pastel.

¿Cuáles son los países más representados en el catálogo de Netflix?

Representación por nube de palabras para visualizar los paises con más titulos, crear una nube de palabras de los generos de los titulos, eliminar valores nulos y unir todos los paises en una sola cadena, separar multiples paises y limpiar espacios, el resultado que el país más representado en el catálogo de Netflix es Estados Unidos, seguido por India y el Reino Unido.

# Cualquier insight o conclusión relevante

Ideal para realizar predicciones implementando análisis de Machine Learning con scikit-learn, por ejemplo, el tipo de contenido (película o programa de televisión) basado en las características disponibles.
Netflix usa estos datos para personalizar recomendaciones, identificar géneros populares y decidir qué tipo de contenido producir.
El análisis de visualización y comportamiento del usuario permite crear series y películas que se alinean con los gustos regionales.
