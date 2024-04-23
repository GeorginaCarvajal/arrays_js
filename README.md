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

## Accediendo a la informacion de un array

### Propiedad length
- Devuelve la cantidad de elementos de un array

### Operador  [Pos]
- Permite acceder para leer o modificar el elemto pos del array

### Metodo at (pos)
- Devuelve el elemento de la posicion pos. el parametro admite valores negativos, lo que significa que empieza a contar por el final del array.

```Javascript
const letters = ["A", "B", "C"];
console.log(letters.length);
console.log(letters[2]);
console.log(letters[5]);
```

## Añadir o eliminar elementos
- Push (ele1, ele2): añade uno ovarios elementos al final del array, Devuelve el tamaño del array.

```Javascript
let miArray = [1, 2, 3];
miArray.push(4); // Agrega el elemento 4 al final del array
console.log(miArray);
```
- op(): devuelve el ultimo elemento del array y lo elimina
```Javascript
let miArray = [1, 2, 3];
miArray.push(); // elimina el ultimo elemento del array
console.log(miArray);
```

- unshift(ele1, ele2): agrega uno a varios elementos al inicio, devolviendo el tamaño del array despues de añadidos
```Javascript
let miArray = [1, 2, 3];
miArray.unshift(0); // agrega el elemento o al inicio del array
console.log(miArray);
```
- shift(): devuelve el primer elemento del array y lo elimina
```Javascript
let miArray = [1, 2, 3];
miArray.shift(0); // elimina el primer elemento del array
console.log(miArray);
```

- concat(ele1, ele2,): concatena dos arrays
```Javascript
let miArray = [1, 2, 3];
let miOtroArray = [4,5];
let minuevoArray = MiArray.concat(miOtroArray);
console.log(miArray);
console.log(miOtroArray);
console.log(minuevoArray);
```

- split(separador): a partir de una cadena, crea un array dividiendo dicha cadena en elementos delimitados por separador
```Javascript
let miString = "Hola, ¿Como estas?";
let miArray = miString.split("");
console.log(miArray);
```

- join(separador): a partir de un array, crea una cadena separando cada elemento con el separador.
```Javascript
let miArray = ["Hola,", "¿Como", "estas?"];
let miString = miArray.join(" ");
console.log(miString);
```

## Busqueda de elementos en un array
- includes(elemento): devuelve true o false  si el elemento existe o no dentro del array
- indexOf(elemento): devuelve la posicion de la primera aparicion del elemento. Si no existe, devuelve -1.
-  lastIndexOf(elemento): devuelve la posicion de la ultima aparicion del elemento. Si no existe, devuelve -1.

## Modificar el array o crear fragmentos
- slice(inicio, fin): devuelveun array con los elementos desde la posicion iniciohasta la posicion fin, ambos excluidos.

##Ordenar elementos de un array
- reverse(): invierte el orden de los elementos del array
- sort(): orfdena el array alfabeticamente.
-sort(criterio): ordena el array con el criterio determinado por la funcion criterio.

## Borrar elementos de un array
- Se puede borrar el contenido de un elemento de un array poniendo su valor a null o asignado una cadena vacia " ".
- Para eliminar completamente un elemnto del array se utiliza el operador delete.

## Recorrido de un Array
1. Recorrer un bucle clasico, pasando por todos los elementos.
```Javascript
var dias = ["lunes", "Martes", "Miercoles", "Jueves", "Viernes", "Sabado", "Domingo"];
for (i=0;i<dias.length;i++)
{
    console.log(dias[i]);
}
```

2. Recorrer con un while, pasando por todos los elemetos
```Javascript
var dias = ["lunes", "Martes", "Miercoles", "Jueves", "Viernes", "Sabado", "Domingo"];
for (i=0;i<dias.length;i++)
{
    console.log(dias[i]);
}
```
3. Usando la sentencia for... in.
```Javascript
var dias = ["lunes", "Martes", "Miercoles", "Jueves", "Viernes", "Sabado", "Domingo"];
for (let index in dias)
{
    console.log(dias[index]);
}
```
## Arrays multidimensionales
```Javascript
const matrix  = [
    [1,2,3],
    [4,5,6],
    [7,8,9]
];
```
Recorrer una matriz utilizando bucles anidados
```Javascript
var dias = ["lunes", "Martes", "Miercoles", "Jueves", "Viernes", "Sabado", "Domingo"];
for (let i=0;i<matrix.length;i++)
{
    for (let j=0;matrix[i].length; j++)
    {
    console.log(matrix[i][j]);
    }
}
```
# Ejercicios

1. Dada una lista de numeros separados por coma, calcular la suma, el mayor, el menor y la media de todos.

2. Introducir dos cadenas con elementos separads por coma, y con un boton concatenar las dos cadenas y mostrarlas en pantalla.

3. Introducir uno a uno los elementos en un array a través de un boton. Con otro botón se va eliminado el último elemento. Siempre que se pulse alguno de los botones de debe mostrar el contenido del array.

4. Introducir un conjunto de números separados por comas. Cuando se pulsa el botón "Pares" cargar una tabla con los números introducidos y luego crear otra que solo incluya los números pares y mostrarla.