# Marp
Marp es una herramienta que permite crear presentaciones a partir de archivos Markdown.

## Crear archivos marp
Para crear una presentación con marp, creamos un archivo con extensión .md, .markdown o .mdown.

## Sintaxis básica
La sintaxis de marp es igual que la de markdown, aunque aqui puede ser mas util usar etiquetas HTML para dar formato a la presentación y añadir otros elementos como imágenes, videos, etc.

Para iniciar una presentación, debemos añadir la etiqueta `---` al inicio del archivo, seguido de la linea `marp: true` para indicar que el archivo es una presentación.

Cada diapositiva debe ir separada por tres guiones `---`.

```markdown
---
marp: true
---

# Mi primera diapositiva

---

```
