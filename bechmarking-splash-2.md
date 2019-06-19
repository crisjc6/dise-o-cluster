# Benchmarking Splash 2

# CONTENIDO

* [](#id1)

El objetivo de la actualización de splash a splash-2 es la siguiente:

* Representar una gama más alta en el computo en el ámbito científico
* Usa mejores algoritmos e implementaciones.
* Una mayor consistencia arquitectónica. 

### Características 

#### Coocurrencia y balanceo de carga

Característica de un programa que me indica cuantos procesadores están siendo utilizados efectivamente por ese programa, 
asumiendo que se tiene perfecta memoria del sistema y arquitectura de comunicación.
Esto indica si un programa con un determinado conjunto de datos es apropiado para evaluar la arquitectura
de comunicación de una máquina de una escala determinada. Por ejemplo, si un
programa no representa cierta velocidad en su ejecución, puede no ser apropiado para evaluar una maquina a gran escala.
  
#### Conjuntos de trabajo de un programa

El ajuste del conjunto de trabajo en el caché puede tener un impacto tremendo en
ancho de banda de memoria local, así como en las necesidades de comunicación. Eso
Por lo tanto, es crucial para comprender los tamaños y la escala de los conjuntos de trabajo importantes, de modo que los parámetros de la máquina y la aplicación se puedan elegir de manera que representen situaciones realistas.
Como veremos, el ajuste de los conjuntos de trabajo puede ayudarnos a eliminar la
dimensión del tamaño de la caché del espacio de parámetros.

#### Relación comunicación a computación 


indica el potencial impacto de la latencia de comunicación en el rendimiento, así como las necesidades potenciales de ancho de banda de la aplicación.

El impacto en el rendimiento real y las necesidades de ancho de banda son más difíciles de predecir, ya que dependen de muchas otras características como de la cantidad de información enviada(burstiness).
De la comunicación y de cuánta latencia se oculta.




#### Localidad Espacial 

Si se hace referencia a una ubicación de almacenamiento particular en un momento determinado,
es probable que se haga referencia a ubicaciones de memoria cercanas en un futuro próximo. 
En este caso, es común intentar adivinar el tamaño y la forma del área alrededor de
la referencia actual para la cual vale la pena preparar un acceso más rápido para la referencia posterior.

Además del uso compartido falso o false-sharing es un patrón de uso que puede reducir el rendimiento de cachés distribuidas 
  con coherencia en los bloques de recurso de tamaño más pequeño gestionado por el mecanismo de caché.
  
 ### Tabla 1
 
 ![image](https://user-images.githubusercontent.com/50051312/59788003-56c1d400-9290-11e9-8643-735cc4b33451.png)

  
### Conclusión 
El conjunto de aplicaciones SPLASH-2 está diseñado para proporcionar
Programas para la evaluación de ideas arquitectónicas y optimización (trade-offs).
Sin embargo, realizar dicha evaluación bien es una tarea difícil debido a que
a la gran cantidad de grados de libertad que interactúan. Por ejemplo,
muchos parámetros del sistema de memoria, como el tamaño del caché, la asociatividad y el tamaño de la línea, pueden impactar cuantitativa y cualitativamente en la recuperación.
Los resultados de un estudio, al igual que los parámetros de aplicación y el número de procesadores utilizados.


### Enlaces 

 [The SPLASH-2 Programs: Characterization
and Methodological Considerations](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.48.2356&rep=rep1&type=pdf)
