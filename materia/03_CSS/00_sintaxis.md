# CSS

[MDN Introduccion](https://developer.mozilla.org/es/docs/Learn/CSS/First_steps)

CSS (Cascading Style Sheets) es un lenguaje de hojas de estilo creado para controlar el aspecto o presentación de los documentos electrónicos definidos con HTML y XHTML. CSS es la mejor forma de separar los contenidos y su presentación y es imprescindible para crear páginas web complejas.

## ¿Qué es CSS?

CSS será el lenguaje que usaremos para darle estilo a nuestra página web. CSS es un lenguaje de hojas de estilo, esto quiere decir que nos permite definir estilos para los elementos de nuestra página web.

Es **muy** importante saber CSS si quieres dedicarte al front-end, ya que es el lenguaje que nos permite darle estilo a nuestra página web.

Es un lengaje **clave** en el desarrollo web, por mucho que os guste el backend, necesitas un mínimo de CSS para poder hacer tu trabajo y diseñar al menos una interfaz básica.

Las librerías de CSS como Bootstrap, Materialize, etc. son muy útiles, pero no os ayudarán a "esquivar" CSS, ya que al final del día, estas librerías están hechas con CSS.

Necesitaréis aprender conceptos que vienen tanto del mundo del diseño, como de la maquetación, que pueden ser aspectos mucho menos lógicos y tecnológicos, esto hace que mucha gente se sienta abrumada por CSS, acaben infravalorando su importancia y no le dediquen el tiempo necesario.

## ¿Cómo funciona CSS?

En realidad, las bases de CSS son muy sencillas, pero a medida que vamos avanzando, nos encontramos con conceptos más complejos.

CSS funciona con **selectores** y **propiedades**.

Los **selectores** son los elementos a los que queremos dar estilo, por ejemplo, los elementos `h1` o `p` de nuestro HTML, o los elementos con una `class` o `id` declarados como atributo.

Las **propiedades** son los estilos que queremos aplicar a los elementos seleccionados, por ejemplo, el color, el tamaño, la posición, etc.

## Sintaxis

La sintaxis de CSS es muy sencilla, se compone de un **selector** y una **propiedad**.

```css
selector {
  propiedad: valor;
}
```

Por ejemplo, si queremos darle un color rojo a todos los elementos `h1` de nuestra página web, escribiríamos lo siguiente:

```css
h1 {
  color: red;
}
```
