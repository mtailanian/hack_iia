# Análisis de datos y predicción de Fraude en Transacciones asociadas a Tarjetas de Crédito 

## Introducción

En este NoteBook se realiza un análisis de los datos de fraude asociados a un conjunto de 284.807 transacciones de tarjetas de crédito. Además se utiliza un modelo predictivo con el fin de detectar transacciones fraudulentas. El modelo predictivo a desarrollar se basa en una red neuronal implementada con la biblioteca Tensorflow.


Cabe desatcar que el conjunto de datos ha sido anonimizado para la confidencialidad y las características V1, ..., V28 son producto del analisis por componentes principales de una transformación de PCA. Acemás hay otras tres variables: monto, clase, tiempo. El monto indica la cantidad de dinero de la transacción, la clase denota si la transacción es fraudulenta (1) o normal (0). El tiempo es un número entero que indica el tiempo transcurrido desde la primera transacción en segundos. Todo el conjunto de datos corresponde a dos días de transacciones con tarjeta de crédito.


## Conjunto de datos

#### Contexto
Es importante que las compañías de tarjetas de crédito puedan reconocer las transacciones fraudulentas con tarjeta de crédito para que no se les cobre a los clientes por los artículos que no compraron.

#### Datos

El conjunto de datos ha analizar contiene transacciones realizadas con tarjetas de crédito en setiembre de 2013 por titulares de tarjetas europeos. Este conjunto de datos presenta las transacciones que ocurrieron en dos días, donde tenemos 492 fraudes en un total de 284.807 transacciones. El conjunto de datos es altamente desequilibrado, la clase positiva (fraudes) representa el 0.172% de todas las transacciones.

Contiene sólo variables de entrada numéricas que son el resultado de una transformación de PCA. Desafortunadamente, debido a problemas de confidencialidad, no podemos proporcionar las características originales y más información de fondo sobre los datos. Las características V1, V2, ... V28 son los componentes principales obtenidos con PCA, las únicas características que no se han transformado con PCA son (tiempo) 'Time' y (monto)'Amount'. La característica 'Time' contiene los segundos transcurridos entre cada transacción y la primera transacción en el conjunto de datos. La carácteristica 'Amount' es el monto de la transacción. Por último la característica 'Clase' es la "Clasificación" y toma el valor 1 en caso de fraude y 0 en caso contrario.

El conjunto de datos ha sido recopilado y analizado durante una colaboración de investigación de Worldline y el Machine Learning Group (http://mlg.ulb.ac.be) de la ULB (Université Libre de Bruxelles) sobre minería de datos grandes y detección de fraude. Más detalles sobre proyectos actuales y pasados ​​sobre temas relacionados están disponibles en http://mlg.ulb.ac.be/BruFence y http://mlg.ulb.ac.be/ARTML


# Referencias
Andrea Dal Pozzolo, Olivier Caelen, Reid A. Johnson y Gianluca Bontempi. Calibración de la probabilidad con submuestreo para la clasificación desequilibrada. Simposio sobre Inteligencia Computacional y Minería de Datos (CIDM), IEEE, 2015.

Repositorio: https://github.com/Currie32/Predicting-Credit-Card-Fraud


# Exploración de datos
El propósito de este trabajo es identificar transacciones fraudulentas con tarjeta de crédito.

Primero cargamos las bibliotecas requeridas y el conjunto de datos con el que vamos a trabajar.

Echemos un vistazo a la estructura del conjunto de datos y hagamos algunos análisis!

