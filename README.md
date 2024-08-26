# SISTEMA DE DETECCION DE ENLACES SPAM  

Queremos implementar un sistema que sea capaz de detectar automáticamente si una página web contiene spam o no basándonos en su URL.

Paso 1: Carga del conjunto de datos

Paso 2: Preprocesamiento de enlaces
Transformamos los datos para compatibilizarlos con el modelo que queremos entrenar. 
Segmentamos las URLs en partes según sus signos de puntuación, eliminamos las stopwords, lematiza, etcétera.

Paso 3: Construimos un SVM
Implementamos un SVM con los parámetros por defecto. 
Lo entrenamos y analizamos sus resultados.

Paso 4: Optimizamos el modelo anterior
Después de entrenar el SVM, optimizamos sus hiperparámetros utilizando un grid search o un random search.

Paso 5: Guardamos el modelo


# ESTRUCTURA

The project is organized as follows:

- `app.py` - The main Python script that you run for your project.
- `explore.py` - A notebook to explore data, play around, visualize, clean, etc. Ideally the notebook code should be migrated to the app.py when moving to production.
- `utils.py` - This file contains utility code for operations like database connections.
- `requirements.txt` - This file contains the list of necessary python packages.
- `models/` - This directory should contain your SQLAlchemy model classes.
- `data/` - This directory contains the following subdirectories:
  - `interin/` - For intermediate data that has been transformed.
  - `processed/` - For the final data to be used for modeling.
  - `raw/` - For raw data without any processing.
 
    
## Setup

**Prerequisites**

Make sure you have Python 3.11+ installed on your. You will also need pip for installing the Python packages.

**Installation**

Clone the project repository to your local machine.

Navigate to the project directory and install the required Python packages:

```bash
pip install -r requirements.txt
```

## Running the Application

To run the application, execute the app.py script from the root of the project directory:

```bash
python app.py
```

## Contributors

This template was built as part of the 4Geeks Academy [Data Science and Machine Learning Bootcamp](https://4geeksacademy.com/us/coding-bootcamps/datascience-machine-learning) by [Alejandro Sanchez](https://twitter.com/alesanchezr) and many other contributors. Find out more about [4Geeks Academy's BootCamp programs](https://4geeksacademy.com/us/programs) here.

Other templates and resources like this can be found on the school GitHub page.
