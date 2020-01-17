## redux-starter

redux mantiene el estado de la aplicación previsible : todo el estado unificado en una misma ubicación, el estado es read-only, solo puede ser modificado por las acciones, el estado permanece inmutable es decir vuelve a su estado original

dentro de un reducer no se pueden mutar sus argumentos, hacer llamadas tipo api ni llamar funciones predeterminadas javascript, estas acciones se ejecutan fuera del reducer y ejecutan dispatch que generan acciones que modifican el estado y a traves de un subscribe el store lanza funciones de renderización.
    
   • para agregar datos al state:
    	push agrega un elemento al state osea viola el principio de no modificar el estado inicial
    	concat crea un nuevo array con el estado agregandole el nuevo elemento
   • para eliminar datos del state:
    	utilizamos filter que crea un nuevo array con el estado anterior menos el elemento a borrar
     
Fetch axios < (efecto externo al renderizar) - lanza un dispatch
socket.io < (efecto externo durante tiempo de ejecución) - lanza un dispatch
react actions < (efecto interno durante tiempo de ejecución) - lanza un dispatch en la ejecución de botones
redux • (efecto transversal de unificación y almacenamiento del state en localstorage) 
