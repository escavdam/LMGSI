# Markdown

Markdown es un lenguaje de marcado ligero creado en 2004, y que se utiliza para dar formato a un texto plano. Es un lenguaje de marcado minimalista, que se centra en la legibilidad y la facilidad de uso. Muy usado entre desarrolladores de cualquier tipo, ya que nos permite escribir documentación, blogs y contenido para páginas web rápidamente.

# Crear archivos markdown

Para crear archivos en markdown no es necesario ningún editor especial, podemos crearlos con cualquier editor de texto plano.
Solo debemos crear un archivo con la extensión .md, .markdown o .mdown.

---
# Sintáxis
## Encabezados
Utilizamos el símbolo # para crear encabezados, podemos crear encabezados de diferentes niveles, dependiendo del número de # que utilicemos.

```markdown
# Esto es un titular de nivel 1
## Esto es un titular de nivel 2
### Esto es un titular de nivel 3
```
---
## Texto y énfasis
Esto es un párrafo, podemos escribir texto plano, tambien destacar texto usando `*cursiva*` o `**negrita**`.

---
## Listas

Crear listas ordenadas es fácil:
```markdown
1. Elemento 1
    1.1 Elemento 1.1
    1.2 Elemento 1.2
    1.3 Elemento 1.3
2. Elemento 2
3. Elemento 3
    3.1 Elemento 3.1
    3.2 Elemento 3.2
4. Elemento 4
5. Elemento 5

Tambien podemos crear listas desordenadas:
- Elemento 1
- Elemento 2
- Elemento 3
    - Elemento 3.1
    - Elemento 3.2
    - Elemento 3.3
- Elemento 4
- Elemento 5
```
---

## Links
Podemos crear links a otras páginas web, o a otros archivos markdown.

[Enlace a Google](https://www.google.es)

[Enlace a otro archivo markdown](./01_Mermaid.md)

[Enlace a una seccion de este mardown](#sintáxis)

## Imagenes
Podemos añadir imágenes de la siguiente forma

`![alt text](url_imagen)`

**Recordad!** Es muy importante añadir un alt text a nuestras imagenes en archivos de marcado, este texto se mostrará en caso de que la imagen no se pueda cargar, esto nos puede beneficiar a la hora de encontrar errores, mejorará nuestro posicionamiento SEO y nos ayudará a que nuestra página sea accesible a personas con problemas de visión.

---

## Código
Muchas veces necesitaremos incorporar código de diferentes lenguajes a nuestros archivos md, para ello podemos usar comillas invertidas triples:

```markdown
# Esto es un ejemplo de código en markdown
```

```html
<!-- Esto es un ejemplo de código en html -->
<h1>Esto es un ejemplo de código en html</h1>
```

```css
/* Esto es un ejemplo de código en css */
body{
    background-color: red;
}
```

```javascript
// Esto es un ejemplo de código en javascript
function saludo(name){
    console.log(`Hola ${name}`);
}
saludo("Antonio")
```

```python
def saludo(name):
    print(f"Hola {name}")
saludo("Antonio")
```

```java
public class Saludo{
    public static void main(String[] args){
        System.out.println("Hola mundo");
    }
}
```

```bash
# Esto es un ejemplo de código en bash
echo "Hola mundo"
```

```sql
-- Esto es un ejemplo de código en sql
SELECT * FROM users;
```

```mermaid
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
```

```c#
// Esto es un ejemplo de código en c#
public class Saludo{
    public static void Main(string[] args){
        Console.WriteLine("Hola mundo");
    }
}
```

Es importante que marqueis que lenguaje es el utilizado en el bloque de código, ya que afecta a la hora de renderizar diferentes aspectos del mismo.

También podemos añadir código inline, utilizando una sola comilla invertida `val = 5`

---

## Tablas
Podemos crear tablas de la siguiente forma:

| User | Password | Email | Role |
| ---- | -------- | ----- | ---- |
| Admin | 123456 | admin@gmail.com | Admin |
| user12309 | qwerty | user12309@gmail.com | User |
| user12310 | asdfgh | user12310@yahoo.com | User |
| user12311 | zxcvbn | user12311@gmail.com | Moderator |

---

## Citas
Podemos crear citas de la siguiente forma:

> Aliqua minim consectetur fugiat aliqua sint ex consequat incididunt ullamco aute. Anim cillum mollit exercitation ipsum nisi in fugiat irure eiusmod consectetur labore velit qui. Id consectetur dolor deserunt non id culpa officia mollit minim nulla adipisicing sint officia nostrud.

---

## Lineas horizontales
Para insertar un separador en forma de linea horizontal, podemos usar tres guiones medios `---`

---

## Caracteres de escape

Para poder escribir caracteres que tienen un significado especial en markdown, podemos usar el caracter de escape `\`

\# Esto no es un encabezado

\> Esto no es una cita

\- Esto no es un elemento de una lista