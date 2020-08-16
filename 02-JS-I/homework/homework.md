1. En un archivo de texto separado que debes crear, escribe explicaciones de los siguientes conceptos como si se lo estuvieras explicando a un niño de 12 años. Hacer esto te ayudará a descubrir rápidamente cualquier agujero en tu comprensión.

	* Variables
        Son espacios reservados en la memoria, para guardar un dato, tienen una clave/identificador para llamarlos, modificarlos o eliminarlos.
        Para declararlos el codigo es el siguiente:
        ```javascript
            var nombre;
        ```
        donde `var` es la palabra reservada para declarar una nueva variable, y `nombre` es la clave/identificador.

    * Strings
        Es el tipo de dato que se destina a guardar informacion tipo texto, se llama string porque es una cadena de caracteres.
        Para asignarle a una variable un String simplemente tengo que poner entre comillas `""` el texto que quiero asignar.
        Como en el siguiente ejemplo:
        ```javascript
            var texto = "My texto";
        ```

	* Funciones (argumentos, `return`)
        Son porciones de codigo o algoritmos que pueden admitir uno, mas de uno o incluso ningun dato de entrada, ejecuta una serie de lineas de codigo, y luego puede o no devolver un dato de salida.
        Los datos de entrados son llamados argumentos o parametros, y los de salida el retorno.
        Son muy utiles para organizar el codigo y mas si son codigos que se reutilizan.
        Se declaran de la siguiente forma:
        ```javascript
            //En este ejemplo la funcion no admite argumento y retorna "hola Mundo"
            function MyFuncion1(){
                return "Hola Mundo";
            }

            //En este admite un argumento deolviendo el mismo
            function MyFuncion2(argumento){
                return argumento;
            }

            //Aca se admite varios argumentos devolviendo la suma de estos
            function MyFuncion3(argumento1, argumento2){
                let ret = argumento1 + argumento2
                return ret;
            }

            //y en este ultimo la funcion no devuelve nada pero modifica una variable previamente modificada
            var retornoDeFuncion4
            function MyFuncion3(argumento1, argumento2){
                retornoDeFuncion4 = (argumento1 + argumento2);
            }
            //Este ultimo en el paradigma de programacion funcional no esta bien visto
        ```

	* Declaraciones `if`
        Las declaraciones `if` tambien llamados condicionales, son algoritmos que se ejecutan solo si se cumple una condicion y sino se cumpliera tambien podria ejecutar otro algoritmos.
        Son la forma de indicarle al codigo que "si se cumple tal condicion hace esto, sino esto otro".
        Para esto el codigo se debe escribir de la sigueinta manera:
        ```javascript
            let condicion = true;
            if (condicion) {
                console.log("la condicion es verdadera");
            } else {
                console.log("la condicion es falsa");
            }
        ```
        Donde lo que esta acontinuacion de la palabra reservada `if` y dentro de los `()` es la condicion que se debe cumplir para ejecutar el algoritmo que esta detro de las llaves `{}`, se puede agregar o no la palabra reservada `else` para agregar el algoritmo que se debe ejecutar si la condicion no se cumpliera.

	* Valores booleanos (`true`, `false`)
        Los valores booleanos son un tipo de dato para almacenar informacion de si y de no, mas alla de la posibilidad de poder almacenar este tipo de informacion, estos son los que se utilizan para guiar el fujo del codigo durante la ejecucion utilizandolos en condicionales o iteraciones a lo largo del mismo.
        Algunos ejemplos:
        ```javascript
            let condicion = true; // <-- booleano
            if (condicion) {
                console.log("la condicion es verdadera");
            }

            condicion = true; // <-- booleano
            i = 0;
            while (condicion) {
                i += 1;
                condicion = i < 255; //aca el comparador le va a asignar el vlaor de false cuando i alcance 255
            }
        ```