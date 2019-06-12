# Diseño de cluster

Implementar un diseño cluster para la insdustria de los circuitos electronicos

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

<a name="id1"></a>

# TEMA 

Implementar un diseño cluster para la insdustria de los circuitos electronicos

**Diseño de cluster para el procesamiento de señales digitales en la electronica**

El primer paso para el diseño de una solucion cluster es escoger el tipo de cluster que vamos a necesitar para el caso del procesamiento de la señales digitales se necesitara que sea en tiempo real y aparte que sea escalable permitiendo incluir  mas hadware sin que afecte el prosesamiento del cluster esto si el trabajo de procesamiento aumenta. 

### Palabra claves 
* Computo paralelo
* Cluster
* Procesamiento de señales digitales

### Señales digitales
dentro de los circuitos electricos se tiene el procesamiento de señales digitales.
son mas economicos que los circuitos analogo, ademas existe un poco mas de seguridad.
Permite realizar tareas muy complejas conocidas como señales de alta fidelidad.


<a name="id2"></a>
# NODOS

Nodo conocido como cualquier servidor que puede formar parte del cluster tienes que tener las mismas capacidades y caracteristicas a nivel de hardware.

<a name="id3"></a>
# CONEXIONES DE RED
Todos los nodos deben estar conectados entre para ello se requiere una conexion de red para esta diseño de cluster se requerirá de un sistema del tipo  GigabitEthernet (1/10Gbps)  ya que es la mas utilizada actualmente. presentando un mayor rendimiento en los clusteres 

<a name="id4"></a>
# AlMACENAMIENTO 

Este puede interno o externo con las diferentes tecnologias.

* IDE ATA de hasta 166M/s
* SATA de hasta 600 M/s
* SCSI de hasta 640 M/s

<a name="id5"></a>
# SISTEMAS OPERATIVOS

Los sistemas operativos a utilizar deben soportar el manejo de hilos, open sourse para este diseño de cluster se podra elegir entre las distribuiones de linux ya que permite tener un soporte multiproceso y multiusuario. para gestion en GNU/linux existe **conga** es una herramienta que me permite realizar la gestion de los nodos del cluster.


<a name="id6"></a>
# AMBIENTE DE PROGRAMACION

Son los que permiten que se pueda hacer uso los diferentes recursos con los que se cuenta dentro del cluster, entre estos podemos mencionar uno muy importante como CPU, la memoria los datos.

Una de las manera de referenciar el rendimiento se relaciona con un termino nuevo denominado FLOPS (operaciones en como flotante por segundo). Esta es una medida comuún cuando se habla del desempeño computacional, especialmente en el uso de operaciones cientificas, que requieren de gran consumo de recursos.

<a name="id7"></a>
# APLICACIONES 
Por lo general es el software que permite la comunicacion entre aplicaciones, hardware u otros sistemas operativos.
Su principal objetivo es ser intermediarios en la comunicaciones facilitar en trabajo de los desarrolladores cuando se hace necesario generar   direfentes conexiones entre los sistemas.

La aplicacion necesaria para el procesamiento de señales sera una aplicaicon de tiempo real, por lo que el diseño del cluster incluira un cluster de tipo de alta disponibilidad y escalabilidad para que se puedan agrear nuevos cluster si el trabajo aumentara.

<a name="id8"></a>
# JUSTIFICACION

La razon por la que se deberia implementar un cluster que permita el procesamiento de señales digitales dentro de la industria de los circuitos electronicos es la siguiente:

El procesamiento de señales digitales ha sido una tarea que se distingue por su alto requerimiento de procesamiento de datos, lo que lleva al diseño de la implementacion de un sistema cluster.






https://es.slideshare.net/Doyler83/componentes-de-un-clster

http://scielo.sld.cu/scielo.php?script=sci_arttext&pid=S2227-18992015000500002

http://repositorio.utp.edu.co/dspace/bitstream/handle/11059/8945/T005.8%20M539.pdf?sequence=1&isAllowed=y

http://repositorio.puce.edu.ec/bitstream/handle/22000/9583/Disertacion_de_grado_Gabriel_Andrade.pdf?sequence=3&isAllowed=y
