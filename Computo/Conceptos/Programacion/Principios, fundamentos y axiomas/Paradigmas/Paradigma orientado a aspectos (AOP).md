### Unidades de manipulacion
- ##### **Business object**
Es una clase que contiene la logica del negocio. No contiene implementacion de logica adicional a esta.

```java
public class SampleAdder { 
	public int add(int a, int b) { 
	return a + b; 
	} 
}

```

- **Aspect**
Es una modularizacion de una preocupacion/problema de la solucion que se divide en multiples clases.
 ^9cd53b
```java
public class AdderAfterReturnAspect { 
	private Logger logger = LoggerFactory.getLogger(this.getClass()); 
	public void afterReturn(Object returnValue) throws Throwable { 
		logger.info("value return was {}", returnValue); 
	} 
}

```
- **Joinpoint**
Es un punto durante la ejecucion de un programa, como la ejecucion de un metodo o el manejo de una excepcion
 ^86245c
- **Pointcut**
Es un predicado que ayuda a enlazar un [[Paradigma orientado a aspectos (AOP)#^3b986a|Advice]] para ser aplicado por un [[Paradigma orientado a aspectos (AOP)#^9cd53b| Aspect]] a un particular [[#^86245c|Joinpoint]]

- **Advice**
Es una accion tomada por un particular [[Paradigma orientado a aspectos (AOP)#^86245c|Joinpoint]]. Diferentes tipos de **Advice** incluyen los verbos "al rededor", "antes", "despues" ^3b986a