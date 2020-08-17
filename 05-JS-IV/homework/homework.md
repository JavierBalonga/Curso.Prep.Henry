1. 

* Objetos:

    Yo describo al Objeto, como representaciones de conceptos realizadas por el desarrollador.


* Propiedades:

    Las propiedades de los objetos, son caracteristicas de los mismos, que se almacenan como variables.


* Métodos:

    Los metodos de los objetos, son funciones contenidas dentro de los mismos, seria el equivalente a las acciones que pueden realizar estos conceptos.


    Un ejemplo de todo esto podria ser el concepto de lo que es un gato:
    Se podria decir los gatos tienen un nombre, una edad, 4 patas, pelo, vigotes, y cuando lo acaricias dicen 'meow! n_n':
    Entonces bajo esa definicion de las caracteristicas de un gato yo podria definirlo en el codigo de la siguiente manera:
    ```javascript
    var gato = {
        nombre: "nacho",
        edad: 5,
        patas: 4,
        pelo: true,
        vigotes: true,
        acariciar: function() {
            console.log('meow! n_n');
        }
    };
    ```
    Asi como esta declarado el gato tiene las siguientes propiedades:
    * nombre
    * edad
    * patas
    * pelo
    * vigotes
    Y los el metodo de acariciarlo:
    ```javascript
    > gato.acariciar();
    < 'meow! n_n'
    ```


* Bucle `for…in`:

    Cuando se quiere recorrer todos los elementos del objeto ya sean propiedades o metodos se puede usar el loop `for…in` para acceder uno por uno a todos ellos, ya sea para modificarlos o acceder simplemente a ellos:
    ```javascript
    var objeto = {
        ElementoA: 'Hola',
        ElementoB: ' ',
        ElementoC: 'Mundo',
        ElementoD: '!'
    };

    for (let clave in objeto){
        console.log(objeto[clave]);
    }
    //hola
    // 
    //Mundo
    //!
    ```


* Notación de puntos vs notación de corchetes

    La notacion de puntos y la notacion de corchetes hacen distintas cosas, pero la mejor forma de explicarlo es con ejemplos:
    ```javascript
    var objeto = {
        propiedad: 'Soy una propiedad',
        YoTambienSoyUnaPropiedad: 'ajam tambien lo soy'
    }
    //Los siguientes llamados son identicos pero con distinta notacion
    //Notacion de puntos:
    Console.log(objeto.propiedad); 
    //'Soy una propiedad'

    //Notacion de corchetes:
    Console.log(objeto.["propiedad"]);
    //'Soy una propiedad'


    //La notacion de corchetes puedo hacer lo sigiente, que es muy util
    //Notacion de corchetes:
    let propiedad = "YoTambienSoyUnaPropiedad";
    Console.log(objeto.[propiedad]);
    //'ajam tambien lo soy'

    //Lo que seria pasar una variable previamente definida entre los corchetes


    //Sinembargo esto seria un error
    //Notacion de corchetes:
    Console.log(objeto.[YoTambienSoyUnaPropiedad]); 
    //Error

    //Porque en este caso YoTambienSoyUnaPropiedad es una variable que no se declaro
    ```