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