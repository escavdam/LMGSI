# CSS

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

## Selectores

Los selectores nos permiten acceder a nuestros elementos HTML y darles estilo.

### Selectores de etiqueta

Los selectores de etiqueta nos permiten seleccionar todos los elementos de un tipo en concreto.

Para usarlos, solo debemos escribir el nombre de la etiqueta.

```css
h1 {
  color: red;
}

p {
  color: blue;
}

a {
  color: green;
}
```

### Selectores de clase

Los selectores de clase nos permiten seleccionar todos los elementos que tengan una clase en concreto.

Las clases se declaran en el HTML con el atributo `class`.

```html	
<p class="parrafo">Soy un párrafo</p>
```

Para usarlos, debemos escribir un punto `.` seguido del nombre de la clase.

```css
.parrafo {
  color: red;
}
```

**Recordad** que las clases pueden ser reutilizadas, podemos tener varios elementos con la misma clase.

### Selectores de id

Los selectores de id nos permiten seleccionar todos los elementos que tengan un id en concreto.

Los id se declaran en el HTML con el atributo `id`.

```html
<p id="parrafo">Soy un párrafo</p>
```

Para usarlos, debemos escribir una almohadilla `#` seguido del nombre del id.

```css
#parrafo {
  color: red;
}
```

**Recordad** que los id deben ser únicos, no debemos tener dos elementos con el mismo id.

### Propiedades

Las propiedades son los estilos que queremos aplicar a los elementos seleccionados.

Las propiedades se escriben en minúsculas y si tienen más de una palabra, se separan con un guión `-`.

```css
h1 {
  color: red;
  font-size: 20px;
}
```

Vamos a ver algunas de las propiedades más importantes.

#### color

La propiedad `color` nos permite cambiar el color del texto.

Podemos utilizar colores por nombre, por ejemplo `red` o `blue`, valores hexadecimales como `#FF00FF` o valores RGBA mediante la funcion `rgba(r, g, b, a)`.

```css
h1 {
  color: red;
}

p {
  color: #0000ff;
}
    
a {
  color: rgba(0, 0, 255, 0.5);
}
```

#### background

La propiedad `background` nos permite cambiar el color de fondo de un elemento.

Podemos usar los mismos tipos de colores que con la propiedad `color`.

```css
h1 {
  background: red;
}

body{
    background: #000000;
    color: #FFFFFF;
}
```

#### font-size

La propiedad `font-size` nos permite cambiar el tamaño de la fuente.

Podemos usar valores en píxeles `px`, puntos `pt`, porcentajes `%`, etc.

```css
h1 {
  font-size: 20px;
}
```

#### font-family

La propiedad `font-family` nos permite cambiar la fuente.

```css
h1 {
  font-family: "Comic Sans MS";
}
```

#### text-align

La propiedad `text-align` nos permite alinear el texto.
Podemos usar los valores `left`, `right`, `center` o `justify`.

```css
h1 {
  text-align: center;
}
```

#### width

La propiedad `width` nos permite cambiar el ancho de un elemento.

```css
div {
  width: 100px;
}
```

Tenemos otras propiedades relacionadas con el ancho, como `max-width` o `min-width`.

#### height

La propiedad `height` nos permite cambiar el alto de un elemento.

```css
div {
  height: 100px;
}
```

Tenemos otras propiedades relacionadas con el alto, como `max-height` o `min-height`.

#### margin

La propiedad `margin` nos permite cambiar el margen de un elemento.

```css
p {
  margin: 100px;
}
```

El margen es el espacio que hay entre el elemento y los elementos de alrededor.

#### padding

La propiedad `padding` nos permite cambiar el relleno de un elemento.

```css
p {
  padding: 100px;
}
```

El relleno es el espacio que hay entre el contenido del elemento y el borde.

#### border

La propiedad `border` nos permite cambiar el borde de un elemento.

```css
p {
  border: 1px solid black;
}
```

El borde es la linea que separa el contenido del elemento y el padding del margen.

### Interacción entre padding, border y margin:

Las propiedades `padding`, `border` y `margin` son propiedades que interactúan entre ellas en un mismo elemento.

Puede ser muy útil inspeccionar un elemento para entender las propiedades que tiene, considera el siguiente `html`:

```html
  <p>Hola mundo</p>
  <p>Este párrafo contiene una línea</p>
  <p>Otro parrafo con mas información</p>
```

Y el siguiente `css` asociado:

```css
p {
  border: 1px solid black;
  padding: 10px;
  margin: 20px;
}
```

Analizando sus propiedades en la consola:

![Margin, padding y border](/02_CSS/images/border_margin_padding.png)

Podemos comprobar que el elemento tiene un borde de 1px, un padding de 10px y un margin de 20px.

### Pseudoclases

Las pseudoclases nos permiten seleccionar elementos en base a su estado, por ejemplo, si el ratón está encima de un elemento, si un elemento está seleccionado, etc.

Las pseudoclases disponibles son:

- `:active`: Selecciona un elemento cuando está activo, por ejemplo, cuando hacemos click en un enlace.
- `:checked`: Selecciona un elemento cuando está marcado, por ejemplo, un checkbox.
- `:disabled`: Selecciona un elemento cuando está deshabilitado, por ejemplo, un botón deshabilitado.
- `:empty`: Selecciona un elemento cuando está vacío, por ejemplo, un elemento `div` sin contenido.
- `:enabled`: Selecciona un elemento cuando está habilitado, por ejemplo, un botón habilitado.
- `:first-child`: Selecciona el primer elemento hijo de otro elemento.
- `:first-of-type`: Selecciona el primer elemento de un tipo.
- `:focus`: Selecciona un elemento cuando tiene el foco, por ejemplo, un `input` cuando hacemos click en él.
- `:hover`: Selecciona un elemento cuando el ratón está encima de él.
- `:in-range`: Selecciona un elemento cuando está dentro de un rango, por ejemplo, un `input` de tipo `number` cuando su valor está dentro del rango especificado.

```css
a{
    background: black;
    color: white;
}

a:hover {
    background: red;
    color: black;
}
```

