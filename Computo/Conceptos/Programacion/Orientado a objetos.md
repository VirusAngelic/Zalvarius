aliases: [Programacion, progra, POO, lenguajes, languages]
[[Orientado a objetos]]

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