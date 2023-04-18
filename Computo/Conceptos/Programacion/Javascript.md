#lenguajes_programacion

Se trata de un lenguaje de programacion con un entorno de ejecucion (regularmente el explorador web) interpretado, de un solo hilo y un solo **call stack**. Su entorno de ejecucion provee de APIs como : DOM, AJAX y **Timers**


##### Call Stack
Debido a que el lenguaje es  **single thread** implica que su **call stack** es sincrono. Se trata de una estructura de datos que usa $**LIFO (Last In, First Out)** para almacenar temporalmente y gestionar las invocaciones a las funciones.

Dentro se almacenan temporalmente las llamadas a $funcion, sus $parametros y $variables en un **stack frame**, el cual es una porcion de memoria reservada para cada $funcion a ejecutar en el **stack**. A esta informacion de la funcion se le conoce como el contexto de la funcion.

Una funcion se considera fuera del **call stack** unicamente cuando retorna.

![[Pasted image 20230417210316.png]]

El **call stack** mantiene un registro de la posicion de cada **stack frame**, sabe cual es la siguiente funcion a llamar y se encarga de removerla de la $pila una vez terminada la ejecucion.

##### Event Loop
Es un proceso $coordinador de javascript que coloca una llamada al **call stack** una vez se encuentra disponible para su ejecucion una funcion asincrona que esperaba por un evento para continuar con su ejecucion. Esto ayuda a evitar el hilo en tiempo de ejecucion de javascript espere por una funcion que no termina aun, permitiendo y dando la ilusion de concurrencia.

En la siguiente imagen se aprecia como la pila de Web API monitorea el contador de la funcion task.
![[Pasted image 20230417212719.png]]

Y al estar disponible para su ejecucion, event loop la retoma para continuar
![[Pasted image 20230417212724.png]]

##### DOM
#document_object_model
Es una acronimo para **Document Object Model**. Representa la estructura de datos de una pagina web para el navegador web.

Contiene la estructura de la pagina en objetos, los cuales contienen:
- Contenido: El contenido de la pagina a mostrar
- Elementos estructurales: Elementos que organizan como se presenta la pagina web en el navegador
- Atributos: Se refiere a las propiedades de los elementos: Clases, estilos, tamaños de los elementos por mencionar algunos ejemplos.
- Nodos: Son todos los componentes que forman al DOM (texto, divs, etiquetas h2, etiquetas a)
- Elemento: Son tipos de nodos que le dan estructura grafica al documento(todas las etiquetas html, pero no contenido como por ejemplo texto)

![[Pasted image 20230417213623.png]]

##### BOM
#browser_object_model
Es un acronimo para **Browser Object Model** y se refiere a una API ofrecida por todos los navegadores para acceder a funcionalidad del entorno de ejecucion de javascript, es decir el navegador web.

##### Event bubbling
Es un comportamiento por default de javascript. Se refiere a la propagacion de los eventos desde el nodo hijo donde de origino el evento hasta el nodo padre que contiene a ese hijo. Sucede en las siguientes fases:

![[Pasted image 20230417215323.png]]

- Fase de captura: Se busca el elemento mas profundo en el DOM que tenga registrado en evento en su listener.
- Fase de target: Ejecuta el evento del elemento en si.
- Fase de burbuja: Verifica si los elementos padre de dicho elemento tienen eventos registrados en sus listeners, si es asi, ejecuta dichos eventos de manera automatica.

##### Hoisting
Se refiere a un comportamiento del lenguaje que permite que todas las declaraciones de funciones o variables sean movida al prinicpio del codigo, permitiendo utilizar variables o llamadas a funciones incluso antes de ser declaradas. Al menos visiblemente en el codigo fuente.