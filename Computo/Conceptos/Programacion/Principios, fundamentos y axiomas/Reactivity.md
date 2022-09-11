### Reactivity

#conceptos_iniciales #fundamentos
Se definen las siguientes propiedades del tipos de datos tomando como referencia los siguientes principios:

- Un valor/valores son obtenidos #getter
- Un valor/valores son establecidos #setter
- Un valor/valores seran/fueron obtenidos #getter
- Un valor/valores seran/fueron establecidos #setter

###### ***Value***
#espaciales
Se refiere a un  singular y espacial tipo de dato en determinado tiempo concreto

###### ***Array***/Coleccion
#espaciales
Es una coleccion plural y espacial de un tipo de dato o n tipo de datos en determinado tiempo concreto

###### ***Deferred***
#eventual 
Se refiere a un singular y eventual valor que se espera sea asignado en algun momento

###### ***Stream***
#eventual 
Se refiere a una coleccion plural y eventual de un tipo de dato o n tipos de datos que se espera sean determinado o fueron determinado en algun momento

###### ***Promise***
#eventual #conceptos_heredados #getter 
Es un **getter** asincrono cuyo valor puede ser obtenido en algun momento o pudo haber sido obtenido para un solo valor

###### ***Resolver***
#eventual #setter #conceptos_heredados 
Es un **setter** asincrono cuyo valor se asigna/procesa en algun momento

###### ***Reader***
#eventual #getter 
Es un **getter** asincrono cuyos valores (notese el plural) pueden ser obtenidos o fueron obtenidos en algun momento para un conjunto de valores

###### ***Writer***
#eventual #setter 
Es un **setter** asincrono cuyos valores (notese el plural) pueden ser obtenidos en algun momento para un conjunto de valores

| Interface |        |          |          |
| --------- | ------ | -------- | -------- |
| Value     | Value  | Singular | Plural   |
| Getter    | Getter | Singular | Espacial |
| Setter    | Setter | Singular | Espacial |
| Array     | Value  | Plural   | Espacial |
| Iterador  | Getter | Plural   | Espacial |
| Generador | Setter | Plural   | Espacial |
| Deferred  | Value  | Singular | Temporal |
| Promise   | Getter | Singular | Temporal |
| Resolver  | Setter | Singular | Temporal |
| Stream    | Value  | Plural   | Temporal |
| Reader    | Getter | Plural   | Temporal |
| Writer    | Setter | Plural   | Temporal         |
