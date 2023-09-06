# OceanApp
Este sistema tiene como objetivo realizar la identificación de dos principales especies en la pesca incidental por cerco, tales como el lobo marino y el pelicano. [Para más información, click aquí](https://docs.google.com/presentation/d/1T5CdcLSzgRe8cQpoi_sPB4U170551NGOrZNykcJD0xU/edit?usp=sharing)

![DemoOceanApp](https://i.pinimg.com/564x/3e/b8/f7/3eb8f7c348dffd7b3dffcafe81fbf2a6.jpg)

# Entrenamiento
## 1)Base de datos:
Esta base de datos actualmente se encuentra subida en Google Drive, en formato .zip y en carpeta. La base de datos se irá actualizando a medida que avance el proyecto  y pueda ser escalable [click para revisar el artículo del proyecto](https://repositorioacademico.upc.edu.pe/handle/10757/667866) .
Para este caso en particular, se esta tomando un total de 993 imagenes de entrenamiento y 248 para la validación, haciendo uso de la técnica 80%-20%.
## 2)Entrenamiento en la Nube
Actualmente se esta haciendo uso de google colab, debido a que proporciona una maquina virtual gratuita por unas horas, por lo que, se realizó el archivo I_Train_OceanApp YOLOv5.ipynb, también puede revisarse directamente en [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1zn7WAplrncgc4dnmUqBwAs39rTaNAJ9F?usp=sharing). Por otro lado, en el mismo proyecto, se debe subir el archivo customcoco128drive.yaml dentro de la carpeta yolov5/data, ya que, nos ayudará a coordinar la información del etiquetado con el entrenamiento de Yolov5 .
Finalmente, la red entrenada generará una archivo llamado best.pt, que se encuentra en la ruta runs/train/exp/weights/best.pt (se debe descargar este archivo para seguir con el siguiente punto).
# Deploy
## 1) Google Colab:
Para hacer un puesta en producción rápida pero limitada, se realizará el deploy en Google Colab[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1oprv-LRw7mMWrhr4SBNJ0pxM-E-JQDMR?usp=sharing), en la que, se deberá subir el archivo mencionado en el punto anterior (best.pt) que viene a ser la red entrenada del modelo.
Nota; este producto solo durará unas horas ya que esta limitado por el uso de google colab
## 2) HugginFace:
Como en nuestro caso, deseamos tener el modelo en la nube de forma permanente y gratuita, estamos realizando el deploy en HuggingFace, el código se encuentra libre en la misma plataforma [Link Deploy](https://huggingface.co/spaces/Ocean2022/MPREAC.OCEANAPP)
# Citación
Este proyecto de tesis universitario se realizó gracias al aporte de:
Trampas Barceló: Detección y monitoreo a tiempo real del mosquito Aedes aegypti [Link al White Paper](https://docs.google.com/presentation/d/1T5CdcLSzgRe8cQpoi_sPB4U170551NGOrZNykcJD0xU/edit?usp=sharing),
Autores: Riat, César  and Schieder, Mario.
2021

# Contacto 
Para mas información, favor de contactarse al correo electrónico u202020275@upc.edu.pe.

# Autores
Geraldine Jayo Escalante, David Hospinal
