# Proyecto-Final
## Definición del problema


Queremos hacer un modelo capaz de clasificar pokemons por imagen. La idea es subir una imágen y que el modelo prediga qué pokemon es, su tipo y estadísticas. 

## Plan de acción


**Dataset**: Usaremos un dataset descargado de kaggle que contiene imágenes de pokemon, además contiene un archivo que también contiene los nombre de los pokemon y sus tipos.


**Modelo**: Usaremos una red CNN, basada en la subida en el práctico 1. Usaremos grad-CAM para interpretar las zonas de la imagen que la redutiliza para realizar su predicción. Seleccionaremos la última capa convolucional, calcularemos el gradiente de la clase objetivo, promediaremos los gradiente por canal, ponderaremos los feature maps por estos pesos, aplicaremos ReLU, por último generaremos un heatmap que mostrará las zonas más relevantes de la imágen.


**Evaluación del modelo**: Para evaluar el modelo vamos a usar "Accuracy" y "Matriz de confusión". Más que nada porque son herramientas estándar para evaluar los modelos.

[Data set : ](https://www.kaggle.com/datasets/lantian773030/pokemonclassification)


## Justificación del modelo


Nosotros elegimos ocupar un modelo basado en redes convolucionales (CNN) más que nada porque son eficaces para modelos de clasificació, esto ya que detectan patrones espaciales locales a través de filtros convolucionales. Las CNN son escalables, requieren menos parámetros y son robustas. Por lo que le cae como anillo al dedo a este pequeño proyecto. Vamos a tomar la estructura expuesta en el práctico 1 y la adaptaremos a este problema de clasificación de pokemons, para simular de forma espiritual el funcionamiento de la pokedex expuesta en el ánime, claro que sin la voz y mucho más simple.