### Imperativo
El paradigma imperativo se refiere al mismo concepto que el paradigma estructurado. Sus caracteristicas son:

- Formar el flujo de control explicitamente
- Afirmar explicitamente los pasos a seguir (como deberia continuar el flujo de ejecucion el algoritmo)
>Es como decirle a un chef paso por paso como hacer una pizza.

- Compartir el estado (la preocupacion en el diseño de un algoritmo que permita a todos los flujos interconectarse y trabajar conjuntamente para la continuacion del flujo de ejecucion).



### Declarativo
Se forma la solucion por lo que se deberia hacer. Sus caracteristicas son:
- Formar el flujo de control implicitamente
- No produce reacciones colaterales
>Es como ordenar una pizza  sin ser consciente de todo lo que tuvo que suceder para crear la pizza

| Caracteristica                  | Acercamiento imperativo                                                        | Acercamiento funcional                                           | Acercamiento orientado a objetos                                                                |
| ------------------------------- | ------------------------------------------------------------------------------ | ---------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- |
| Atencion del programador        | Como realizar las tareas (algoritmos) y como rastrear los cambios en el estado | Que informacion es deseada y que transformaciones son requeridas | Diseño de jerarquia de clases,  encapsulacion y preocupacion por terminos de contratos de clase |
| Cambio de estado                | Importante                                                                     | No existente                                                     | Primordiales                                                                                    |
| Orden de ejecucion              | Importante                                                                     | Poca importancia                                                 | Utilizacion de clases, interfaces, herencia, y polimorfismo                                     |
| Flujo de control primario       | Loops, condicionales y llamadas a funcion (metodos)                            | Llamadas a funcion, inclusion de recursion                       | Instancia de clases                                                                             |
| Unidad de manipulacion primaria | Instancias de estructuras o clases                                             | Colecciones de datos y funciones de primera clase como objetos   | Clases, instancias y llamados estaticos                                                                                                |



#evolucion_paradigmas
En relacion a los 2 paradigmas los subparadigmas de programacion evolucionaron una perspectiva especifica:
- ###### Paradigma estructural
	- Flujo de transferencia de control y restriccion de uso de **goto** con palabras reservadas como: **if/else/then/loop** y otras.
	- Limita el flujo de control.
- ##### [[Paradigma orientado a objetos]]
	- Restringe la programacion con el polimorfismo como punteros hacia distintas funciones con nombres iguales.
- ##### [[Paradigma funcional]]
	- Restringe los estados compartidos y efectos colaterales introduciendo la inmutabilidad.
- ##### Paradigma orientado a aspectos (AOP)
	- Busca incrementar la modularidad permitiendo la separacion de problemas transversales.
	- Busca la reutilizacion separando codigo en modulos que se pueden compartir.