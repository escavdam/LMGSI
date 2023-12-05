# Medidas del navegador

Nuestro navegador nos proporciona información sobre el tamaño de la ventana del navegador, el tamaño del documento, y el tamaño de la pantalla que estamos usando.

Podemos acceder a esta información desde JavaScript.

[Ejemplo interactivo](https://puredata.neocities.org/ejemplos/navegador_size/)

## Tamaño de pantalla

El tamaño de pantalla es el tamaño de la pantalla física que estamos usando. Nuestro monitor.

Para obtener el tamaño de pantalla, podemos usar las propiedades `screen.width` y `screen.height`:

```js
console.log(screen.width);
console.log(screen.height);
```

## Tamaño de ventana

El tamaño de ventana es el tamaño del marco exterior del navegador.

Para obtener el tamaño de ventana, podemos usar las propiedades `outerWidth` e `outerHeight`:

```js
console.log(window.outerWidth);
console.log(window.outerHeight);
```

## Tamaño de documento + scroll

El tamaño de documento es el tamaño del documento HTML que estamos mostrando en el navegador, incluyendo, si lo hay, el scroll.

Para obtener el tamaño de documento, podemos usar las propiedades `innerWidth` e `innerHeight`:

```js
console.log(window.innerWidth);
console.log(window.innerHeight);
```

## Tamaño de documento

El tamaño de documento es el tamaño del documento HTML que estamos mostrando en el navegador, sin incluir el scroll lateral o inferior, ni la barra de herramientas del navegador.

Para obtener el tamaño de documento, podemos usar las propiedades `document.documentElement.clientWidth` y `document.documentElement.clientHeight`:

```js
console.log(document.documentElement.clientWidth);
console.log(document.documentElement.clientHeight);
```
