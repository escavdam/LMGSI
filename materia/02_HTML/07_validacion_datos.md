# Validación de datos

Validad datos significa comprobar que los datos que vamos a enviar a un servidor son correctos, por ejemplo, asegurarnos de que un email tiene el formato correcto, o limitar el número de caracteres que el usuario puede introducir en un campo.

Esta validación puede hacerse tanto en el cliente (en el navegador) como en el servidor. Mientras que validar datos en el servidor es **OBLIGATORIO**, validar datos en el cliente es **RECOMENDABLE**.

## Validación en el cliente

Cuando estemos validando datos en el cliente usaremos JavaScript, aunque nuestro servidor ya sea capaz de manejar esta validación, si validamos en el cliente antes de mandar los datos haremos que la experiencia de usuario sea mucho mejor. Además, limitar el número de datos que enviamos al servidor nos ayudará a reducir el consumo de ancho de banda y a tener más seguridad en nuestro servidor, ya que no tendremos que preocuparnos de que un usuario malintencionado envíe datos que no debería.

### Validación de formularios

Validar datos no es difícil, pero debemos combinar varias técnicas para conseguirlo de forma eficiente. La forma más común de validar datos es usando propiedades en nuestros inputs de formularios HTML.

#### required

El atributo `required` nos permite indicar que un campo es obligatorio, si el usuario intenta enviar el formulario sin rellenar un campo obligatorio el navegador le mostrará un mensaje de error.

```html
<form action="/usuarios" method="POST">
  <label for="usuario">Usuario</label>
  <input type="text" name="usuario" required>
  
  <label for="password">Password</label>
  <input type="password" name="password" required>
  
  <input type="submit">
</form>
```

#### pattern

El atributo `pattern` nos permite indicar una expresión regular que el valor del campo debe cumplir, si el valor del campo no cumple la expresión regular el navegador le mostrará un mensaje de error.

```html
<form action="/usuarios" method="POST">
  <label for="usuario">Usuario</label>
  <input type="text" name="usuario" pattern="[a-z]{3,10}" required>
  
  <label for="password">Password</label>
  <input type="password" name="password" required>
  
  <input type="submit">
</form>

```

#### minlength y maxlength

Los atributos `minlength` y `maxlength` nos permiten indicar el número mínimo y máximo de caracteres que el usuario puede introducir en un campo, si el usuario introduce un número de caracteres que no cumple con estas restricciones el navegador le mostrará un mensaje de error.

```html
<form action="/usuarios" method="POST">
  <label for="usuario">Usuario</label>
  <input type="text" name="usuario" minlength="3" maxlength="10" required>
  
  <label for="password">Password</label>
  <input type="password" name="password" required>
  
  <input type="submit">
</form>
```

#### min y max

Los atributos `min` y `max` nos permiten indicar el valor mínimo y máximo que el usuario puede introducir en un campo, si el usuario introduce un valor que no cumple con estas restricciones el navegador le mostrará un mensaje de error.

```html
<form action="/usuarios" method="POST">
  <label for="usuario">Usuario</label>
  <input type="text" name="usuario" minlength="3" maxlength="10" required>
  
  <label for="password">Password</label>
  <input type="password" name="password" required>
  
  <label for="edad">Edad</label>
  <input type="number" name="edad" min="18" max="99" required>
  
  <input type="submit">
</form>
```

#### step

El atributo `step` nos permite indicar el incremento que se debe usar al incrementar o decrementar el valor de un campo, por ejemplo, si el valor de un campo es `10` y el `step` es `2`, al incrementar el valor del campo el valor será `12`.

```html
<form action="/usuarios" method="POST">
  <label for="usuario">Usuario</label>
  <input type="text" name="usuario" minlength="3" maxlength="10" required>
  
  <label for="password">Password</label>
  <input type="password" name="password" required>
  
  <label for="edad">Edad</label>
  <input type="number" name="edad" min="18" max="99" step="2" required>
  
  <input type="submit">

</form>
```

#### type="xxxx"

El atributo `type` nos permite indicar el tipo de datos que se deben introducir, además de aportar funcionalidad extra al campo, por ejemplo, si el tipo de datos es `email` el navegador comprobará que el valor del campo tiene el formato de un email.

```html
<form action="/usuarios" method="POST">
  <label for="usuario">Usuario</label>
  <input type="text" name="usuario" minlength="3" maxlength="10" required>
  
  <label for="password">Password</label>
  <input type="password" name="password" required>
  
  <label for="edad">Edad</label>
  <input type="number" name="edad" min="18" max="99" step="2" required>
  
  <label for="email">Email</label>
  <input type="email" name="email" required>
  
  <input type="submit">
</form>
```

#### checkValidity()

Podemos validar los datos que el usuario ha introducido en un formulario usando el método `checkValidity()`, este método devuelve `true` si los datos son válidos y `false` si no lo son, dependiendo de las restricciones que hayamos puesto en los campos del formulario.

```html
<form action="/usuarios" method="POST">
  <label for="usuario">Usuario</label>
  <input type="text" name="usuario" minlength="3" maxlength="10" required>
  
  <label for="password">Password</label>
  <input type="password" name="password" required>
  
  <label for="edad">Edad</label>
  <input type="number" name="edad" min="18" max="99" step="2" required>
  
  <label for="email">Email</label>
  <input type="email" name="email" required>
  
  <input type="submit">
</form>

<script>
  const form = document.querySelector('form');
  
  form.addEventListener('submit', (event) => {
    event.preventDefault();
    if (form.checkValidity()) {
      form.submit();
    }
  });
</script>
```

## Validación personalizada

Nuestra aplicación puede necesitar de algún tipo de validación que se escape de las posibilidades que nos ofrecen los atributos de los inputs de formularios HTML, por ejemplo, podemos querer comprobar que el usuario no puede usar ciertas palabras en su nombre de usuario, o comprobar que la contraseña tiene al menos una mayúscula, una minúscula y un número.

Dependerá de nuestras necesidades el tipo de validación que necesitemos, pero en cualquier caso, la validación personalizada se hace usando JavaScript.

```js
const form = document.querySelector('form');
const usuario = document.querySelector('.input_usuario');

form.addEventListener('submit', (event) => {
  event.preventDefault();
  if (form.checkValidity()) { // validacion de html
    
    //aqui podemos validar los datos que queramos

    if(usuario.value.length < 3) {
      console.log('El usuario debe tener al menos 3 caracteres');
      return;
    }
    if(usuario.value.length > 10) {
      console.log('El usuario no puede tener más de 10 caracteres');
      return;
    }

    form.submit();
  }
});
```

## Validación en el servidor

Validar datos en el servidor es **OBLIGATORIO**, los datos se pueden manipular desde el cliente en varios puntos:

- En el front, usando Javascript o modificando el HTML.
- Interceptar la petición una vez ha sido validada en el front, previo a enviarla al servidor.
- En el back, antes de capturar los datos.
- En el back, antes de devolver los datos.

Por lo tanto, **siempre** debemos validar los datos en el servidor.

Esta validación se puede hacer manualmente, escribiendo tus propias validaciones con las herramientas que te proporciona el lenguaje de programación que estés usando, o usando librerías que ya existen para validar datos.

