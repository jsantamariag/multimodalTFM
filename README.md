# Meme-GPT 🦙🐸

## What is Meme-GPT?

Meme-GPT es un modelo basado en CLIP-LLaMA diseñado para entender y generar texto y memes multimodales. Utiliza el poder de los modelos CLIP y LLaMA para proporcionar capacidades avanzadas en procesamiento de lenguaje natural y visión por computadora. Se trata de una arquitectura encoder-decoder donde CLIP genera embeddings de imágenes y LLaMA las procesa para escribir un tweet. Meme-GPT ha sido entrenado sobre el dataset MMHS150K y está preparado para generar twits a partir de memes.

![Meme-GPT](https://github.com/jsantamariag/multimodalTFM/blob/main/MEME_GPT.png)

## Primeros Pasos

Para empezar con este proyecto, primero necesitas instalar las dependencias necesarias. Puedes hacerlo ejecutando la siguiente celda de código en tu entorno:

```bash
pip install -r requirements.txt
```

## Resumen de Archivos
### Notebooks
- TFM_T5.ipynb: Entrenamiento y testeo del modelo encoder-decoder basado en CLIP y T5.
- TFM_LLM.ipynb: Entrenamiento y testeo del modelo encoder-decoder basado en CLIP y LLaMA.
- TFM_LLAVA.ipynb: Script para entrenar con LLaVA, como experimento adicional pero que no se ha llegado a terminar de ejecutar por falta de GPU.
- metricas.ipynb: Notebook en el que se han testeado y sacado métricas de los modelos desarrollados.
- search.ipynb: Notebook breve con código para poder buscar cualquier tweet concreto del dataset si se quiere.
- Initial_Config.ipynb: Notebook inicial para instalar dependencias y descargar el dataset.
### Otros Archivos
- image_embeddings.pkl: Archivo de embeddings precalculados para el entrenamiento.
- full_val_records_llama: Archivo con los logs de validación del modelo LLaMA.
## Guía de Uso
1. Instalar dependencias e iniciar datos
Ejecutar el código en Initial_Config.ipynb, que contiene la instalación de dependencias y la descarga del dataset. Si alguno de los enlaces públicos utilizados para descargar el dataset dejase de funcionar, dirigirse a Kaggle Dataset.

2. Ejecutar uno de los notebooks principales
- TFM_T5.ipynb contiene el código para entrenar o testear un modelo CLIP-T5.
- TFM_LLM.ipynb contiene el código para entrenar o testear un modelo CLIP-LLaMA.
3. Ejecutar cualquiera de los notebooks secundarios para hacer búsquedas, calcular métricas o ejecutar el entrenamiento de LLaVA, respectivamente
- search.ipynb
- metricas.ipynb
- TFM_LLAVA.ipynb
