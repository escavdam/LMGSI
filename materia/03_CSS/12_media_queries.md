# Mediaquery

mediaquery es una característica de CSS3 que permite adaptar el contenido a diferentes dispositivos, como por ejemplo, pantallas de ordenador, tablets, móviles, etc.

## Sintaxis

```css
@media <tipo> and <condición> {
  /* Estilos */
}
```

## Tipos

- `all`: Todos los dispositivos.
- `print`: Dispositivos de impresión.
- `screen`: Dispositivos de pantalla, como ordenadores, tablets, móviles, etc. Es el más usado.
- `speech`: Dispositivos de voz.
- `tv`: Dispositivos de televisión.
- `handheld`: Dispositivos portátiles, como móviles, tablets, etc.
- `projection`: Dispositivos de proyección.
- `braille`: Dispositivos de braille.

## Condiciones

Las condiciones nos permiten indicar las características del dispositivo para el que queremos aplicar los estilos.

### Ancho y alto

```css
@media screen and (min-width: 768px) {
  /* Estilos */
}
```

En este ejemplo, los estilos se aplicarán a dispositivos de pantalla con un ancho mínimo de `768px`.

```css
@media screen and (max-width: 768px) {
  /* Estilos */
}
```

En este ejemplo, los estilos se aplicarán a dispositivos de pantalla con un ancho máximo de `768px`.

```css
@media screen and (min-width: 768px) and (max-width: 1024px) {
  /* Estilos */
}
```

En este ejemplo, los estilos se aplicarán a dispositivos de pantalla con un ancho mínimo de `768px` y un ancho máximo de `1024px`.

Podemos establecer condiciones para el alto de la misma forma usando `min-height` y `max-height`.

Usando las mediaqueries podemos adaptar el contenido a diferentes dispositivos, por ejemplo, podemos adaptar el ancho de un contenedor según el ancho de la pantalla:

```css
.container{
  width: 100%;
  padding: 2rem;
  background: #333;
  text-align: center;
  color: white;
  margin: 0 auto;
}

@media screen and (min-width: 768px){  
  .container{
    width: 50vw;
  }
}

```

Algunos de los tamaños de pantalla más comunes son:

- `320px`: Móviles.
- `768px`: Tablets.
- `1024px`: Tablets y ordenadores pequeños.
- En sobremesa hay absolutamente de todo, pero los más comunes son `1280px`, `1366px`, `1440px`, `1600px` y `1920px`.
- Hay personas con pantallas de `2560px` o más, cada vez son más comunes, pero no son la mayoría.

### Orientación

Modo horizontal:

```css
@media screen and (orientation: landscape) {
  /* Estilos */
}
```

Modo vertical:

```css
@media screen and (orientation: portrait) {
  /* Estilos */
}
```
