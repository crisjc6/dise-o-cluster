# Diseño de cluster

**By** Cristhian Jumbo

**Multiprocesamiento y arquitectura alternativas**

#### Implementar un diseño cluster para la industria de los circuitos electrónicos

# CONTENIDO

* [Tema](#id1)

* [Nodos para la implementación.](#id2)

* [Conexiones de red.](#id3)

* [Almacenamiento.](#id4)

* [Sistema Operativos.](#id5)

* [Ambiente de programación.](#id6)

* [Aplicaciones.](#id7)

* [Justificación de uso.](#id8)
  
* [Conclusiones y Recomendaciones.](#id9)

* [Enlaces.](#id10)

<a name="id1"></a>

# TEMA 

### Palabra claves 
* Computo paralelo
* Cluster
* Procesamiento de señales digitales


**Implementar un diseño cluster para la industria de los circuitos electrónicos**

#### Señales digitales
dentro de los circuitos eléctricos se tiene el procesamiento de señales digitales.

Son mas económicos que los circuitos análogo, además existe un poco mas de seguridad.

Permite realizar tareas muy complejas conocidas como señales de alta fidelidad.

**Diseño de cluster para el procesamiento de señales digitales en la electrónica**

El primer paso para el diseño de una solución cluster es escoger el tipo de cluster que vamos a necesitar para el caso del procesamiento de la señales digitales se necesitara que sea en tiempo real y aparte que sea escalable permitiendo incluir más hardware sin que afecte el procesamiento del cluster esto si el trabajo de procesamiento aumenta. 

**OpenMosix**: La idea de este modelo de cluster es que la distribución de tarea las realizar de forma dinámica conforme se van creando las tareas. Cuando un nodo está demasiado cargado las tareas que se están ejecutando pueden migrar a cualquier otro nodo del cluster sin que el proceso sufra mayores cambios. Además, este modelo funciona a nivel del kernel por lo tanto puede conseguir todas la información 

Una vez elegido el modelo de cluster se procede a especificar las características de cada nodo 

![image](https://user-images.githubusercontent.com/50051312/59373982-6a10f480-8d10-11e9-9f01-9f079d12646a.png)




<a name="id2"></a>
# NODOS

Nodo conocido como cualquier servidor que puede formar parte del cluster tienes que tener las mismas capacidades y características a nivel de hardware.

<a name="id3"></a>
# CONEXIONES DE RED
Todos los nodos deben estar conectados entre para ello se requiere una conexión de red para esta diseño de cluster se requerirá de un sistema del tipo  GigabitEthernet (1/10Gbps)  ya que es la mas utilizada actualmente. presentando un mayor rendimiento en los clusteres 

<a name="id4"></a>
# Almacenamiento 

Este puede interno o externo con las diferentes tecnologías.

* IDE ATA de hasta 166M/s
* SATA de hasta 600 M/s
* SCSI de hasta 640 M/s

<a name="id5"></a>
# SISTEMAS OPERATIVOS

Los sistemas operativos a utilizar deben soportar el manejo de hilos, open source para este diseño de cluster se podrá elegir entre las distribuciones de linux ya que permite tener un soporte multiproceso y multiusuario. para gestión en GNU/linux existe **conga** es una herramienta que me permite realizar la gestión de los nodos del cluster.


<a name="id6"></a>
# AMBIENTE DE PROGRAMACION

Son los que permiten que se pueda hacer uso los diferentes recursos con los que se cuenta dentro del cluster, entre estos podemos mencionar uno muy importante como CPU, la memoria los datos.

Una de las manera de referenciar el rendimiento se relaciona con un termino nuevo denominado FLOPS (operaciones en como flotante por segundo). Esta es una medida común cuando se habla del desempeño computacional, especialmente en el uso de operaciones científicas, que requieren de gran consumo de recursos.

<a name="id7"></a>
# APLICACIONES 
Por lo general es el software que permite la comunicación entre aplicaciones, hardware u otros sistemas operativos.
Su principal objetivo es ser intermediarios en la comunicaciones facilitar en trabajo de los desarrolladores cuando se hace necesario generar   diferentes conexiones entre los sistemas.

La aplicación necesaria para el procesamiento de señales será una aplicación de tiempo real, por lo que el diseño del cluster incluirá un cluster de tipo de alta disponibilidad y escalabilidad para que se puedan agregar nuevos cluster si el trabajo aumentara.




<a name="id8"></a>
# JUSTIFICACION

La razón por la que se debería implementar un cluster que permita el procesamiento de señales digitales dentro de la industria de los circuitos electrónicos es la siguiente:

El procesamiento de señales digitales ha sido una tarea que se distingue por su alto requerimiento de procesamiento de datos, lo que lleva al diseño de la implementación de un sistema cluster.

Las diferentes aplicaciones que se puede ejecutar a gran escale en el procesamiento de las señales digitales como:

* Procesamiento de audio digital
* Procesamiento de voz digital
* Procesamiento de imágenes digitales 
* Procesamiento de video digital
* Procesamiento de datos digitales


El procesamiento digital de señales (PDS) hasta la fecha se ha realizado con sistemas de computadores en su mayoría de un solo procesador. El tipo de procesador define la forma en que el algoritmo del procesamiento de señales digitales (PDS). Estos procesos definidos por la cantidad de núcleos de procesador y estos en su mayoría son altamente realizable sen paralelo. Todo esto permitiendo acelerar los procesos de las tareas y una mayor eficiencia.



## Arquitectura de comunicación

![image](https://user-images.githubusercontent.com/50051312/59375910-bcecab00-8d14-11e9-82b9-93fda8cb36b8.png)

<a name="id9"></a>
# CONCLUSIOENS Y RECOMENDACIONES

*  Se pudo comprobar que un efecto cluster puede reducir el tiempo de ejecución en el procesamiento de las señales digitales de cualquier aplicación, aumentando el rendimiento de las maquinas maximizando la utilización de los recursos disponibles.

* La evolución de los computadores paralelos ha sido clara en varias direcciones, una de las cuales es la utilización de hardware de computo estándar. En este sentido los microprocesadores de uso masivo en los computadores de bajo costo como las estaciones de trabajo y PC´s son utilizados en las implementaciones de clusters 

<a name="id10"></a>
# ENLACES


https://es.slideshare.net/Doyler83/componentes-de-un-clster

http://scielo.sld.cu/scielo.php?script=sci_arttext&pid=S2227-18992015000500002

http://repositorio.utp.edu.co/dspace/bitstream/handle/11059/8945/T005.8%20M539.pdf?sequence=1&isAllowed=y

http://repositorio.puce.edu.ec/bitstream/handle/22000/9583/Disertacion_de_grado_Gabriel_Andrade.pdf?sequence=3&isAllowed=y
