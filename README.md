# Arrays

- Una array es una zona de almacenamiento continuo, conde se pueden introducir varios valores cada uno de ellos ubicado por la posición que ocupa en el array.

- Tambien son denominados arreglos o vectores, y cuando son de 2 dimensiones son llamados matrices.

- Los arrays no brindan la capacidad de almacenar una coleccion de elementos y acceder a ellos de manera individual.

- Cada elemento se identifica mediante su posición en el array, denominada **indice** y estos indices son siempre secuenciales.

- En Javascript son altamente frexibles en terminos de los difeentes tipos e datos que podemos almacenar en cada posición de la array.

## Crear Un Array 

1. Declarando una array con elementos en linea 

```Javascript
let miArray = [1, 2, 3];
consele.log(miArray);
```

2. Declarando un array con la sintaxis **new Array()**

```Javascript
let miArray = new Array(1, 2, 3);
consele.log(miArray);
```

3. Declarando un array con un tamaño especifico utilizando la sintaxis **new Array** y asignando valores despues:

```Javascript
let miArray = new Array(3);
miArray [0] = 1;
miArray [1] = 2;
miArray [2] = 3;
console.log(miArray);
```

4. Declarando un array con elementos de diferentes tipos de datos

```Javascript
let miArray4 = [1, "dos", true, {nombre: "Juan", edad: 30}];
console.log(miArray4);
```

## Accediendo a la información de un array

### Propiedad length
- Devuelve la cantidad de elementos del array

### Operador [pos]
- Permite acceder para leer o modificar el elemento post del array

### Método at(pos)
- Devuelve el elemento de la posición pos. El parametro admite valores negativos , lo que significa que empiezan a contar por el final del array.

```Javascript
const letters = ["A", "B", "C"];
console.log(letters.length);
console.log(letters[2]);
console.log(letters[5]);
```

## Añadir o eliminar elementos 
- push (ele1, ele2): añade uno o varios elementos al final del array. Devuelve el tamaño del array.

```Javascript
let miArray = [1, 2, 3];
miArray.push(4); // Agg el elemento 4 al final del array 
console.log(miArray);
```
- pop(): Devuelve el ultimo elemento del array y lo elimina 

```Javascript
let miArray = [1, 2, 3];
miArray.pop(); // Elimina el ultimo elemento del array
console.log(miArray);
```

- unshift(ele1, ele2): ñade uno o varios elementos al inicio devolviendo el tamaño del array despues de añadidos

```Javascript
let miArray = [1, 2, 3];
miArray.unshift(0); // Agg el elemento 0 al inicio del array 
console.log(miArray);
```

- shift(): Devuelve el primer elemento del array y lo elimina 

```Javascript
let miArray = [1, 2, 3];
miArray.shift(0); // Elimina el primer elemento del array  
console.log(miArray);
```

- Concat(ele1, ele2): concatena dos arrays

```Javascript
let miArray = [1, 2, 3];
let miOtroArray = [4, 5];
let nuevoArray = miArray.concat(miOtroArray)
console.log(miArray);
console.log(miOtroArray);
console.log(nuevoArray)
```

-split(separador): a partir de una cadena, crea un array dividiendo dicha cadena en elementos delimitados por separador.

```Javascript
let miString = "Hola, ¿cómo estas?";
let miArray = miString.split(" ");
console.log(miArray);
```

- join(separdor): a partir de un array, crea una cadena separando cada elemento con el separador.

```Javascript
let miString = "Hola, ¿cómo estas?";
let miString = miArray.join(" "); 
console.log(miString);
```

## Búsqueda de elementos en un array

- includes(elemento): devuelve true o false si el elemento existe o no dentro del array

- Indexof(elemento): devuelve la posición de la primera aparición del elemento. Si no existe, devuelve -1.

- LastIndexOf(elemento): devuelve la posición de la ultima aparición del elemento. Si no existe, devuelve -1.

## Modificar el array o crear fragmentos 

- slice(inicio, fin): devuelve un array con los elementos desde la posición inicio hasta la posición fin, ambos excluidos.

## Ordenar elementos de un array 

- reverse(): invierte el orden d los elementos del array.

- sort(): ordena el array alfabeticamente 

-sort(criterio): ordena el array con e criterio determinado por la función criterio.

## Borrar elementos de un array

- Se puede borrar el contenido de un elemento de un array poniendo su valor a null o asignando una cadena vacia " ".

- Para elminar completamente un elemento del array se utiliza el operador delete.

## Recorrido de un array

1. Recorrer con un bucle clásico, pasando por todos los elementos.

```Javascript
var dias = ["lunes", "martes", "miercoles", "jueves", "viernes", "sabado", "domingo"];
for (i=0; i<dias.length;i++)
{
    console.log(dias[i]);
}
```

2. Recorrer con while, pasando por todos los elementos

```Javascript
var dias = ["lunes", "martes", "miercoles", "jueves", "viernes", "sabado", "domingo"];
var i =0;
while(i=0; i<dias.length)
{
    console.log(dias[i]);
}
```

3. Usando la sentencia for..in.

```Javascript
var dias = ["lunes", "martes", "miercoles", "jueves", "viernes", "sabado", "domingo"];
for(let index in dias)
{
    console.log(dias[index]);
}
```

## Arrays multidimensionales 

```Javascript
const matrix = [
    [1,2,3],
    [4,5,6],
    [7,8,9]
];
```

- Recorrer una matriz utilizando bucles anidados 

```Javascript
var dias = ["lunes", "martes", "miercoles", "jueves", "viernes", "sabado", "domingo"];
for (let i=0; i<matriz.length;i++)
{
    for(let j=0;matriz[i]. length; j++)
    {
        console.log(dias[i][j]);
    }
}
```

# Ejercicios

1. Dada una lista de números separados por coma, calcular la suma, el mayor, el menor y la media de todos.

2. Introducir dos cadenas con elementos seperados por coma, y con un botón concatenar las dos cadenas y mostrarlas en pantalla.

3. Introducir uno a uno los elementos en un array a través de un boton. Con otro botón se va eliminado el último elemento. Siempre que se pulse alguno de los botones de debe mostrar el contenido del array.

4. Introducir un conjunto de números separados por comas. Cuando se pulsa el botón "Pares" cargar una tabla con los números introducidos y luego crear otra que solo incluya los números pares y mostrarla.

