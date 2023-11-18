# Practica 5

Deadline: ?

En esta práctica vamos a comenzar a usar el flujo de trabajo normal cuando desarrollamos, iniciaremos un repositorio lo clonaremos a nuestro pc y nos sincronizaremos en vscode, en este proyecto vamos estructurar una web básica con varias secciones en una misma página, en cada sección, exploraremos un aspecto diferente de HTML, CSS y JavaScript.

## Instrucciones

1. Crea un repositorio en [GitHub](https://github.com/new) con el nombre `practica_5`.
2. Clona el repositorio en tu pc.
3. Abre el repositorio en vscode.
4. Crea un archivo `index.html` y añade el código base de html.
5. Crea un archivo `style.css`, asegurate de añadirlo a tu html.
6. Crea un archivo `script.js`, asegurate de añadirlo a tu html.
7. Edita tu archivo html, css y js de la forma mas mínima posible, de forma que veas que todo funciona correctamente.

👀 Asegurate de que todo funcione bien...

🚨 ¡Listo! Avisa y espera al resto de compañeros.

## Secciones

Ahora que tenemos todo listo, vamos a crear las secciones de la web, cada una corresponde a un ejercicio separado que nos ayudará a practicar diferentes conceptos.

Recuerda avisar cuando termines cada sección, mientras esperas a que los demás terminen, puedes ayudar a tus compañeros y trabajar en las funcionalidades extra.

### Emoji Aleatorio

En esta sección vamos a crear un h2 centrado que muestre un emoji aleatorio cada vez que se recarga la página, y que muestre otro emoji aleatorio cada vez que se hace click en el mismo.

1. Crea un elemento h2 centrado en la seccion.
2. Haz que se muestre un emoji aleatorio en el h2 cada vez que se recarga la página.
3. Haz que cada vez que se pulse en el emoji se muestre otro emoji aleatorio.

🚨 ¡Listo! Avisa y espera al resto de compañeros.

> Extra: Haz que el emoji gire 360 grados cada vez que se pasa el ratón por encima.
> Extra: Haz que el emoji suba 100px cada vez que se hace click sobre el mismo.

### Input dinámico

En esta sección vamos a crear un input que muestre el texto que el usuario escribe en el mismo.

1. Crea una seccion con un h2 y un input centrados.
2. Haz que el h2 muestre el texto que se escribe en el input.
3. Asegúrate de mostrar el texto "Escribe en el input" en tu elemento h2 cuando no haya nada escrito en el input.

🚨 ¡Listo! Avisa y espera al resto de compañeros.

> Extra: Haz que el texto tome un color aleatorio cada vez que el usuario escribe en el input.

### Color switch

En esta sección vamos a crear un div sin contenido, que mostrara el color de fondo que el usuario elija.
El usuario podrá utilizar tres deslizadores para elegir el color de fondo del div utilizando el modelo RGB.

1. Crea una seccion con un div y tres inputs de tipo range dentro, centra los elementos.
2. Asegúrate de que los inputs solo aceptan valores entre 0 y 255, y que se inicien a 0.
3. Haz que cada input controle un valor de color (rojo, verde y azul) de fondo del div.

🚨 ¡Listo! Avisa y espera al resto de compañeros.

### CSS Gradient

Esta sección es muy similar a la anterior, pero en lugar de elegir un color, vamos a crear un degradado y generar el código CSS necesario para utilizarlo.

Cuando queremos hacer degradados en CSS, podemos utilizar la propiedad `background` y el valor `linear-gradient`, este valor acepta como parámetros el ángulo del degradado y los colores que queremos utilizar, por ejemplo:

```css
background: linear-gradient(90deg, red, rgb(0, 255, 0));
```

1. Crea otra sección con un div centrado.
2. Añade un grupo de tres inputs de tipo range, cada uno controla un valor (RGB) del primer color del degradado del div.
3. Añade otro grupo de tres inputs de tipo range, cada uno controla un valor (RGB) del segundo color del degradado del div.
4. Muestra el degradado en el div correspondiente.
5. Añade un h2 al final de la sección.
6. Muestra el código CSS necesario para utilizar el degradado en el h2.



