# Bloques vs Inline

Todos los elementos CSS se pueden dividir en dos categorías: **bloques** e **inline**.

## Bloques

Los elementos de bloque siempre comienzan en una nueva línea y ocupan todo el ancho disponible.

Algunos elementos como los que hemos visto previamente son bloques, por ejemplo:
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

### Inline

Los elementos inline no comienzan en una nueva línea y solo ocupan el ancho que necesitan.

Algunos elementos como los que hemos visto previamente son inline, por ejemplo:

- `<a>`
- `<span>`
- `<img>`
- `<input>`
- `<button>`
- `<label>`
- `<textarea>`
- `<select>`
- `<option>`

## Bloques vs Inline

Los elementos de bloque y los elementos inline se comportan de forma diferente en algunas situaciones.

### Ancho

Los elementos de bloque ocupan todo el ancho disponible, mientras que los elementos inline solo ocupan el ancho que necesitan.

Por ejemplo, si tenemos un elemento `<a>` con un texto muy largo, este se dividirá en varias líneas:

```html
<a href="#"> Lorem ipsum dolor sit amet, consectetur adipiscing elit. </a>
```

Sin embargo, si lo convertimos en un bloque, ocupará todo el ancho disponible:

```css
a {
    display: block;
}
```

De la misma manera, un elemento `<span>` no ocupará todo el ancho disponible, ayudándonos a "dividir" elementos dentro de un bloque:

```html
<p> El planeta <span> Marte </span> es el cuarto planeta del sistema solar. </p>
```

