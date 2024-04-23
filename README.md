# arrays_js

- Un array es una zona de almacenamiento contunuo, donde se introducir varios valores , cada uno de ells ubicados por la posicion que ocupa en el array. 
- Tambien son denminados arreglos o vectores, y cuando son de dimensiones son llamados matrices.
- Los arrays nos brindan la capacidad de almacenar una coleccion de elementos y accedera ellos de manera individual.
- Cada elemento se identifica mediante su posicion en el array, denominada **indice**, y estos indices son siempre secuenciales.
- En Javascript son altamente flexibles en terminos de los diferentes tipos de datos que podemos almacenar en cada posicion del array.

## Crear un Array

1. Declarando un array con elemntos en linea 

```Javascript
let miArray = [1,2,3];
console.log(miArray);
```

2. Declarando un array con la sintaxis **new Array()**

```javascript
let miArray = new Array(1,2,3);
console.log(miArray);
```
3. Declarando un array con un tamaño especifico utilizando la sintaxis **new Array** y asignando valores despues:


```javascript
let miArray = new Array(3);
miArray[0] = 1;
miArray[1] = 2;
miArray[2] = 3;
console.log(miArray);
```
4. Declarando un array con elemntos de diferentes tipos de datos.

```javascript
let miArray4 = [1, "dos", true, {nombre: 'juan', edad: 30}];
console.log(miArray4);
```