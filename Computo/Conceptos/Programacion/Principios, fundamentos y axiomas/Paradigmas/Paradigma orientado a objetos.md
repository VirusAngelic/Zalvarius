aliases: [Programacion, progra, POO, lenguajes, languages]

### Clases
#clases
Las clases no ejecutan nada
	Consideraciones:
	- En java aquella clase donde se especifique el metodo main determinara la logica del negocio

### Objetos
#objetos
Son instancias (una copia en ejecucion) de una clase con un contexto determinado por su creacion en tiempo de ejecucion
	Consideraciones:
	- Cada objeto tiene su propio espacio de ejecucion en memoria
	- Las propiedades o metodos con "static" implican que son independientes de la instancia de aquel objeto al cual estan siendo referenciadas
	- Los objetos se pueden instanciar solo en terminos de un **supertype** debido al principio de substitucion

### Metodos
#metodos
Son funciones que pertenecen a una clase y estan ligadas a la ejecucion de cada objeto

### Metodo constructor
#metodos 
Es una funcion especial ejecutada cuando un metodo se inicializa que contiene o no logica al ejecutar.
	Consideraciones:
		- Puede contar o no con parametros. El constructor default no contiene parametros
		- Existe un constructor default que siempre se ejecuta y contiene una referencia a la clase padre de  aquella clase se este tratando

Los constructores cuenta con el mismo nombre de la clase
```java 
public Cars(){
	//Codigo a ejecutar para el contructor por default
}
```


En una instanciacion de alguna clase (creacion de objeto) se puede instanciar al constructor de una clase padre o aquella a la que se haga referencia



### Principios SOLID

#### S
Single Responsability Principle
#prinicpio_de_responsabilidad_unica
Se pretende que cada clase sea responsable de una unica parte de la funcionalidad proporcionada.


#### O
Open/Close
#principio_abierto_cerrado
La adicion de nueva funcionalidad, extendiendo asi un tipo; debe ser permisible para que cualquier tipo hijo pueda obtener parte de la funcionalidad del padre y extenderse, por este principio, la funcionalidad requerida

#### L
Liskov Substitution Principle
#principio_de_substitucion 
>Los **subtypes** deben ser capaces de poder ser reemplazados en terminos de **supertypes**

Cada subclase debe de permanecer compatible con el comportamiento de la superclase (clase padre).  Se deben de cumplir los siguientes requisitos para lograr el cumplimiento de este prinicpio:

- *Argumentos de **types***: Argumentos de los **types** hijos deben ser equivalentes o mas que aquellos argumentos del padre
	- Los tipos de parametros en el metodo de una subcclase deben coincidir o ser mas abstractos que los tipos de parametros del metodo de la superclase
***************************************************************
- *Retorno de **types***: El retorno de los **subtypes** debe ser menor o equivalente que los retornos de aquellos metodos sobreescritos
	- El tipo de retorno en el metodo de una subclase debe coincidir o ser un subtipo del tipo de retorno del metodo de la superclase
***************************************************************
- *Excepciones*: Las excepciones que un **subtype** puede ser disparar deben ser menores o iguales a las del **supertype** 
	- Un metodo de una subclase no debe arrojar tipos de excepciones que no se espere que arroje el metodo base
***************************************************************
- *Invariabilidad*: Los **subtypes** deben permanecer invariables en aquellos limites o definiciones que los **supertypes** definieron desde el principio
	- Los invariantes de una superclase deben preservarse. Los invariantes son propiedades que definen el tipo de clase u objeto que se diseña en el sistema de tal manera que su ausencia no definiria en mas el tipo del cual se este tratando
***************************************************************
- *Historico de restricciones*: Los **subtypes** deben respetar las restricciones que los **supertypes** definieron sin importar si se requieren alterar en la implementacion futura
- *Precondiciones*: Los **subtypes** pueden relajar las restricciones que los **supertypes** implementan pero no deben acortarlas aun mas que las ya establecidas en los **supertypes**, permitiendo asi que los reemplazos de **subtypes** en terminos de **supertypes** sean permitidos
	- Una subclase no debe fortalecer las condiciones previas
***************************************************************
- *Postcondiciones*: Los **subtypes** pueden fortalecer las restricciones que los **supertypes** implementan pero no deben relajarlas mas, permitiendo que teniendo postcondiciones mas robustas que los supertypes las condiciones permitan reemplazar **subtypes** en terminos de **supertypes**. Mientras que postcondiciones mas endebles no garantizan que las postcondiciones de los **subtypes** sean reemplazables en terminos de **supertypes**
	- Una subclase no debe debilitas las condiciones posteriores
***************************************************************
- *Modificadores de acceso inmutables*: Evitar cambiar los campos



