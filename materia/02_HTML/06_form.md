# form

Los formularios son una parte importante de la web. Nos permiten enviar datos al servidor para que este los procese y nos devuelva una respuesta.

La etiqueta `<form>` nos permite agrupar inputs y enviar su resultado al servidor.

```html 
<form action="https://www.google.com/search" method="GET">
    <input type="text" name="q">
    <input type="submit" value="Buscar">
</form>
```

## Atributos

### action

El atributo `action` nos permite indicar la URL a la que se enviarán los datos del formulario.

### method

El atributo `method` nos permite indicar el método HTTP que se usará para enviar los datos del formulario. Los métodos más comunes son `GET` y `POST`.

### target

El atributo `target` nos permite indicar en qué ventana se abrirá la respuesta del servidor. Los valores más comunes son `_blank` y `_self`.

### autocomplete

El atributo `autocomplete` nos permite indicar si el navegador debe completar automáticamente los campos del formulario. Los valores más comunes son `on` y `off`.

### enctype

El atributo `enctype` nos permite indicar el tipo de codificación que se usará para enviar los datos del formulario. Las codificaciones más comunes son `application/x-www-form-urlencoded` cuando se envían datos de texto, `multipart/form-data` cuando se envían archivos (imágenes, videos, etc) o `text/plain` cuando se envían datos de texto sin formato.

## Submit

Los formularios tienen un botón de tipo `submit` que nos permite enviar los datos del formulario al servidor.

```html
<form action="https://www.google.com/search" method="GET">
    <input type="text" name="q">
    <input type="submit" value="Buscar">
</form>
```

Cuando hacemos submit se lanza un evento `submit` que podemos capturar desde JavaScript. Este evento tambien se lanza cuando el usuario usa la tecla `Enter` para enviar el formulario.

```js
const form = document.querySelector('form');

form.addEventListener('submit', (event) => {
    event.preventDefault();
    //haz algo con tu formulario
    console.log('Formulario enviado');
});
```

## FormData

El objeto `FormData` nos permite acceder a los datos de un formulario desde JavaScript.

```html 
<form action="/usuarios" method="POST">
  <label for="usuario">Usuario</label>
  <input type="text" name="usuario">
  
  <label for="password">Password</label>
  <input type="password" name="password">
  
  <input type="submit">
</form>
```

```js
const form = document.querySelector('form');

form.addEventListener('submit', (event) => {
    event.preventDefault();
    const formData = new FormData(form);
    console.log(formData.get('q'));
});
```

DataForm sólo funciona con inputs que tengan un atributo `name`, si un input no tiene un atributo `name` no se incluirá en el objeto `FormData`.

Para enviar un formulario con JavaScript podemos usar el método `submit()`.

```js
const form = document.querySelector('form');

form.addEventListener('submit', (event) => {
    event.preventDefault();
    const formData = new FormData(form);
    console.log(formData.get('q'));
    form.submit();
});
```

O nuestros propios métodos `fetch()` o `XMLHttpRequest()`.

```js
const form = document.querySelector('form');

form.addEventListener('submit', (event) => {
    event.preventDefault();
    const formData = new FormData(form);
    console.log(formData.get('q'));
    fetch(form.action, {
        method: form.method,
        body: formData
    });
});
```




