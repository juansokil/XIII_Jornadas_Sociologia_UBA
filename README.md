# Deep Learning y Ciencias Sociales

Este repositorio contiene los script utilizados para la ponencia
"Redes para entender redes. El uso de redes neuronales para el análisis de redes sociales."
XIII Jornadas de Sociologia
Facultad de Ciencias Sociales, UBA, Agosto 2019 

## Resumen

Este trabajo propone analizar las imágenes publicadas en Instagram por referentes de tres agrupaciones políticas argentinas (Unidad Ciudadana, Cambiemos y FIT), bajo el supuesto de que a partir de las imágenes es posible identificar las ideas que profesan cada, que existen componentes no-verbales que permiten asociar una imagen a una postura política. Para tal fin se trabajar ́a con redes neuronales convolucionales, buscando identificar esos componentes no-verbales que permiten identificar las ideas.


### Primer parte, detectar objetos y personas###

Object Detection: Detecta objetos en una imagen, con un "Bounding Box". Utiliza resnet50_v2.0.1.h5

Face Detection: Detecta caras, utiliza la red preentrenada MTCNN


### Recortar las caras y caracterizarlas

Face Crop: Recorta las caras y las guarda en un archivo nuevo. Utiliza CascadeClassifier

AgePrediction y GenderPrediction: Utilizan Utilizan una red vgg preentrenada para identificar la edad aparente y el genero aparente.


### Modelo de clasificación - No utilizado en el trabajo final

Image Classification: Permite clasificar una imagen a partir de distintas categorias de respuesta.


## Resultados

Ver la presentación:

https://github.com/juansokil/XIII_Jornadas_Sociologia_UBA/blob/master/Presentacion.pdf

Ver el trabajo completo:

http://jornadasdesociologia2019.sociales.uba.ar/altaponencia/?acciones2=ver&id_mesa=9&id_ponencia=679
