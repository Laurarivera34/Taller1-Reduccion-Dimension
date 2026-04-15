## Descripción del proyecto

Este proyecto aplica técnicas de reducción de dimensionalidad en dos contextos distintos. Por un lado, se utiliza el análisis de componentes principales (PCA) para estudiar la calidad de vida en diferentes ciudades. Por otro lado, se emplea la descomposición en valores singulares (SVD) para el reconocimiento facial a través del método de eigenfaces. El objetivo general es simplificar conjuntos de datos con muchas variables, facilitando su interpretación y análisis.

## Estructura del proyecto

El proyecto está organizado en las siguientes carpetas:

##  data
Contiene las bases de datos utilizadas en el análisis, incluyendo los datos de calidad de vida y el conjunto de imágenes de rostros.

## figs
Incluye las visualizaciones generadas a lo largo del proyecto, como gráficos de varianza explicada, proyecciones de PCA y representaciones de eigenfaces.

## Parte 1. Análisis de componentes principales

Se trabaja con datos provenientes del Almanaque Calificado de Lugares, donde 329 ciudades fueron evaluadas según nueve criterios relacionados con calidad de vida: clima y terreno, alojamiento, salud y medio ambiente, crimen, transporte, educación, artes, recreación y economía.

Dado el número de variables, el análisis directo resulta complejo debido a la gran cantidad de relaciones entre ellas. Para abordar este problema se utiliza PCA, que permite reducir la dimensionalidad del conjunto de datos y resumir la información en un menor número de componentes.

A partir de este análisis se obtiene la varianza explicada por cada componente, así como nuevas representaciones de las ciudades en un espacio de menor dimensión, lo que facilita la identificación de patrones.

## Parte 2. Descomposición en valores singulares

En la segunda parte se utiliza la base de datos Labeled Faces in the Wild, que contiene más de trece mil imágenes de rostros etiquetados. Se trabaja con un subconjunto de personas que cuentan con múltiples imágenes.

Se aplica SVD para descomponer la información de las imágenes y obtener las llamadas eigenfaces, que son representaciones principales de los rostros. Estas permiten expresar cada imagen como una combinación de componentes principales.

El uso de SVD facilita la reducción de dimensionalidad, la reconstrucción de imágenes y el análisis de patrones en los datos visuales.

## Herramientas utilizadas

El desarrollo del proyecto se realiza en Python, utilizando librerías como NumPy, Pandas, scikit-learn y Matplotlib.

## Conclusiones

El uso de PCA permite resumir información compleja sobre calidad de vida en unas pocas dimensiones interpretables. Por su parte, SVD muestra su utilidad en el procesamiento de imágenes y en la extracción de características relevantes para el reconocimiento facial.

Ambas metodologías evidencian la importancia de la reducción de dimensionalidad en el análisis de datos.
