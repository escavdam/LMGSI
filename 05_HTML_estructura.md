# Origen
Previamente a la aparición de HTML, la información de las páginas web se almacenaba en ficheros de texto plano. Estos ficheros contenían texto y comandos que indicaban cómo debía mostrarse el texto (negrita, cursiva, etc.). El problema de este sistema es que no se podían incluir imágenes, sonidos, vídeos, etc. Además, cada navegador interpretaba los comandos de una forma diferente, por lo que una misma página se veía de forma distinta en cada navegador.

HTML fue creado en 1990 por Tim Berners-Lee, un científico del CERN (Organización Europea para la Investigación Nuclear). HTML es un lenguaje de marcas, es decir, un lenguaje que permite describir la estructura y el contenido de un documento. HTML no es un lenguaje de programación, es un lenguaje de marcas que define la estructura de una página web.

Una de las características de HTML es que permite incluir en un documento texto, imágenes, sonidos, vídeos, etc. Además, HTML permite definir la estructura de una página web, es decir, permite definir qué es un título, un párrafo, una lista, etc. HTML no define cómo se deben mostrar estos elementos, sino que indica qué significado tienen. Por ejemplo, HTML permite definir que un texto es un título, pero no indica cómo se debe mostrar ese título (con un tamaño de letra mayor, en negrita, etc.). La apariencia de los elementos se define mediante hojas de estilo.

[El primer website creado](http://info.cern.ch/hypertext/WWW/TheProject.html)

# Estructura de un elemento HTML
Un elemento HTML está formado por una etiqueta de apertura, el contenido del elemento y una etiqueta de cierre, diferenciada por una barra inclinada (/).

```html
<tag> contenido </tag>
```

En muchos casos, las etiquetas de apertura y cierre pueden tener atributos, que se utilizan para modificar el comportamiento de la etiqueta. Los atributos se escriben dentro de la etiqueta de apertura, y tienen la forma nombre=valor. Los atributos se separan entre sí por un espacio en blanco.

```html
<tag atributo1=valor1 atributo2=valor2> contenido </tag>
```

En muchos casos, utilizaremos etiquetas anidadas, es decir, una etiqueta dentro de otra. En este caso, la etiqueta anidada se escribe entre la etiqueta de apertura y la de cierre de la etiqueta que la contiene.

```html
<div> 
    <p> contenido </p> 
</div>
```

# Estructura de un documento HTML
Un documento HTML con `<!DOCTYPE html>` indica que el documento es un documento HTML5, este tag . A continuación, se incluye la etiqueta `<html>`, que indica que el documento es un documento HTML. El contenido del documento se incluye entre las etiquetas `<html>` y `</html>`.

El contenido del documento se divide en dos partes: la cabecera y el cuerpo. La cabecera se incluye entre las etiquetas `<head>` y `</head>`, y contiene información sobre el documento y nuestra web. 
El cuerpo se incluye entre las etiquetas `<body>` y `</body>`, y es donde realmente creamos nuestros elementos que mostraremos en nuestro documento.

```html
<!DOCTYPE html>
<html>
    <head>
        <title> Título del documento </title>
    </head>
    <body>
        Contenido del documento
    </body>
</html>
```
[Mas sobre el DOCTYPE](https://developer.mozilla.org/es/docs/Glossary/Doctype)