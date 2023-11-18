# Propiedades

[MDN Referencia](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference)

Las propiedades son los estilos que queremos aplicar a los elementos seleccionados.

Las propiedades se escriben en minúsculas y si tienen más de una palabra, se separan con un guión `-`.

```css
h1 {
  color: red;
  font-size: 20px;
}
```

Vamos a ver algunas de las propiedades más usadas:

## color

La propiedad `color` nos permite cambiar el color del texto.

Podemos utilizar colores por nombre, por ejemplo `red` o `blue`, valores hexadecimales como `#FF00FF` o valores RGBA mediante la funcion `rgba(r, g, b, a)`.

```css
h1 {
  color: red;
}

p {
  color: #0000ff;
}
    
a {
  color: rgba(0, 0, 255, 0.5);
}
```

## background

La propiedad `background` nos permite cambiar el color de fondo de un elemento.

Podemos usar los mismos tipos de colores que con la propiedad `color`.

```css
h1 {
  background: red;
}

body{
    background: #000000;
    color: #FFFFFF;
}
```

## font-size

La propiedad `font-size` nos permite cambiar el tamaño de la fuente.

Podemos usar valores en píxeles `px`, puntos `pt`, porcentajes `%`, etc.

```css
h1 {
  font-size: 20px;
}
```

## font-family

La propiedad `font-family` nos permite cambiar la fuente.

```css
h1 {
  font-family: "Comic Sans MS";
}
```

## text-align

La propiedad `text-align` nos permite alinear el texto.
Podemos usar los valores `left`, `right`, `center` o `justify`.

```css
h1 {
  text-align: center;
}
```

## width

La propiedad `width` nos permite cambiar el ancho de un elemento.

```css
div {
  width: 100px;
}
```

Tenemos otras propiedades relacionadas con el ancho, como `max-width` o `min-width`.

## height

La propiedad `height` nos permite cambiar el alto de un elemento.

```css
div {
  height: 100px;
}
```

Tenemos otras propiedades relacionadas con el alto, como `max-height` o `min-height`.

## margin

La propiedad `margin` nos permite cambiar el margen de un elemento.

```css
p {
  margin: 100px;
}
```

El margen es el espacio que hay entre el elemento y los elementos de alrededor.

## padding

La propiedad `padding` nos permite cambiar el relleno de un elemento.

```css
p {
  padding: 100px;
}
```

El relleno es el espacio que hay entre el contenido del elemento y el borde.

## border

La propiedad `border` nos permite cambiar el borde de un elemento.

```css
p {
  border: 1px solid black;
}
```

El borde es la linea que separa el contenido del elemento y el padding del margen.

## Interacción entre padding, border y margin:

Las propiedades `padding`, `border` y `margin` son propiedades que interactúan entre ellas en un mismo elemento.

Puede ser muy útil inspeccionar un elemento para entender las propiedades que tiene, considera el siguiente `html`:

```html
  <p>Hola mundo</p>
  <p>Este párrafo contiene una línea</p>
  <p>Otro parrafo con mas información</p>
```

Y el siguiente `css` asociado:

```css
p {
  border: 1px solid black;
  padding: 10px;
  margin: 20px;
}
```

![padding, border y margin](./img/padding_border_margin.png)
