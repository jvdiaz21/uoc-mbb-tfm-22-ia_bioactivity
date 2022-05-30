# UOC | Máster en Bioinformática y Bioestadística | TFM

### Comparación de modelos de inteligencia artificial basados en estructuras y descriptores moleculares para la predicción de bioactividad en el marco de desarrollo de fármacos

Este repositorio contiene la solución integral para el desarrollo, el entrenamiento y el análisis de rendimiento varios algoritmos de inteligencia artificial aplicados a la predicción de bioactividad. 

El primer grupo de modelos corresponde a los algoritmos eXtreme Gradient Boost, Random Forest y Support Vector Machine de machine learning, tres de los métodos más populares utilizado en la tarea de predicción de actividad farmacológica [1] y se utilizan descriptores moleculares como variables regresoras. 

El segundo algoritmo corresponde a una arquitectura de deep learning definida sin referencia y basada en redes neuronales gráficas convolucionales [2] y se utilizan grafos correspondientes a las estructuras bidiomensionales de las moleculas (i.e., posición y tipo de sus átomos y conexiones entre ellas) como input de la red.

El objetivo principal del proyecto se enfoca en evaluar la viabilidad de estos tipos de algoritmos para la tarea de regresión mencionada y comparar su rendimiento para determinar si considerar únicamente la estructura molecular podría resultar equivalente o mejor que considerar un conjunto de descriptores cuantitativos. 

### Acerca de

Este proyecto corresponde al Trabajo Final de Máster del programa de [Máster universitario en Bioinformática y Bioestadística de la UOC](https://estudios.uoc.edu/es/masters-universitarios/bioinformatica-bioestadistica/presentacion), desarrollado en el semestre de primavera del curso 2021-2022 por:

[Juan Vigueras Díaz](https://www.linkedin.com/in/juan-v-012124180/)

## Distribución del Repositorio 

La distribución de los archivos del proyecto en este repositorio es:

	├── Checkpoints			# Modelos Entrenados
		├── DL				# Modelos de Deep Learning
		└── ML				# Modelos de Machine Learning 
	├── Datasets				# Conjuntos de datos
		├── DATA_FRAMES		# Datos de experimentos ML 
		├── DATA_LOADERS		# Datos de experimentos DL 
		├── DATA_LOADERS_75		# Datos reducidos de experimentos DL 
		├── DATA_RAW			# Datos descargados de la BBDD
		└── DESCRIPTORS		# Listas de descriptores específicos para cada target-indicador
			└── RAW			# Todos los descriptores calculados para cada target-indicador
		└── DATASET_RAW.txt		# Archivos DATA_RAW unificados y resumidos
	├── Documentos      		# Documentos con la planificación y desarrollo del proyecto
	├── Notebooks	 			# Notebooks para ejecutar en Google Colab u otra IDE (Ej. Jupyter)
	├── Resultados				# Archivos con los resultados experimentales
		├── DL				# Modelos de Deep Learning
		└── ML				# Modelos de Machine Learning
	└── README.md

## Cómo ejecutar el código

El proyecto entero puede ejecutarse abriéndolo en Google Colab y ejecutando las celdas correspondientes. 

Hay que tener un especial cuidado con las rutas utilizadas, pues es necesario referenciar correctamente las rutas de los directorios de Google Drive donde se dipositan los datos y donde se quieren guardar los resultados. Al principio de cada notebook, existe un `diccionario` llamado `path` en el que el usuario puede definir estas rutas. La estructura indicada por defecto puede no coincidir con la distribución de carpetas de este repositorio.

## Desarrollo

El planteamiento, la planificación, el desarrollo (implementación, ejecución) y análisis de resultados del proyecto se puede consultar en los dos archivos adjuntos llamados `Definición de los contenidos de trabajo`, `Plan de Trabajo`, `Desarrollo del Trabajo I` y `Desarrollo del Trabajo II`. En una futura actualización del repositorio, se incluirá la `Memoria` completa del trabajo. 

## Referencias

[1] Lavecchia A. (2015). Machine-learning approaches in drug discovery: methods and applications. Drug discovery today, 20(3), 318–331. https://doi.org/10.1016/j.drudis.2014.10.012 

[2] Kipf, T. N., & Welling, M. (2016). Semi-supervised classification with graph convolutional networks. arXiv preprint arXiv:1609.02907 . https://doi.org/10.48550/arXiv.1609.02907 

Todas las referencias sobre los artículos consultados y las bibliotecas utilizadas están indicadas directamente en la documentación de desarrollo del proyecto.#uoc-mbb-tfm-22-ia_bioactivity
