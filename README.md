# Proyecto-Final
## Definición del problema


Queremos hacer un modelo capaz de clasificar pokemons por imagen. La idea es subir una imágen y que el modelo prediga qué pokemon es, su tipo y estadísticas. 

## Plan de acción


**Dataset**: Usaremos un dataset descargado de kaggle que contiene imágenes de pokemon, además contiene un archivo que también contiene los nombre de los pokemon y sus tipos.


**Modelo**: Usaremos una red CNN, basada en la subida en el práctico 3. El modelo entrenado con un dataset compuesto de imágenes de los 150 pokemon originales, haremos transfer learning para que en la parte de testeo puedas cargar la imagen del pokemon que deseas identificar. La imagen se convertirá en tensores, que posteriormente se le entregarán al modelo para hacer su predicción.


**Evaluación del modelo**: Para evaluar el modelo vamos a usar "Accuracy" y "Loss Over Epochs". Más que nada porque son herramientas estándar para evaluar los modelos.

[Data set : ](https://www.kaggle.com/datasets/lantian773030/pokemonclassification)


## Justificación del modelo


Nosotros elegimos ocupar un modelo basado en redes convolucionales (CNN) más que nada porque son eficaces para modelos de clasificació, esto ya que detectan patrones espaciales locales a través de filtros convolucionales. Las CNN son escalables, requieren menos parámetros y son robustas. Por lo que le cae como anillo al dedo a este pequeño proyecto. Vamos a tomar la estructura expuesta en el práctico 1 y la adaptaremos a este problema de clasificación de pokemons, para simular de forma espiritual el funcionamiento de la pokedex expuesta en el ánime, claro que sin la voz y mucho más simple.