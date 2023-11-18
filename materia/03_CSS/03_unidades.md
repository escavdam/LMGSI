# Unidades de medida en CSS

[MDN Referencia](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Values_and_units)

CSS utiliza diferentes unidades de medida para especificar tamaños de elementos.

Estas unidades pueden ser relativas o absolutas.

## Unidades absolutas

Las unidades absolutas son unidades que no dependen de otras propiedades, estas son:

- `px`: Píxeles, es la unidad más común, un píxel es un punto en la pantalla.
- `cm`, `mm`, `pc` e `in`: Centímetros, milímetros, picas y pulgadas, son unidades de medidas físicas.
- `pt`: Puntos, es una unidad de medida física, un punto es una unidad de longitud que equivale a 1/72 de pulgada.
- `q`: Cuartos de milímetro, es una unidad de medida física, un cuarto de milímetro es una cuarta parte de un milímetro (0,248 mm).

### Pixel

Es la unidad más conocida por la gente cuando hablamos de pantallas, un píxel es un punto en la pantalla.

Sin embargo, la medida de un píxel no es fija en CSS y depende de la pantalla donde se muestre.

### cm, mm, in

Estas unidades de medida son unidades físicas, son unidades que se usan para medir distancias en el mundo real y nos son familiares.

Si la web que diseñamos se va a imprimir, estas unidades de medida son las más adecuadas.

### pt, pc, q

Los puntos y las picas son unidades de medida que se usan en la impresión, un punto equivale a 1/72 de pulgada y una pica equivale a 12 puntos.

La pica viene de la época en la que se usaban tipos móviles para imprimir, una pica era el tamaño de una letra `M` mayúscula, mientras que el punto era el tamaño de una letra `i` minúscula.

## Unidades relativas

Las unidades relativas son unidades que dependen de otras propiedades, estas son:

- `%`: Porcentaje, toma como referencia el marco o contexto actual, sus valores no tienen por qué ir de cero a cien, se pueden usar medidas mayores.
- `rem`: Toma como referencia el tamaño de la fuente del elemento raíz (normalmente el `html`).
- `vw`: Toma como referencia el ancho de la ventana.
- `vh`: Toma como referencia el alto de la ventana.
- `vmin`: Toma como referencia el tamaño de la ventana, pero usa el menor de los dos valores (ancho o alto).
- `vmax`: Toma como referencia el tamaño de la ventana, pero usa el mayor de los dos valores (ancho o alto).
- `em`: Toma como referencia el tamaño de la letra `M`.
- `ch`: Toma como referencia el tamaño de la letra `0` (cero).
- `ex`: Toma como referencia el tamaño de la letra `x` minúscula.
- `fr`: Toma como referencia el espacio disponible que queda en el contenedor.

### Unidades relativas a su contenedor

Si definimos un tamaño en el root, por ejemplo, en el `html`, entonces todas las unidades relativas se calcularán en base a ese tamaño.

```css
html {
  font-size: 16px;
}

p {
  font-size: 1em; /* 16px */
}

p span {
  font-size: 0.5em; /* 8px */
}
```
