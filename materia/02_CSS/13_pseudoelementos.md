# Pseudoelementos

Los pseudoelementos nos permiten seleccionar partes de un elemento, por ejemplo, el primer párrafo de un elemento `div`.

Los pseudoelementos disponibles son:

- `::after`: Selecciona la parte de después de un elemento.
- `::before`: Selecciona la parte de antes de un elemento.
- `::first-letter`: Selecciona la primera letra de un elemento.
- `::first-line`: Selecciona la primera línea de un elemento.
- `::selection`: Selecciona el texto seleccionado por el usuario.
- `::backdrop`: Selecciona el fondo detrás de un elemento.
- `::placeholder`: Selecciona el texto de un elemento `input` o `textarea` que no ha sido rellenado.

Algunos de los pseudoelementos más usados son `::after` y `::before`, que nos permiten insertar contenido antes o después de un elemento, considera el siguiente ejemplo:

```html
<p>Esto es un párrafo</p>
```

```css
p::after {
  content: " - Fin del párrafo";
}

p::before {
  content: "Inicio del párrafo - ";
}
```

Tambien podemos afectar a la primera letra de un elemento:

```css
p::first-letter {
  font-size: 300%;
}
```

O a la primera línea:

```css
p::first-line {
  font-weight: bold;
}
```
