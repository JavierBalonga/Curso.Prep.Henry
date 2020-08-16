1.

* `for`:

    La palabra reservada `for` esta destinada a declarar un bucle o loop asi llamado for, como el siguiente:
    ```javascript
    for (let i = 0; i < 255; i++) {
        console.log(i);
    }
    ```
    Donde el primer argumento que admite `let i = 0` inicializa una variable `i` que es la que va a guiar por asi decir la ejecucion del bucle.
    El segundo argumento `i < 255` es la condicion que se va a revisar en cada iteracion, si la misma da `true` el bucle continueara iterando de lo contrario detiene las iteraciones.
    El tercer argumento `i++` es el incremento de la variable inicializada que se va a ejecutar en cada iteracion.
    Y asi como en los condicionales lo que esta entre las llaves `{}` es el algoritmo que se ejecuta en cada iteracion.


* `&&`, `||`, `!`

    Los operadores lógicos and `&&`, or `||`, not `!` son operadores que se utilizan para trabajar con las condiciones, como por ejemplo si se quisiera ejecutar algo solo si se cumplen dos o mas condiciones, o si se cumpliera alguna de varias condiciones, o si no se cupliera alguna condicion.
    Unos ejemplos:
    ```javascript
    let condicion1 = true && true // true
    let condicion2 = true && false // false
    let condicion3 = false && true // false
    let condicion4 = false && false // false

    let condicion5 = true || true // true
    let condicion6 = true || false // true
    let condicion7 = false || true // true
    let condicion8 = false || false // false

    let condicion9 = !true // false
    let condicion9 = !false // true
    ```
