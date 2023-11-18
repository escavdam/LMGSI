# Texto

Podemos editar el texto de un elemento con muchas propiedades, vamos a ver las mas importantes.

## color

La propiedad `color` nos permite cambiar el color del texto.

```css
p {
  color: red;
}
```

## background

La propiedad `background` nos permite cambiar el color de fondo de un elemento.

```css
p {
  background: red;
}
```

## font-size

La propiedad `font-size` nos permite cambiar el tamaño de la fuente.

```css
p {
  font-size: 20px;
}

h1 {
  font-size: 10em;
}
```

## font-family

La propiedad `font-family` nos permite cambiar la fuente.

```css
p {
  /* font-family: "Times New Roman", Times, serif; */
    font-family: Arial, Helvetica, sans-serif;
}
```

CSS incluye las siguientes fuentes por defecto, algunas de las mas comunes son:

- `serif`: Fuentes con remates, como Times New Roman.
- `sans-serif`: Fuentes sin remates, como Arial.
- `monospace`: Fuentes de ancho fijo, como Courier.
- `cursive`: Fuentes con aspecto de escritura a mano, como Comic Sans.
- `fantasy`: Fuentes decorativas, como Impact.
- `system-ui`: Fuentes del sistema operativo.
- `ui-serif`: Fuentes con remates del sistema operativo.
- `ui-sans-serif`: Fuentes sin remates del sistema operativo.
- `ui-monospace`: Fuentes de ancho fijo del sistema operativo.
- `ui-rounded`: Fuentes redondeadas del sistema operativo.

## text-align

La propiedad `text-align` nos permite alinear el texto horizontalmente.

```css
p {
  text-align: center;
}
```

Podemos usar los valores `left`, `right`, `center` o `justify`.

## line-height

La propiedad `line-height` nos permite cambiar la altura de una línea de texto.

```css
p {
  line-height: 1.5;
}
```

## letter-spacing

La propiedad `letter-spacing` nos permite cambiar el espacio entre letras.

```css
p {
  letter-spacing: 1px;
}
```

## word-spacing

La propiedad `word-spacing` nos permite cambiar el espacio entre palabras.

```css
p {
  word-spacing: 1px;
}
```

## text-decoration

La propiedad `text-decoration` nos permite añadir decoraciones al texto.

```css
p {
  text-decoration: underline;
}
```

Podemos usar los valores `underline`, `overline`, `line-through` o `none`.

## text-transform

La propiedad `text-transform` nos permite cambiar el texto a mayúsculas o minúsculas.

```css
p {
  text-transform: uppercase;
}
```

Podemos usar los valores `uppercase`, `lowercase` o `capitalize`, ten en cuenta que esto solo afecta a la apariencia del texto, no a su contenido html.

## text-shadow

La propiedad `text-shadow` nos permite añadir sombras al texto.

```css
p {
  text-shadow: 1px 1px 1px black;
}
```

El primer valor es el desplazamiento horizontal, el segundo el desplazamiento vertical, el tercero el desenfoque y el cuarto el color.

## white-space

La propiedad `white-space` nos permite cambiar el comportamiento de los espacios en blanco.

```css
p {
  white-space: nowrap;
}
```

Podemos usar los valores `normal`, `nowrap` o `pre`, si usamos `pre` los saltos de línea se respetarán, y si usamos `nowrap` el texto no se partirá en varias líneas, `normal` es el valor por defecto.


