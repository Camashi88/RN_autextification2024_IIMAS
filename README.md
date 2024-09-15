# Red Neuronal de la tarea 1 de Autextification.

# Corpus.📄
Para evitar que nuestros modelos presenten overfitting, realizamos una mezcla aleatoria del corpus de cada subtarea antes de dividirlo en conjuntos de entrenamiento y prueba. La división se realiza de manera estratificada, de modo que el 70% de los datos se asigna al conjunto de entrenamiento y el 30% restante al conjunto de validación, asegurando particiones bien equilibradas en ambos conjuntos.

El corpus se encuentra [aquí]([url](https://drive.google.com/drive/folders/1VdTmKAzrfFrL-MKEmsvEXjYKugrm5Rw7)).

# Acerca del modelo.🔬

A partir del corpus incial, podemos obtener las siguientes características y refinamientos, también encontrados en el link donde:

1. **RoBERTa, BERT y e5** embeddings son refinamientos que proveen de contexto, así como el significado basado en oraciones.
2. **stylometric** embeddings capturan el estilo y estructura de escritura de las oraciones y proveen información basada en el estilo y no semánticas.

# Proceso.⚙️
- Los embeddings entran en la Red Neuronal.
- La Red Nueronal aprende nuevas representaciones sobre los embeddings de entrada mediante las capaz densas. Estas representaciones dará a conocer patrones o características que pueden ser de ayuda para la tarea (distinguir entre "generated" y "human")
- El modelo procesa los embeddings de entrada por varias transformaciones (capas densas, activaciones y dropouts) y da predicciones de salida basadas en la capa final (en este caso sigmoid, ya que es una tarea binaria).

<img width="500" alt="4" src="https://github.com/user-attachments/assets/73d93373-28dd-4da9-ac94-1adb66c289d5">

