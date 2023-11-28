# Data

Todos los elementos HTML pueden tener como propiedad `data-*`, donde `*` es cualquier nombre que queramos darle, esta propiedad nos permite almacenar información adicional sobre el elemento, y poder acceder a ella desde JavaScript o CSS.

## Acceder desde CSS

Podemos almacenar la URL de una imagen en la propiedad `data-img` de un elemento `<a>`:

```html
<a href="#" data-img="https://picsum.photos/200/300"> Lorem ipsum dolor sit amet, consectetur adipiscing elit. </a>
```

Y luego, desde CSS, podemos acceder a la propiedad `data-img` usando el selector `::before`:

```css
a::before {
    content: url(attr(data-img));
}
```

## Acceder desde JavaScript

Podemos almacenar el nombre de un usuario en la propiedad `data-user` de un elemento `<a>`:

```html
<a href="#" data-user="Manolo"> Lorem ipsum dolor sit amet, consectetur adipiscing elit. </a>
```

Y luego, desde JavaScript, podemos acceder a la propiedad `data-user` usando el método `getAttribute()`:

```js
const user = document.querySelector('a').getAttribute('data-user');
```