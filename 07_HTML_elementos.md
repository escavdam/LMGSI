# Elementos HTML
HTML posee 142 tags o etiquetas, cada una con su función específica. Algunos renderizan elementos en la pantalla, otros como elementos vacíos.

[Lista de etiquetas HTML](https://developer.mozilla.org/es/docs/Web/HTML/Elemento)

>**Recuerda** que puedes utilizar la consola para analizar cualquier web y ver que tags y elementos utilizan para crear su estructura. 

## Indice
- 1.0 [Etiquetas de texto](#etiquetas-de-texto)  
  - 1.1 Cabeceras `<h1> - <h6>`
  - 1.2 Párrafos `<p>`
  - 1.3 Saltos de línea `<br>`
  - 1.4 Líneas horizontales `<hr>`
  - 1.5 Negrita `<b>`
  - 1.6 Cursiva `<i>`
  - 1.7 Subrayado `<u>`
  - 1.8 Texto importante `<strong>`
  - 1.9 Texto enfatizado `<em>`
  - 1.10 Texto pequeño `<small>`
  - 1.11 Texto marcado `<mark>`
  - 1.12 Texto eliminado `<del>`
  - 1.13 Texto insertado `<ins>`
  - 1.14 Texto subíndice `<sub>`
  - 1.15 Texto superíndice `<sup>`
  - 1.16 Cita `<q>`
  - 1.17 Cita larga `<blockquote>`
  - 1.18 Abreviatura `<abbr>`
  - 1.19 Código `<code>`
  - 1.20 Teclas `<kbd>`
- 2.0 [Etiquetas de enlaces](#etiquetas-de-enlaces)
  - 2.1 Enlace `<a>`
  - 2.2 Enlace con `target="_blank"`
  - 2.3 Enlace con `download`
  - 2.4 Enlace con `rel="noopener"`
- 3.0 [Etiquetas de imágenes](#etiquetas-de-imágenes)
  - 3.1 Imagen `<img>`
  - 3.2 Imagen con `alt`
  - 3.3 Imagen con `width` y `height`
- 4.0 [Etiquetas de listas](#etiquetas-de-listas)
  - 4.1 Lista desordenada `<ul>`
  - 4.2 Lista ordenada `<ol>`
  - 4.3 Elemento de lista `<li>`
## Etiquetas de texto
### `<h1> - <h6>`
Las etiquetas `<h1>` a `<h6>` se utilizan para definir los títulos de una página web. `<h1>` es el título principal, `<h2>` es un subtítulo, `<h3>` es un subtítulo de `<h2>`, etc.

```html
<h1> Cabecera de nivel 1 </h1>
<h2> Cabecera de nivel 2 </h2>
<h3> Cabecera de nivel 3 </h3>
```

### `<p>`
La etiqueta `<p>` se utiliza para definir un párrafo.

```html
<p> Esto es un párrafo. </p>
```

### `<br>`
La etiqueta `<br>` se utiliza para insertar un salto de línea.

```html
<p> Esto es un párrafo. <br> Esto es otro párrafo. </p>
```

### `<hr>`
La etiqueta `<hr>` se utiliza para insertar una línea horizontal.

```html
<p> Esto es un párrafo. </p>
<hr>
<p> Esto es otro párrafo. </p>
```

### `<b>`
La etiqueta `<b>` se utiliza para definir un texto en negrita.

```html
<p> Esto es un texto <b> en negrita </b>. </p>
```

### `<i>`
La etiqueta `<i>` se utiliza para definir un texto en cursiva.

```html
<p> Esto es un texto <i> en cursiva </i>. </p>
```

### `<u>`
La etiqueta `<u>` se utiliza para definir un texto subrayado.

```html
<p> Esto es un texto <u> subrayado </u>. </p>
```

### `<strong>`
La etiqueta `<strong>` se utiliza para definir un texto importante.

```html
<p> Esto es un texto <strong> importante </strong>. </p>
```

### `<em>`
La etiqueta `<em>` se utiliza para definir un texto enfatizado.

```html
<p> Esto es un texto <em> enfatizado </em>. </p>
```

### `<small>`
La etiqueta `<small>` se utiliza para definir un texto pequeño.

```html
<p> Esto es un texto <small> pequeño </small>. </p>
```

### `<mark>`
La etiqueta `<mark>` se utiliza para definir un texto marcado.

```html
<p> Esto es un texto <mark> marcado </mark>. </p>
```

### `<del>`
La etiqueta `<del>` se utiliza para definir un texto eliminado.

```html
<p> Esto es un texto <del> eliminado </del>. </p>
```

### `<ins>`
La etiqueta `<ins>` se utiliza para definir un texto insertado.

```html
<p> Esto es un texto <ins> insertado </ins>. </p>
```

### `<sub>`
La etiqueta `<sub>` se utiliza para definir un texto subíndice.

```html
<p> Esto es un texto <sub> subíndice </sub>. </p>
```

### `<sup>`
La etiqueta `<sup>` se utiliza para definir un texto superíndice.

```html
<p> Esto es un texto <sup> superíndice </sup>. </p>
```

### `<q>`
La etiqueta `<q>` se utiliza para definir una cita.

```html
<p> Esto es un texto con una <q> cita </q>. </p>
```

### `<blockquote>`
La etiqueta `<blockquote>` se utiliza para definir una cita larga.

```html
<blockquote> Esto es un texto con una cita larga. </blockquote>
```

### `<abbr>`
La etiqueta `<abbr>` se utiliza para definir una abreviatura.

```html
<p> Esto es un texto con una <abbr> abreviatura </abbr>. </p>
```

### `<code>`
La etiqueta `<code>` se utiliza para definir un texto con código.

```html
<p> Esto es un texto con <code> código </code>. </p>
```

### `<kbd>`
La etiqueta `<kbd>` se utiliza para definir un texto con teclas.

```html
<p> Esto es un texto con <kbd> teclas </kbd>. </p>
```

## Etiquetas de enlaces
### `<a>`
La etiqueta `<a>` se utiliza para definir un enlace.

```html
<a href="https://www.google.com"> Google </a>
```

### `<a>` con `target="_blank"`
La etiqueta `<a>` con el atributo `target="_blank"` se utiliza para definir un enlace que se abre en una nueva pestaña.

```html
<a href="https://www.google.com" target="_blank"> Google </a>
```

### `<a>` con `download`
La etiqueta `<a>` con el atributo `download` se utiliza para definir un enlace de descarga.

```html
<a href="https://www.google.com" download> Google </a>
```

### `<a>` con `rel="noopener"`
La etiqueta `<a>` con el atributo `rel="noopener"` se utiliza para definir un enlace que no permite acceder a la ventana del navegador.

```html
<a href="https://www.google.com" rel="noopener"> Google </a>
```

## Etiquetas de imágenes
### `<img>`
La etiqueta `<img>` se utiliza para definir una imagen.

```html
<img src="imagen.jpg">
```

### `<img>` con `alt`
La etiqueta `<img>` con el atributo `alt` se utiliza para definir una imagen con un texto alternativo.

```html
<img src="imagen.jpg" alt="Texto alternativo">
```

### `<img>` con `width` y `height`
La etiqueta `<img>` con los atributos `width` y `height` se utiliza para definir una imagen con un ancho y un alto.

```html
<img src="imagen.jpg" width="100" height="100">
```

## Etiquetas de listas
### `<ul>`
La etiqueta `<ul>` se utiliza para definir una lista desordenada.

```html
<ul>
    <li> Elemento 1 </li>
    <li> Elemento 2 </li>
    <li> Elemento 3 </li>
</ul>
```

### `<ol>`
La etiqueta `<ol>` se utiliza para definir una lista ordenada.

```html
<ol>
    <li> Elemento 1 </li>
    <li> Elemento 2 </li>
    <li> Elemento 3 </li>
</ol>
```

### `<li>`
La etiqueta `<li>` se utiliza para definir un elemento de una lista.

```html
<ul>
    <li> Elemento 1 </li>
    <li> Elemento 2 </li>
    <li> Elemento 3 </li>
</ul>
```

