# keyframes

Los keyframes en css nos permiten crear animaciones.

Para crear una animación, primero debemos definir los keyframes con la propiedad `@keyframes` y luego aplicarlos a un elemento con la propiedad `animation`.

```css
@keyframes nombre {
  0% {
    /* Estilos */
  }
  100% {
    /* Estilos */
  }
}

.elemento {
  animation: nombre 1s infinite;
}
```

En este ejemplo, hemos creado una animación llamada `nombre` que se ejecutará durante `1s` y se repetirá infinitamente.

Los keyframes nos permiten definir los estilos que queremos que tenga un elemento en diferentes momentos de la animación.

En el ejemplo anterior, hemos definido que en el momento `0%` el elemento tenga unos estilos y que en el momento `100%` tenga otros.

Podemos definir tantos momentos como queramos.

```css
@keyframes nombre {
  0% {
    /* Estilos */
  }
  50% {
    /* Estilos */
  }
  100% {
    /* Estilos */
  }
}
```

En este ejemplo, hemos definido que en el momento `0%` el elemento tenga unos estilos, que en el momento `50%` tenga otros y que en el momento `100%` tenga otros.

## Animar elementos:

Podemos cambiar cualquier propiedad CSS en nuestros keyframes:

```css
*{
  margin: 0;
  padding: 0;
}
.container{
  background: black;
  
}
@keyframes anim1 {
  0% {
    width: 0vw;
    height: 0vh;
  }
  100% {
    width: 100vw;
    height: 100vh;
  }

}

.container {
  animation: anim1 5s infinite ease-in-out;
}
```

En este ejemplo, hemos creado una animación que hace que el elemento `.container` crezca desde `0vw` y `0vh` hasta `100vw` y `100vh` en `5s` y que se repita infinitamente, ademas hemos añadido un efecto de aceleración y desaceleración usando `ease-in-out`.

## Animar elementos con transformaciones:

Podemos usar transformaciones para animar elementos:

```css
*{
  margin: 0;
  padding: 0;
}

.container{
  background: black;
  width: 100vw;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
}

@keyframes anim1 {
  0% {
    transform: rotate(0deg);
  }
  100% {
    transform: rotate(360deg);
  }

}

.container {
  animation: anim1 5s infinite linear;
}
```

**Recuerda** que puedes usar transform para muchos de estos efectos:





