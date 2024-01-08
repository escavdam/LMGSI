# Transform

Transform nos deja modificar la posición, rotación y escala de un elemento mediante las siguientes propiedades:

- `translate`: Nos permite modificar la posición del elemento.
- `rotate`: Nos permite modificar la rotación del elemento.
- `scale`: Nos permite modificar la escala del elemento.
- `skew`: Nos permite modificar la inclinación del elemento.
- `transform-origin`: Nos permite modificar el punto de origen de la transformación.
- `transform`: Nos permite aplicar varias transformaciones a la vez.
- `perspective`: Nos permite modificar la perspectiva de un elemento.

## translate

Translate nos permite modificar la posición de un elemento.

```css
.box {
  transform: translate(100px, 100px);
}
```

En este ejemplo, hemos movido el elemento `.box` `100px` hacia la derecha y `100px` hacia abajo.

Podemos usar `translateX` y `translateY` para mover el elemento solo en un eje.

```css
.box {
  transform: translateX(100px);
}
```

En este ejemplo, hemos movido el elemento `.box` `100px` hacia la derecha.

## rotate

Rotate nos permite modificar la rotación de un elemento.

```css
.box {
  transform: rotate(45deg);
}
```

En este ejemplo, hemos rotado el elemento `.box` `45deg`.

```css 
.box {
    width: 100px;
    height: 100px;
    transition: 0.5s;
}

.box:hover{
    transform: rotate(45deg);
}

```