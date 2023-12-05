# BEM

BEM es un acrónimo de Block, Element, Modifier. Es una metodología de nomenclatura para nombrar clases en CSS.

## ¿Por qué usar BEM?

Algunos de los principales problemas que encontramos cuando nombramos clases en CSS sin una metodología son:

- **Especificidad**: Si tenemos dos clases con el mismo nombre, pero una de ellas está dentro de otra, la clase más específica tendrá más prioridad que la clase menos específica.

- **Colisión de clases**: Si tenemos dos clases con el mismo nombre en diferentes componentes, estas clases pueden colisionar y provocar que nuestro código CSS no funcione correctamente. Incluso si el estilo de ambas clases es el mismo, semánticamente no es correcto.

- **Escalabilidad**: Nuestro código CSS puede volverse muy difícil de mantener si no tenemos una nomenclatura clara.

BEM nos ayuda a solucionar estos problemas, **no** es una solución perfecta, entre algunas de sus contras se encuentran:

- **Verbosidad**: BEM puede hacer que nuestro código HTML y CSS sea más largo.

- **Dificultad de aprendizaje**: BEM puede ser difícil de aprender al principio.

## ¿Cómo funciona BEM?

BEM nos propone una nomenclatura para nombrar clases en CSS, esta nomenclatura se basa en tres conceptos:

- **Block**: Un bloque es un componente independiente de nuestra página web. Por ejemplo, un menú de navegación, un botón, un formulario, etc.

- **Element**: Un elemento es una parte de un bloque.

- **Modifier**: Un modificador es una clase que modifica el estilo de un bloque o un elemento.

### Block

Un bloque es un componente independiente de nuestra página web. Por ejemplo, un menú de navegación, un botón, un formulario, etc.

La idea de un bloque es poderlo reutilizar en diferentes partes de nuestra página web, por eso es importante que los bloques sean independientes.

Para nombrar un bloque, usaremos un nombre en minúsculas, sin espacios, y usando guiones para separar palabras. Este nombre debe ser único, y debe describir el propósito del bloque semánticamente:

```css
/* Block */
.menu-lateral {
  /* ... */
}

.form-login {
  /* ... */
}

.tarjeta-empleado {
  /* ... */
}
```

### Element

Un elemento es una parte de un bloque. Puede ser cualquier elemento HTML, como un párrafo, un botón, un enlace, etc.

Para nombrar un elemento, usaremos el nombre del bloque, seguido de dos guiones bajos, seguido del nombre del elemento. Este nombre debe ser único, y debe describir el propósito del elemento semánticamente:

```css
.menu-lateral {
    /* Block */
}
.menu-lateral__item {
    /* Element */
}
.menu-lateral__imagen {
    /* Element */
}
.menu-lateral__item__icono {
    /* Element */
}
```

### Modifier

Un modificador es una clase que modifica el estilo de un bloque o un elemento.

Para nombrar un modificador, usaremos el nombre del bloque o elemento, seguido de dos guiones, seguido del nombre del modificador. Este nombre debe ser único, y debe describir el propósito del modificador semánticamente:

```css
.menu-lateral {
    /* Block */
}
.menu-lateral--oculto {
    /* Modifier */
}
.menu-lateral__item {
    /* Element */
}
.menu-lateral__item--activo {
    /* Modifier */
}
```


