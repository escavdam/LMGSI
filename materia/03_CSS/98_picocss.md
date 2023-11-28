# Picocss

[Picocss](https://picocss.com/) es un framework CSS minimalista, que nos proporciona estilos CSS para nuestros elementos HTML, pero sin añadir mucho peso ni JS adicional a nuestra página web.

[Documentación](https://picocss.com/docs/)
[Guía de inicio](https://picocss.com/docs/getting-started/)

[Guía de personalización](https://picocss.com/docs/customize/)
[Guía de componentes](https://picocss.com/docs/components/)
[Guía de utilidades](https://picocss.com/docs/utilities/)
[Guía de clases](https://picocss.com/docs/classes/)
[Guía de variables](https://picocss.com/docs/variables/)


## ¿Cómo usar Picocss?

Podemos descargar Picocss desde su [página web](https://picocss.com/), o podemos añadirlo a nuestro proyecto mediante un CDN:

```html
<link rel="stylesheet" href="https://unpkg.com/picocss/dist/pico.min.css">
```

Un proyecto limpio de Picocss puede ser algo así:

```html
<!DOCTYPE html>
<html lang="en" data-theme="light">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Picocss</title>
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@picocss/pico@1/css/pico.min.css">
</head>
<body>
  
</body>
</html>
```

## ¿Cómo funciona Picocss?

Una vez instalado en nuestro proyecto, podemos empezar a escribir HTML usando los elementos y clases que nos proporciona Picocss.

Picocss es un framework basado en la filosofía de [Mobile First](https://www.arkaitzgarro.com/mobile-first/), por lo que todos sus estilos están pensados para dispositivos móviles, y luego se van adaptando a pantallas más grandes.

Por ello, los elementos html en Picocss por defecto ocupan el 100% del ancho de la pantalla, y se van adaptando a pantallas más grandes:

```html
<body>
  <h1>Hola mundo</h1>
  <h2>Picocss</h2>
  <p>Estos elementos saldrán con su propio estilo si picocss esta correctamente instalado.</p>
</body>
```

## Layout

Podemos usar Picocss para crear un layout básico de nuestra página web, para ello, Picocss nos proporciona las clases `container` y `grid`.

### container

[Documentación](https://picocss.com/docs/containers.html)

La clase `container` nos permite crear un contenedor centrado en la pantalla, el contenedor tambien añade un padding a los lados, por lo que los elementos dentro del contenedor no ocuparán el 100% del ancho de la pantalla. Este contenedor posee diferentes breakpoints para adaptarse a diferentes tamaños de pantalla de manera responsiva:

```html
<body>
  <div class="container">
    <h1>Hola mundo</h1>
    <h2>Picocss</h2>
    <p>Estos elementos saldrán con su propio estilo si picocss esta correctamente instalado.</p>
  </div>
</body>
```

### grid

[Documentación](https://picocss.com/docs/grid.html)

Con grid podemos crear un sistema de columnas para nuestro layout, simplemente añade la clase `grid` a un contenedor semantico o generico, situa dentro de este los elementos que quieras que se comporten como columnas:
  
```html
<div class="grid">
    <p>Esto es una columna</p>
    <p>Esto es otra columna</p>
    <p>Esto es otra columna</p>
</div>
```
