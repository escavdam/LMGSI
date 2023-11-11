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
