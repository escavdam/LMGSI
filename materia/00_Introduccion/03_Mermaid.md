# Mermaid
Mermaid es una herramienta para crear diagramas de flujo utilizando un lenguaje de marcado de texto.
Nos puede ayudar durante el desarrollo de software para documentar procesos, pero también para cualquier otro tipo de estructura que queramos representar.

```mermaid	
flowchart LR
    A[Inicio] --> B[Proceso 1]
    B --> C[Proceso 2]
    C --> D[Proceso 3]
    D --> E[Fin]
    E --> A
```
# Sintaxis
La sintaxis de Mermaid es muy sencilla, se basa en el uso de palabras clave para definir los elementos del diagrama y los conectores entre ellos.

Podemos utilizar mermaid en cualquier archivo con extension .md, .markdown o .mdown.

La cabecera de cualquier diagrama comienza con la palabra clave `flowchart`, a continuación podemos definir la dirección del diagrama, `LR` (left to right), `RL` (right to left), `TB` (top to bottom) o `BT` (bottom to top).

**RECUERDA** que markdown no puede interpretar el código de mermaid por si mismo, sin embargo, dependiendo de nuestro editor, podemos encontrar plugins que nos permitan renderizar el diagrama en tiempo real.

---
# Crear nodos
Para crear un nodo nos basta con escribirlo, a ese elemento se le conoce como id.
    
```mermaid
flowchart LR
    A
    B
    C
```

Por defecto, mermaid utiliza el texto del id para renderizar el nodo, pero podemos cambiarlo utilizando la siguiente sintaxis:

```mermaid
flowchart LR
  A
  B[Esto es otro nodo, pero con un texto diferente al id]
  C[Podeis utilizar
  saltos de linea]
```

---
# Conectar elementos
## Conexion abierta

Utilizamos `---` para conectar dos elementos:
    
```mermaid
flowchart LR
  A---B
```

## Conexion cerrada

Utilizamos `-->` para conectar dos elementos:
    
```mermaid
flowchart LR
  A-->B
```
---
# Forma de los nodos
Mermaid dispone de varios tipos de nodos, podemos utilizarlos para diferenciar entre acciones, decisiones, etc.
Para usarlos, debemos envolver nuestro texto entre diferentes caracteres o combinacion de estos, siendo "[]", "()" y "{}" los más utilizados.

```mermaid
flowchart TD
    A[Rectangular]
    B(Redondeado)
    C{Decision}
    D((Circular))
    E[(Cilindro)]
    F[[Subrutina]]
    G>Asimetrico]
    H{{Hexagono}}
    I[/Paralelogramo/]
```

---

