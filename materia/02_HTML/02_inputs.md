# Inputs

Además de elementos de texto e imágenes, HTML nos permite crear elementos de entrada de datos.

## `<input>`

La etiqueta `<input>` se utiliza para definir un campo de entrada de datos.

```html
<input type="text" >
```

El atributo `type` define el tipo de campo de entrada de datos. Los valores más comunes son:

- `text`: Campo de texto.
- `password`: Campo de contraseña.
- `email`: Campo de correo electrónico.
- `number`: Campo de número.
- `date`: Campo de fecha.
- `file`: Campo de archivo.
- `checkbox`: Campo de casilla de verificación.
- `radio`: Campo de botón de opción.
- `submit`: Campo de envío de formulario.


### Validación en el cliente

El atributo type no solo cambia el aspecto del campo de entrada de datos, añade también validación en el cliente.

Por ejemplo, si definimos un campo de entrada de datos de tipo `email`, el navegador nos mostrará un mensaje de error si el valor introducido no es un correo electrónico válido.

Esto es muy útil, ahorra trabajo al servidor comprobando ciertos datos antes de enviar el formulario, asi el usuario no debe esperar a la respuesta del mismo para saber si hay un error, además, aliviamos nuestros servidores.

## `<label>`

La etiqueta `<label>` se utiliza para definir una etiqueta de texto para un campo de entrada de datos.

```html
<label> Nombre: </label>
<input type="text" >
```

Es importante que la etiqueta `<label>` esté asociada al campo de entrada de datos mediante el atributo `for` y que el input tenga un `id` con el mismo valor.

```html
<label for="nombre"> Nombre: </label>
<input type="text" id="nombre">
```

Esto hará que al hacer clic en la etiqueta se seleccione el campo de entrada de datos.

## `<textarea>`

La etiqueta `<textarea>` se utiliza para definir un campo de entrada de datos de texto multilínea.

```html
<label for="comentario"> Comentario: </label>
<textarea id="comentario"></textarea>
```

## `<select>`

La etiqueta `<select>` se utiliza para definir un campo de entrada de datos de selección.

```html
<label for="pais"> País: </label>
<select id="pais">
    <option value="es"> España </option>
    <option value="fr"> Francia </option>
    <option value="uk"> Reino Unido </option>
</select>
```

## `<button>`

La etiqueta `<button>` se utiliza para definir un botón.

```html
<button> Enviar </button>
```

## `<form>`

La etiqueta `<form>` se utiliza para definir un formulario.

```html
<form>
    <label for="nombre"> Nombre: </label>
    <input type="text" id="nombre">
    <label for="comentario"> Comentario: </label>
    <textarea id="comentario"></textarea>
    <label for="pais"> País: </label>
    <select id="pais">
        <option value="es"> España </option>
        <option value="fr"> Francia </option>
        <option value="uk"> Reino Unido </option>
    </select>
    <button> Enviar </button>
</form>
```

Esto nos sirve para agrupar los elementos de entrada de datos y enviarlos todos juntos, además, nos permite definir un método de envío y una URL de destino.

```html
<form method="post" action="https://www.mibackendfavorito.com/login">
    <label for="nombre"> Nombre: </label>
    <input type="text" id="nombre">
    <label for="comentario"> Contraseña: </label>
    <input type="password" id="contraseña">
    <button> Enviar </button>
</form>
```

## `<fieldset>`

La etiqueta `<fieldset>` se utiliza para definir un grupo de elementos de entrada de datos.

```html
<form>
    <fieldset>
        <legend> Datos personales </legend>
        <label for="nombre"> Nombre: </label>
        <input type="text" id="nombre">
        <label for="comentario"> Comentario: </label>
        <textarea id="comentario"></textarea>
    </fieldset>
    <fieldset>
        <legend> Datos de contacto </legend>
        <label for="pais"> País: </label>
        <select id="pais">
            <option value="es"> España </option>
            <option value="fr"> Francia </option>
            <option value="uk"> Reino Unido </option>
        </select>
    </fieldset>
    <button> Enviar </button>
</form>
```

## `<datalist>`

La etiqueta `<datalist>` se utiliza para definir una lista de opciones para un campo de entrada de datos.

```html
<label for="pais"> País: </label>
<input type="text" id="pais" list="paises">
<datalist id="paises">
    <option value="es"> España </option>
    <option value="fr"> Francia </option>
    <option value="uk"> Reino Unido </option>
</datalist>
```

## `<output>`

La etiqueta `<output>` se utiliza para definir un campo de salida de datos.

```html
<label for="nombre"> Nombre: </label>
<input type="text" id="nombre">
<output for="nombre"></output>
```

## `<progress>`
La etiqueta `<progress>` se utiliza para definir una barra de progreso.

```html
<progress value="50" max="100"></progress>
```

## `<meter>`
La etiqueta `<meter>` se utiliza para definir un medidor.

```html
<meter value="50" min="0" max="100"></meter>
```

