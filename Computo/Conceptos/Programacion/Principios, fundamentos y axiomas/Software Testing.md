#### Los objetivos del testing

- Verificar errores y asegurarse que el producto funciona como se especifico.
- Asegurarse que el producto cumple con los estandares de la industria.
- Resolver posibles problemas en produccion.
- Prevenir futuras disfunciones del producto.


#### Caracteristicas de los test
- Practicos.
- Confiable.
- Autenticos.
- Apto para encontrar errores.
- Apto para verificar la validez del software.

## Metodos de software testing

- ### **Functional testing**
	*Proceso de validar la utilidad del software con respecto a sus especificaciones.*
	Estos son algunos ejemplos de testing funcional:
	- Unit Testing: Prueba unidades individuales o funciones en el codigo fuente. Puede ser implementado automatico o manual.
	- API Testing: Valida el consumo de una API verificando su fiabilidad, seguridad y efectividad con respecto al producto que la consume.
	- UI Testing/Acceptance Testing: Prueba de la interfaz del usuario que verifica los requerimientos de la interfaz se implementaron de la manera en que se especificaron
	- Integration Testing: Prueba las relaciones de componentes/unidades separados en su proposito con el fin de verificar que realmente su relacion funcional se cumple.
	- Regression Testing: Verifica el producto de software como un todo
+ #### **Non-functional testing** 
	*Valida el rendimiento del software.*
	Estos son algunos ejemplos de testing no-funcional
	- Volume Testing: Verifica que la cantidad de datos con el que el software puede lidiar
	- Security Testing: Verifica la seguridad del software requerida para el proteccion de riesgos y amenazas (autenticacion, autorizacion, confidencialidad, etc). 
	
##### Las 3 A del diseño de testing
- **Arrange**: Se refiere a la preparacion del test y su flujo de ejecucion. Se inicializan o declaran variables, se instancian objetos, se referencian datos especificos y se ligan a constantes y demas.
- **Act**: Seccion donde el codigo/funcionalidad de interes se pone a prueba
- **Assert**: Representa el resultado aprobatorio. Se define la salida/comportamiento esperado por el codigo/funcionalidad puesto a prueba


