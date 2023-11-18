# Imagenes

Al insertar imágenes, por defecto, estas se muestran a su tamaño original. Para poder adaptar el tamaño a diferentes dispositivos, podemos usar la propiedad `width` y `height` junto a `object-fit`.

En general, lo que buscamos al adaptar imágenes es que el ancho de la imagen se adapte al ancho del contenedor, y que la altura se adapte proporcionalmente. Para ello, podemos usar una regla como la siguiente:

```css
img {
  width: 100%;
  height: auto;
}
```

Sin embargo, si el contenedor no se corresponde con la proporcion de tamaño de la imagen, esta se deformará. Para evitarlo, podemos usar la propiedad `object-fit`:

```css
img {
  width: 100%;
  height: auto;
  object-fit: cover;
}
```

Algunos de los valores que podemos usar para `object-fit` son:

- `fill`: La imagen se estira para cubrir todo el contenedor, pudiendo deformarse.
- `contain`: La imagen se estira para cubrir todo el contenedor, sin deformarse.
- `cover`: La imagen se estira para cubrir todo el contenedor, sin deformarse, y se recorta si es necesario.
- `none`: La imagen se muestra a su tamaño original.
- `scale-down`: La imagen se muestra a su tamaño original, o más pequeña si es necesario.

## Selección de imágenes

Generalmente, usaremos `src` para indicar la ruta de la imagen que queremos mostrar. Sin embargo, podemos usar `srcset` para indicar diferentes rutas de la imagen, y que el navegador seleccione la más adecuada dependiendo del tamaño de la pantalla.

```html
<img src="imagen.jpg" srcset="imagen.jpg 1x, imagen2x.jpg 2x, imagen3x.jpg 3x">
```

```html
<img src="imagen.jpg" srcset="imagen.jpg 300w, imagen2x.jpg 600w, imagen3x.jpg 900w">
```

Debemos añadir `sizes` para indicar el tamaño del contenedor en el que se mostrará la imagen.

```html
<img src="imagen.jpg" srcset="imagen.jpg 300w, imagen2x.jpg 600w, imagen3x.jpg 900w" sizes="(max-width: 600px) 300px, 600px">
```

