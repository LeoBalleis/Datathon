![HenryLogo](https://d31uz8lwfmyn8g.cloudfront.net/Assets/logo-henry-white-lg.png)

# <h1 align="center">**`Proyecto Individual 2`**

<p align="center">
<img src="https://tecnologiaparatuempresa.ituser.es/files/201908/sanidad.jpg"   
>
</p>

​
¡Bienvenidos! Mi nombre es Leonel Facundo Balleis, al momento de hacer este proyecto me encuentro cursando la etapa de Labs para la carrera de Data Science de SoyHenry. A continuación voy a describir el proyecto, sus objetivos y la conclusión a la cual llegue, luego de realizar un exaustivo analisis de los diferentes modelos .


## Descripción 

Un importante Centro de Salud lo ha contratado con el fin de poder predecir si un paciente tendrá una estancia hospitalaria prolongada(más de 8 días) o no, utilizando la información contenida en el dataset asociado, la cual recaba una muestra histórica de sus pacientes, para poder administrar la demanda de camas en el hospital según la condición de los pacientes recientemente ingresados.
En resumen tenemos que predecir si los pacientes se van a quedar más de 8 días.

## Objetivo 

- Entrenamiento y predicción utilizando un Modelo de Machine Learning adecuado al problema (clasificación o regresión).
- Análisis exploratorio de los datos (EDA).
- División de dataset en train y test utilizando train_test_split, CV, KFold o similares.
- Utilización de Pipelines en la producción del modelo.
- Comentarios y redacción con la fundamentación de la solución propuesta, escrita en Markdown en el Jupyter Notebook (.ipynb) o bien en un documento aparte.
​

## **Explicación de los contenidos del Repositorio:**
​
Se proveen los siguientes archivos :
- La carpeta 'datasets' que contiene 2 archivos: 'hospitalizaciones_train.csv','hospitalizaciones_test.csv'.
- En el notebook 04final se encuentra el código comentado paso por paso, explicando las decisiones tomadas.
- En el archivo DecisionTree_model.pkl se encuentra el modelo de árbol de decisión creado.
- Archivo ' README.md'.
- LeoBalleis.csv es el csv con la predicciones.


## **Métrica a utilizar**
+ precision_score.

+ accuracy_score.

+ f1_score.

+ roc_auc_score.

+ recall_score.
​

## **Herramientas utilizadas**:

+ Python.

+ Pandas.

+ sklearn.

+ seaborn.

+ matplotlib.

+ Numpy.

+ Joblib


## CONCLUSION

Trabajando en el proyecto que busca predecir la instancia hospitalaria de los pacientes aplique 2 modelos: LogisticRegression y DecisionTreeClassifier; Los cuales fui descartando hasta llegar a elegir el DecisionTreeClassifier considerando que tiene el mejor desempeño en cuanto a la Precisión, Exatitud, Recall,f1_score y curva roc.
Gracias a mi experiencia laboral hospitalaria y analisando las metricas en consideracion, he llegado a la conclusion de que priorizo tener un recall más alto que la precisión porque estimo mejor tener mas falsos positivos (gente que se va  a quedar mas de 8 dias pero no lo hace) que el caso contrario tener mas falsos negativos (gente que no se va  a quedar mas de 8 dias pero lo hace) y encontrarme en la situacion de no tener camas.

