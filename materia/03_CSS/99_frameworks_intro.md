# Frameworks CSS

## ¿Qué es un framework?

Un framework CSS es un conjunto de estilos CSS que nos permiten crear páginas web de forma más rápida y sencilla. Los frameworks CSS nos proporcionan una serie de estilos CSS predefinidos que podemos usar en nuestras páginas web directamente.

## ¿Por qué usar un framework CSS?

La mayoría de frameworks CSS nos prometen que podemos crear páginas web de forma más rápida y sencilla. Esto hasta cierto punto es cierto, pero un framework no siempre será la solución a nuestros problemas.

No intentéis evitar CSS mediante el uso de frameworks, CSS es un lenguaje muy potente y es importante conocer bien sus aspectos básicos, de lo contrario podéis acabar peleando contra clases y estilos definidos por la librería sin entender como estos funcionan.

Además, la fama de CSS de ser un lenguaje difícil de aprender es en parte culpa de los frameworks CSS, ya que estos nos evitan escribir CSS, pero no nos evitan tener que aprender como funcionan.

Esta dificultad ha ido reduciendose con el tiempo y varias actualizaciones de CSS, cada vez es más fácil hacer una web responsive sin necesidad de añadir estilos extra.

### Pros:

- Podemos olvidarnos de escribir CSS si nos limitamos a usar los estilos que incluye el framework.
- Según el framework, estos estilos pueden modificarse, por lo que podemos personalizarlos y adaptarlos a nuestras necesidades.
- Si trabajamos en equipo, los frameworks CSS nos permiten tener un código más limpio y ordenado, ya que todos los miembros del equipo seguirán las mismas convenciones.
- Añaden comportamientos responsive a nuestra página, nos soluciona uno de los aspectos más complicados de diseñar web.
- Suelen ser compatibles con la mayoría de navegadores, por lo que no tenemos que preocuparnos por la compatibilidad.
- Nos ayudarán a desarrollar nuestras habilidades de estructuración de código, ya que estamos obligados a seguir las indicaciones del framework para que los componentes funcionen bien, y nos dejan iterar mas rápido nuestra página o aplicación.
- Eventualmente, se pueden quitar y reemplazarlos por estilos propios, este proceso puede ser tedioso dependiendo de la cantidad de componentes que se hayan usado, pero el proceso puede realizarse de forma gradual.

### Contras:

- Pueden llegar a ser muy pesados, por lo que pueden afectar al rendimiento de la página web, además, podemos estar sobrecargando la página con estilos que no vamos a usar pero que están incluidos en el framework.
- Pueden llegar a ser muy restrictivos, por lo que podemos tener problemas para personalizar los estilos.
- Nos evitan escribir CSS, pero deberemos aprender como funcionan clases y componentes escritos por otras personas.
- Si no tenemos cuidado, podemos acabar con una página web que se parece a **cualquiera**.

## ¿Qué framework CSS usar?

Existen **muchos** frameworks CSS, vamos a ver algunos de los más populares según sus tipos:

### Frameworks CSS semánticos

Los frameworks CSS semánticos son frameworks que nos proporcionan estilos CSS para elementos HTML, simplemente tenemos que preocuparnos por escribir HTML usando los tags que nos proporciona el framework.

Pueden hacer uso de clases, pero en muchos casos no es necesario, o solo es para ciertos componentes.

- [Bootstrap](https://getbootstrap.com/), es el framework CSS más popular, es **muy** completo y hay mucha documentación sobre la misma, depende de jQuery y utiliza algunas clases para algunos de sus componentes, añadirá **mucho** código a nuestra página web.
- [Semantic UI](https://semantic-ui.com/), este framework CSS es muy similar a Bootstrap, pero utiliza **menos clases**, dejando tu HTML más limpio.

### Frameworks CSS minimalistas

Los frameworks CSS minimalistas se centran en proporcionar estilos CSS para tus elementos HTML, intentando añadir el mínimo código y peso posible a tu página web.

- [Picocss](https://picocss.com/), es un framework semántico minimalista, casi no tiene clases, no tiene dependencias y pesa **menos de 1kb**, extremadamente ligero, personalizable, fácil de escalar y añadir tus propios estilos.
- [Bulma](https://bulma.io/), es un framework CSS muy completo, es muy similar a Bootstrap, pero usa  **menos clases**, y es mucho mas ligero, mucho mas completo que `Picocss`, siendo casi igual de minimalista.

### Frameworks CSS de componentes

Los frameworks CSS de componentes nos proporcionan estilos CSS para componentes, por lo que deberemos usar la estructura y clases que nos proporciona el framework para crear nuestros componentes y estilizarlos.

- [Tailwind](https://tailwindcss.com/), es un framework CSS que nos proporciona estilos CSS para componentes. Es un framework muy completo y de los más populares en equipos grandes, pero no es semántico, por lo que deberemos usar clases para crear nuestros componentes.
- [Materialize](https://materializecss.com/), es un framework CSS que nos proporciona estilos CSS para componentes. Es el framework que usa google en sus aplicaciones.

## ¿Cómo usar un framework CSS?

### Localmente

Cuando descargamos un framework CSS, este suele venir con varios archivos CSS, añade el necesario a tu proyecto, y referencialo como hemos hecho hasta ahora con nuestros estilos:

```html
<link rel="stylesheet" href="bootstrap.css">
```

### CDN

Algunos frameworks CSS están disponibles en un CDN, por lo que podemos añadirlos a nuestro proyecto mediante una etiqueta `<link>` y la url correspondiente:

```html
<link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
```

Adicionalmente, algunos frameworks CSS pueden requerir que añadamos algún fichero `.js` o alguna librería externa mediante `<script>`, por lo que deberemos leer la documentación del framework para saber como usarlo.