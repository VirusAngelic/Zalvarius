##### User Story
Es un enunciado informal que describe las funcionalidades de un sistema. Son escritos desde la perspectiva del usuario generalmente aunque es posible escribirlos desde la perspectiva de otro rol implicado en el diseño del software.

##### Test Suite
Grupo de test categorizados por tipo/finalidad del test. Se puede referir a un archivo con funciones o clases de un tipo de test especifico o bien a un conjunto de archivos en una carpeta los cuales incluyen un tipo de test concreto.

##### Stateful
Implementacion que provoca el almacenamiento de informacion de registros acerca de eventos o actividades del usuario teniendo un conjunto de informacion acerca de sus interacciones.

##### Stateless
Implementacion que provoca la omision del registro de informacion latente sobre los eventos o actividades del usuario en un sistema. 

##### Paradigma de programacion
	![[Pasted image 20221031234421.png]]

##### **Block Storage**
Administrado por un sistema libre desacoplado de entornos como Linux y Windows, almacena los datos en distintos bloques separados que al ser solicitados dependiendo del requerimiento del entorno.

##### **File Storage**
Los datos se almacenan jerarquicamente (sistema **file-level**/**file-based**). La metadata de la informacion almacenada es limitada, contando unicamente con el path para referenciar a datos almacenados. Solo es posible escalarlos con mas dispositivos que a su vez agreguen un sistema **File Storage**. 

##### **Routing**
Una solucion para el cambio de interfaces de usuario dinamicamente a peticion del usuario o flujo de algun aplicativo sin hacer una peticion de recursos. Por ejemplo: El **routing** de una pagina web puede evitar que un explorador vuelva a hacer un request de una pagina diferente al servidor que se este esperando acceder mediante la renderizacion de la nueva pagina mostrada  y la eliminacion de la anterior.

##### Web Service
Es un sistema de software que esta diseñado para ser interoperable maquina a maquina sobre una red.
Desglosando las 3 características fundamentales:
- Diseñado para la interacción entre maquina a maquina (aplicación a aplicación): Permite la interaccion entre diferentes sistemas de software
- Debería permitir la interoperabilidad. Sin depender de la plataforma: No importa el lenguaje sobre el que este programado o de que manera, si su diseño fue realizado pensando en su consumo.
- Debería permitir la comunicación vía red