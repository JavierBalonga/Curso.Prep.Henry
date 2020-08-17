1. 

* Arrays:

    Los `array` son arreglos o listas de elementos, estos pueden ser leidos, modificados, eliminados, o incluso agregados.
    La forma de acceder a esos elementos es con indices:
    ```javascript
    var array = ['Elemento1', 'Elemento2', 'Elemento3', 'Elemento4'];
    array; // llama el array entero

    var indice = 0;
    array[indice]; // 'Elemento1'

    array[3]; // 'Elemento4'
    ```
    Se pueden usar los metodos:
    `.push` para agregar un elemento al final:
    ```javascript
    array.push('Elemento5');
    // ['Elemento1', 'Elemento2', 'Elemento3', 'Elemento4', 'Elemento5']
    ```
    `.pop` para eliminar el ultimo elemento:
    ```javascript
    array.pop();
    // ['Elemento1', 'Elemento2', 'Elemento3', 'Elemento4']
    array.pop();
    // ['Elemento1', 'Elemento2', 'Elemento3']
    ```
    `.unshift` para agregar un elemento al principio :
    ```javascript
    array.unshift('Elemento0');
    // ['Elemento0', 'Elemento1', 'Elemento2', 'Elemento3']
    ```
    `.shift` para eliminar el primer elemento:
    ```javascript
    array.shift();
    // ['Elemento1', 'Elemento2', 'Elemento3']
    array.shift();
    // ['Elemento2', 'Elemento3']
    ```

