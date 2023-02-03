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

En orden crecientes los valores de los pixeles cubiertos por la ventana
móvil son

115, 119, 120, 123, 124, 125, 126, 127,
150

El valor de la mediana será pues 124.

Además, como la mediana es uno de los valores de los pixeles vecinos, conduce a resultados más realistas que la media. Esto hace que la mediana si bien  ̈suaviza ̈
la imagen preserva los bordes más grandes cuyas dimensiones sean mayores que las dimensiones del kernel. Esto es muy conveniente cuando este filtro se aplica
para eliminar ruidos como los de  ̈salt and pepper ̈ o los speckles de las imágenes de radar.

### Aplicación del algoritmo
Se aplicaron los tres algoritmos TOPLISS por medio del código propuesto

![image](https://user-images.githubusercontent.com/99137141/216526293-7aca50df-6e05-41d3-9a4f-55decadf96b5.png)

