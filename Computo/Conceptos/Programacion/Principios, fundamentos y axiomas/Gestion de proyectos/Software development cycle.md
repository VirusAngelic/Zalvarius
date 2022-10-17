## Estrategias de desarrollo de software

#### Test-First Programming
#testing
Se emplea trabajando primero en codificar los **test** para posteriormente trabajar en la implementacion de la solucion del problema. De esta manera se trabajar en la reafirmacion de los requisitos del usuario a traves de un **[[Software Testing#Metodos de software testing| Functional testing]]** .
![[Pasted image 20220921082102.png]]

Esto reduce el numero de bugs, incrementa la productividad y afecta positivamente al tiempo de todo el equipo de desarrollo cortando el feedback loop. 

![[Pasted image 20220921082740.png]]

#### Test-Driven Development
![[Pasted image 20220921085328.png]]
Debido a casos en donde el diseño de la solucion puede no encajar con un ciclo de **Testing/Coding** , es posible decir que un ciclo de desarrollo inverso puede conducir a un diseño donde fue influenciado por la implementacion que a su vez fue influenciado por el test (la verificacion de los requerimientos del sistema). Permitiendo que el diseño contenga una factorizada implementacion (Uso de patrones de diseño) nos otorga la certeza que el diseño contiene el suficiente codigo enfocado a cumplir con los requisitos del sistema.
![[Pasted image 20220921084547.png]]

#### Behavior-Driven Development
Integra la etapa de analisis en el ciclo de desarrollo de manera que se tiende a dividir las funcionalidades del sistema como un todo en pequeñas unidades.
![[Pasted image 20220921101558.png]]

Desde el dia uno de desarrollo se produce una **suite test** que mantiene al sistema entero completamente verificable en relacion con los requerimientos del usuario.

![[Pasted image 20220921101904.png]]