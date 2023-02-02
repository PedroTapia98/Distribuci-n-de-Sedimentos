# Distribución de Sedimentos en Deltas

Un delta es un accidente geográfico convexo formado en la desembocadura de un río en un lago o en el mar a través de los sedimentos que deposita la corriente.
Se desea analizar la distribución de los sedimnetos que contiene un delta ubicado en el Rió Ometepec, Guerrero. Posteriomente por medio del histrograma raster saber que tipo de sedimento se encuentra en la distribución analizada.

La percepción remota es una disciplina que integra los desarrollos más recientes en observación, exploración y monitoreo del planeta tierra. Los sensores remotos cumplen la misión de ofrecer información en diferentes regiones del espectro electromagnético. La capacidad de registrar información en las regiones del espectro electromagnético, permite caracterizar objetos en la superficie terrestre dependiendo de la región que se trabaja y es una fuente de información relevante para estimar variables biofísicas.

## Metodología


### Ubicación
Se encuentra ubicado en el estado de Guerrero, casi en la frontera con Oaxaca, Latitud Norte: 16.577412, Longitud Oeste: 98.785086.

### Imágenes Satelitales usadas
Se seleccionaron imágenes del 06 de diciembre del 2019 para descargar de la pagina https://earthexplorer.usgs.gov/con un nivel 1 y nubosidad menor al 10 porciento.

### Preprocesamiento
Se realizaron las correcciones atmosféricas y de temperatura en Qgis con la herramienta Semi-Automatic Classification Plugin en el software QGIS

### Filtrado de la imágen

#### Filtro de Mediana
Se suele usar para eliminar ruido en la imagen. Los filtros de mediana sustituyen cada píxel de la imagen por la mediana de los pixeles vecinos.

![image](https://user-images.githubusercontent.com/99137141/216234835-de5cd26f-ea2d-446b-8465-c62a1a4fa15d.png)
