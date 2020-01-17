## redux-starter

 redux mantiene el estado de la aplicación previsible :
    - todo el estado unificado en una misma ubicación
    - el estado es read-only, solo puede ser modificado por las acciones
    - el estado permanece inmutable es decir vuelve a su estado original

    dentro de un reducer no se puede mutar sus argumentos, hacer llamadas tipo api y llamar funciones predeterminadas javascript
    • para agregar datos al state:
    	push agrega un elemento al state osea viola el principio de no modificar el estado inicial
    	concat crea un nuevo array con el estado agregandole el nuevo elemento
    • para eliminar datos del state:
    	utilizamos filter que crea un nuevo array con el estado anterior menos el elemento a borrar
