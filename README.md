## Proyecto4_Acamica

El objetivo de este proyecto es profundizar en el proyecto 3 para el desarrollo de un sistema de recomendación para la plataforma de juegos Steam. Este fué desarrollado como la cuarta entrega del curso de Data Science de la plataforma de enseñanza [Acamica](https://www.acamica.com/)

Los Datasets utilizados pueden ser descargados [aquí](https://github.com/kang205/SASRec). Consta de un Archivo de Reseñas (reviews) y uno con la información del juego (game info).

Es desarrollado en lenguaje Python y utiliza las librerias Numpy, Scipy, Pandas, Matplotlib, Seaborn, Implicit, Scikit-Learn y Scikit Optimize

Este proyecto consta de 2 secciones

A. Ánálisis exploratorio de los datos suministrados y preprocesamiento de los datos

B. Formulación y desarrollo de diferentes estrategias de sistemas de recomendación, entre las que se encuentran dos algoritmos de filtro colaborativo basado en memoria, un algoritmo de filtro colaborativo basado en modelo y un algoritmo basado en contenidos. comparación de los algoritmos por medio de la métrica precisión media promedio [MAP](https://en.wikipedia.org/wiki/Evaluation_measures_(information_retrieval)#Mean_average_precision).

La optimización de los algoritmos con multiples hiperparámetros se desarrolla por medio de un procedimiento de optimización gausiana, que es mas eficiente que la optimización por grilla utilizada en los proyectos anteriores.

El algoritmo con mejor desempeño es el de filtro colaborativo basado en modelo, de mínimos cuadrados alternantes (ALS). basado en el algoritmo presentado en el artículo [Collaborative Filtering for Implicit Feedback Datasets](http://yifanhu.net/PUB/cf.pdf). El procedimiento iterativo para la resolución de la función de costo es desarrollado en el artículo [Applications of the Conjugate Gradient Method for Implicit Feedback Collaborative Filtering](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.379.6473&rep=rep1&type=pdf).

