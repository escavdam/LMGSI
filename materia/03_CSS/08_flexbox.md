# Flexbox

Flexbox es un modelo de diseño que nos permite crear layouts flexibles. Es decir, layouts que se adaptan a diferentes tamaños de pantalla y dispositivos.

[MDN](https://developer.mozilla.org/es/docs/Web/CSS/CSS_Flexible_Box_Layout/Conceptos_Basicos_de_Flexbox)

[Guia / PDF tamaño poster](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)

## Contenedor flex

Para crear un contenedor flex, debemos usar la propiedad `display`:

```css
.contenedor {
  display: flex;
}
```

Una vez tenemos un contenedor flex, los elementos hijos del contenedor se convierten en elementos flex. Esto significa que podemos usar las propiedades de flexbox para modificar su comportamiento.

### flex-direction

La propiedad `flex-direction` nos permite modificar la dirección en la que se muestran los elementos flex. Por defecto, los elementos flex se muestran en fila:

```css
.contenedor {
  display: flex;
  flex-direction: row;
}
```

Podemos usar `flex-direction` para mostrar los elementos en columna:

```css
.contenedor {
  display: flex;
  flex-direction: column;
}
```

También podemos usar `flex-direction` para mostrar los elementos en fila, pero en orden inverso:

```css
.contenedor {
  display: flex;
  flex-direction: row-reverse;
}
```

O en columna, pero en orden inverso:

```css
.contenedor {
  display: flex;
  flex-direction: column-reverse;
}
```

Cuando tenemos `flex-direction` configurado como `row`, el eje principal es el horizontal, y el eje secundario es el vertical. Cuando tenemos `flex-direction` configurado como `column`, el eje principal es el vertical, y el eje secundario es el horizontal. Esto es importante tenerlo en cuenta a la hora de usar `justify-content` y `align-items`.

### flex-wrap

La propiedad `flex-wrap` nos permite modificar el comportamiento de los elementos flex cuando no caben en el contenedor. Por defecto, los elementos flex se muestran en una sola línea:

```css
.contenedor {
  display: flex;
  flex-wrap: nowrap;
}
```

Podemos usar `flex-wrap` para mostrar los elementos en varias líneas:

```css
.contenedor {
  display: flex;
  flex-wrap: wrap;
}
```

### flex-flow

La propiedad `flex-flow` nos permite modificar `flex-direction` y `flex-wrap` al mismo tiempo:

```css
.contenedor {
  display: flex;
  flex-flow: row wrap;
}
```

### justify-content

La propiedad `justify-content` nos permite modificar la alineación de los elementos flex en el `eje principal`. Por defecto, los elementos flex se muestran alineados a la izquierda, pero podemos usar los siguientes valores para modificarlo:

- `flex-start`: Los elementos se muestran alineados a la izquierda.
- `flex-end`: Los elementos se muestran alineados a la derecha.
- `center`: Los elementos se muestran centrados.
- `space-between`: Los elementos se muestran separados con el mismo espacio entre ellos.
- `space-around`: Los elementos se muestran separados con el mismo espacio alrededor de ellos.
- `space-evenly`: Los elementos se muestran separados con el mismo espacio entre ellos y alrededor de ellos.

### align-items

La propiedad `align-items` nos permite modificar la alineación de los elementos flex en el `eje secundario`. Por defecto, los elementos flex se muestran alineados arriba, pero podemos usar los siguientes valores para modificarlo:

- `flex-start`: Los elementos se muestran alineados arriba.
- `flex-end`: Los elementos se muestran alineados abajo.
- `center`: Los elementos se muestran centrados.
- `stretch`: Los elementos se muestran estirados para ocupar todo el espacio disponible.
- `baseline`: Los elementos se muestran alineados por su línea base.
- `first baseline`: Los elementos se muestran alineados por la línea base del primer elemento.
- `last baseline`: Los elementos se muestran alineados por la línea base del último elemento.
- `safe center`: Los elementos se muestran centrados, pero teniendo en cuenta el padding del contenedor.
- `unsafe center`: Los elementos se muestran centrados, sin tener en cuenta el padding del contenedor.

### flex-grow

La propiedad `flex-grow` nos permite modificar la proporción en la que los elementos flex crecen. Por defecto, todos los elementos flex tienen el mismo tamaño, pero podemos usar `flex-grow` para modificarlo:

```css
.elemento {
  flex-grow: 1;
}
```
