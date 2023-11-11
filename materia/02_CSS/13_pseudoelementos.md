# Pseudoelementos

Los pseudoelementos nos permiten seleccionar partes de un elemento, por ejemplo, el primer párrafo de un elemento `div`.

Los pseudoelementos disponibles son:

- `::after`: Selecciona la parte de después de un elemento.
- `::before`: Selecciona la parte de antes de un elemento.
- `::first-letter`: Selecciona la primera letra de un elemento.
- `::first-line`: Selecciona la primera línea de un elemento.
- `::selection`: Selecciona el texto seleccionado por el usuario.

```css
p::first-letter {
  font-size: 300%;
}
```
