
# Mercado Inmobiliario
Este proyecto se enfocará en el análisis de datos de un dataset de la página web [Properati](https://www.properati.com.ar/data/), el cual presenta información sobre propiedades en venta en sectores cercanos a la capital Argentina, Buenos Aires. Con ellos se realizará un análisis explotoratorio de los datos (EDA) para luego entrenar un regresor que nos permita predecir el precio de un inmueble. 

Este proyecto se realizará en dos partes, en la primera parte realizaremos una exploración y limpieza de los datos para entrenar algunos modelos de Machine learning sencillos, y en la segunda parte se aplicará ingeniería de Features y Modelos Avanzados (Regularización Ridge, Lasso, Xgboots, RandomForest, optimización de hiperparámetros usando Cross Validation junto a GridSearchCV y RandomSearchCV) para desarrollar con mayor profundidad un modelo de Machine Learning.
## Contenido
### Primero
- [Exploración](#s-11)
  - [Variables categóricas](#s-112)
  - [Variables númericas continuas](#s-113)  
  - [Variables númericas discretas](#s-114) 
  - [Correlación](#s-1ad)   
- [Desafio](#s-12)
- [Machine Learning](#s-13)
  - [Preparación datos](#s-131)
  - [Benchmark](#s-132)
  - [Regresión por knn casos partículares](#s-133)
  - [Regresión por por tree casos particulares](#s-134)
  - [Función de Modelos casos generales](#s-135)
  - [Transformación de variables y mejoramiento de los modelos de regresión](#s-14)
  - [Benchmark Transformado](#s-141)
         - [Knn Transformado](#s-142)
         - [Tree Transformado](#s-143)
             
- [Conclusiones](#s-15)      

### Segundo
  - [**Primera parte: EDA**](#s-1)
    - [Tratamiento nulos](#s-10)
    - [Features ](#s-11)
     - [Variables categóricas](#s-112)
     - [Variables númericas continuas](#s-113)
     - [Criterio de los 3$\sigma$](#s-113a)
     - [**Transformación variables continuas**](#s-113b)
     - [Correlación](#s-12)
     - [Variables númericas discretas](#s-13) 
      - [Predición batrooms faltantes](s-131) 
     
  - [**Segunda parte: Modelos simples mejorados**](#s-2)
    - [Benchmark](#s-21)
     - [Aciertos y Desaciertos](#s-3raciertos)  
     - [Importancia predictores](#s-21a)
     - [DecisionTree](#s-22)
     - [Optimización de hiperparámetros](#s-221)
     - [Aciertos y Desaciertos](#s-3raciertos2)      
     - [Importancia predictores](#s-221a)
     -[KNeighbors  ](#s-23)
       - [Aciertos y Desaciertos](#s-3raciertos3)
       - [Optimización de hiperparámetros](#s-231)
           
   - [**Tercera parte: Modelos Avanzados**](#s-3)
     - [Ridge](#s-311)
      - [Optimización de hiperparámetros](#s-311a)
       - [Aciertos y Desaciertos](#s-3raciertos3)   
       - [Importancia predictores](#s-311b)
     - [Lasso](#s-312)
       - [Optimización de hiperparámetros](#s-312a)
       - [Aciertos y Desaciertos](#s-3raciertos4)
       - [Importancia predictores](#s-312b)
    - [xgboots](#s-32)
       - [Optimización de hiperparámetros](#s-321)
       - [Aciertos y Desaciertos](#s-3raciertos5)
       - [Importancia de predictores](#s322)
    - [RandomForest](#s-33)
       - [Aciertos y Desaciertos](#s-3raciertos6)
       - [Optimización de hiperparámetros](#s-331)
       - [Importancia predictores](#s-332)
      
  - [**Comparación modelos**](#s-4) 
  
  - [**Conclusiones**](#s-5)
  
  [**Extra**](#s-6)
    - [Detección de outliers de forma gráfica](#s-61)
