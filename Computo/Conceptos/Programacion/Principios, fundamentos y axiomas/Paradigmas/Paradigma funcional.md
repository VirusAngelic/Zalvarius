

### Funciones de primer orden
Un lenguaje de programacion se dice tiene funciones de primer orden si sus funciones son tratadas como cualquier otra variable. Por lo tanto, pueden ser asignadas a cualquier otra variable o pasada como argumento o puede ser retornada por otra funcion. Las propiedades son:
- Pueden ser asignadas a variables regulares
- Pasar funciones para argumentos a otras funciones
- Retornadas como el resultado de funciones
- Pueden ser incluidas en cualquier estructura de datos

Funciones asignadas a variables
---
```javascript
const string = "Foo"

const num = 2

const bool = false

const greet = (name) => `Hello ${name}`

// ... other primitive data types

greet('John') // Hello John
```

Funciones como argumentos a otras funciones
---
```javascript
const nums = [1, 2, 3, 4, 5]

const addOne = (n) => n + 1

const addedOne = nums.map(addOne) // [2, 3, 4, 5, 6]
```

Retornados como el resultado de una funcion
---
```javascript
const makeCounter = () => {

let count = 0

return () => ++count

}

const counter = makeCounter()

counter() // 1

counter() // 2

counter() // 3

counter() // 4
```

Incluido en cualquier estructura de datos
---
```javascript
const wakeUp = name => `${name}, wake up early!`

const takeShower = name => `${name}, take shower!`

const workout = name => `${name}, workout!`

const shutUp = name => `${name}, shut up!`

const morningRoutines = [

wakeUp,

takeShower,

workout,

shutUp

]

morningRoutines.forEach(routine => routine('John'))

// John, wake up early!

// John, take shower!

// John, workout!

// John, shut up!
```

### Funciones de orden alto
Una funcion que recibe otra funcion como argumento o que retorna una nueva funcion o ambas es llamada de orden alto.

| Funciones de primer orden                                                                       | Funciones de orden alto                                                     |
| ----------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| Son tratadas como una variable que puede ser reasignada a otra variable o pasada como argumento. | Reciben otra funcion como argumento o/y retorna una funcion de primer orden. |
| El concepto solo es aplicado en programacion.                                                    | Puede ser aplicado el concepto en otros campos fuera de la programacion.     |
| Su prescencia implica la prescencia de las funciones de orden alto.                              | No implica su prescencia la prescencia de funciones de primer orden.         |


### Closures
Es una funcion retornada por una funcion padre y tiene acceso  al estado interno de la funcion padre.

```javascript
const add = (x) => (y) => x + y

const add5 = add(5) // add5 = (y) => 5 + y

const add10 = add(10) // add10 = (y) => 10 + y

add5(1) // 6

add10(1) // 11
```
	Las funciones add5 y add10 son closures debido a que contiene cada una un valor definido dentro de su definicion y siguen siendo accesibles. 