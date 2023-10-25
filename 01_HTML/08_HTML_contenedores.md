# Contenedores

En HTML5 existen dos tipos de contenedores: los de bloque y los de línea.

## Contenedores de bloque

Estos contenedores ocupan todo el ancho disponible y se colocan uno debajo de otro.
Algunos elementos como los que hemos visto previamente son contenedores de bloque, por ejemplo:
- `<h1>` a `<h6>`
- `<p>`
- `<form>`
- `<ul>`
- `<ol>`
- `<li>`
- `<table>`
- `<header>`
- `<footer>`
- `<div>`

### `<div>`

La etiqueta `<div>` se utiliza para definir un contenedor de bloque genérico.

```html
<div> Esto es un contenedor de bloque. </div>
```

Debemos tener en cuenta que la etiqueta `<div>` no tiene ningún significado especial, simplemente se utiliza para agrupar elementos, tenemos mejores opciones para agrupar elementos de forma semántica, pero puede sernos útil en algunos casos.

## Contenedores de línea

Estos contenedores, al contrario que los de bloque no ocupan todo el ancho disponible y se colocan uno al lado del otro.

### `<span>`

La etiqueta `<span>` se utiliza para definir un contenedor de línea genérico.

```html
<span> Esto es un contenedor de línea. </span>
<span> Esto es otro contenedor de línea. </span>
```

Y aun más útil si le añadimos un identificador:

```html
<p> Mi nombre es <span id="nombre"> Juan </span> y tengo <span id="edad"> 20 </span> años. </p>
```

Ahora podemos acceder al contenido de cada contenedor de línea desde JavaScript:

```js
let nombre = document.getElementById("nombre").innerHTML;
let edad = document.getElementById("edad").innerHTML;
```

Tanto `<div>` como `<span>` son contenedores genéricos, nos ayudan a poder dividir el contenido de nuestra página en secciones, pero no tienen ningún significado especial, por lo que no son muy útiles para los buscadores.

Estudiaremos más adelante los conceptos de HTML semántico, estos contenedores ayudan a definir la estructura de nuestra página, pero no su significado.

