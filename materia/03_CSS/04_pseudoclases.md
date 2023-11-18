# Pseudoclases

[MDN Introduccion a pseudoclases y pseudoelementos](https://developer.mozilla.org/es/docs/Learn/CSS/Building_blocks/Selectors/Pseudo-classes_and_pseudo-elements)

[MDN Pseudoclases](https://developer.mozilla.org/es/docs/Web/CSS/Pseudo-classes)

Las pseudoclases nos permiten seleccionar elementos en base a su estado, por ejemplo, si el ratón está encima de un elemento, si un elemento está seleccionado, etc.

Las pseudoclases disponibles son:

- `:active`: Selecciona un elemento cuando está activo, por ejemplo, cuando hacemos click en un enlace.
- `:checked`: Selecciona un elemento cuando está marcado, por ejemplo, un checkbox.
- `:disable`: Selecciona un elemento cuando está deshabilitado, por ejemplo, un botón deshabilitado.
- `:empty`: Selecciona un elemento cuando está vacío, por ejemplo, un elemento `div` sin contenido.
- `:enabled`: Selecciona un elemento cuando está habilitado, por ejemplo, un botón habilitado.
- `:first-child`: Selecciona el primer elemento hijo de otro elemento.
- `:last-child`: Selecciona el último elemento hijo de otro elemento.
- `:first-of-type`: Selecciona el primer elemento de un tipo.
- `:focus`: Selecciona un elemento cuando tiene el foco, por ejemplo, un `input` cuando hacemos click en él.
- `:hover`: Selecciona un elemento cuando el ratón está encima de él.
- `:in-range`: Selecciona un elemento cuando está dentro de un rango, por ejemplo, un `input` de tipo `number` cuando su valor está dentro del rango especificado.

## 

Las pseudoclases son muy utiles para poder seleccionar elementos en base a su estado, por ejemplo, para cambiar el color de un enlace cuando el ratón está encima de él:

```css
a:hover {
  color: red;
}
```

Pero también podemos usarlas para seleccionar elementos que no tienen un estado concreto, por ejemplo, para seleccionar el primer elemento `p` de un elemento `div`:

```css
div p:first-child {
  color: red;
}
```

Otro ejemplo, aqui siempre seleccionamos el ultimo elemento, independientemente del tipo:

```css
div :last-child {
  color: red;
}
```
