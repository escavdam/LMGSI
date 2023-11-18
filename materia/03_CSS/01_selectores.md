# Selectores

[MDN Selectores](https://developer.mozilla.org/es/docs/Web/CSS/CSS_selectors)

Los selectores nos permiten acceder a nuestros elementos HTML y darles estilo.

## Selectores de etiqueta

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

## Selectores de clase

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

## Selectores de id

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