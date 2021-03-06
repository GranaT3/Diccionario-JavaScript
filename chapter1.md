# _**Funciones**_

Las funciones en `JavaScript` son un `objeto`, heredan sus propiedades de la clase padre `object.`Son bloques de código ejecutable, le podemos pasar parámetros y operar con ellos. Podemos modular nuestros programas y estructurar en bloque que realicen una tarea en concreto.

Las funciones al terminar su ejecución devuelven un valor que obtenemos con el parámetro `return`. Pueden llevar un nombre para ser invocadas más adelante o pueden no tener nombre y son llamadas`funciones anónimas`. Para evitar que el valor `undefined`  nos provoque errores y no poder controlarlo, podemos usar uno de los operadores `booleanos`.

`OR  -- ||` podemos usarlo para asignar un valor por default si no está definido.

`Let nombre = nombre || "Juan"`

_**Funciones Anidadas:**_ Pueden tener otras funciones dentro de ellas, ocasionando nuevos ámbitos para las `variables`definidas dentro de cada función. Para acceder a las funciones fuera de ellas tenemos que usar el operador doble paréntesis`()()`

_**Closures:**_  Los closures o funciones de cierre, son un patrón de diseño muy utilizado en `JavaScript`

Es una función que encapsula `variables` y definiciones`locales`, únicamente accesibles si son devueltas con el operador `return`, este patrón hace posible modularizar nuestro código.

**Generadores: **Es un objeto que sirve para decirle a`JavaScript`que nuestra función en un generador y se debe indicar con un asterisco de la siguiente forma:

```js
function* generador() { 
   yield 1;
   yield 2;
   yield 3;
}

var g = generador(); // "Generador { }"
```

Si creamos un generador debemos colocar la palabra clave`yield`la cual indica que cuando llamemos a la función después de la primera vez, esta iniciara en la linea después de`yield`. El generador convierte en objeto la función.

