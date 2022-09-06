# HTML
## ETIQUETAS: <a href="https://htmlreference.io "> Guia Aqui </a>
```HTML
<img alt >: alt= atributo para poner una segunda opcion por si no se realiza la funcion primaria
<b>: Pone tu texto en negritas (pero esta etiqueta NO tiene sentido semántico).
<strong>: También pone tu texto en negrita, pero esta SÍ tiene sentido semántico (Google le da relevancia al texto que pongas ahí).
<i>: Pone tu texto en cursivas (pero esta etiqueta NO tiene sentido semántico).
<em>: También pone tu texto en cursivas, pero esta SÍ tiene sentido semántico (Google le da relevancia al texto que pongas ahí).
<br>: Hace un salto de línea, funciona como si diéramos un enter con el teclado 😄.
<a>: Enlaces
<h1-h6>: Textos Segun tamaño siendo 1 importante y 6 menso importante
<p>: parrafos
<span>: ayuda escribit dentro de textos palabras estlizadas
<form>: formularios
<ul> <li> <ol>: listas

```



## Proceso de renderizado del motor del navegador
El motor del navegador realiza 5 pasos o procesos para compilar nuestro código hasta el renderizado por pantalla. Estos pasos son los siguientes:

Transforma los archivos a un árbol de objetos HTML o CSS, estos se denominan DOM (Document Object Model) y CSSDOM (Cascade Style Sheet Object Model), respectivamente. Cada nodo en el árbol es una representación de los elementos que contiene el archivo HTML o CSS.
Calcula el estilo correspondiente a cada nodo del DOM relacionado al CSSDOM.
Calcula las dimensiones de cada nodo y dónde va en la pantalla.
Pinta o renderiza los diferentes elementos como cajas o contenedores.
Agrupa todas las cajas en diferentes capas para convertirlas en una imagen que se renderiza en pantalla.

## Los 5 pasos de los motores:

1. Pasa los archivos de HTML a objetos (El DOM). Esto para que el navegador pueda entenderlo.
2. Calcula el estilo correspondiente a cada nodo en el DOM.
3. Calcula las dimensiones de cada nodo y va a empezar a estructurar la página web.
4. Pinta las diferentes cajas.
5. Toma las capas y las convierte en una imagen, para finalmente mostrar esta imagen en la pantalla.
 
## ¿Cuáles son los elementos HTML?
Los elementos son cada una de las partes que conforman un archivo HTML. Su estructura contiene:

Etiquetas: es la representación de un elemento HTML. Se dividen en etiquetas de apertura, representadas por `<etiqueta>` y etiquetas de cierre, representadas por `</etiqueta>`.
Contenido: es el texto o elementos encerrados por la etiqueta, este valor es opcional en algunas de ellas.

## Qué son atributos HTML
Los atributos HTML son propiedades en la etiqueta de apertura que manejan el comportamiento del elemento. Su valor está envuelto en comillas.

## Qué son los elementos vacíos
Los elementos vacíos son aquellos que únicamente se representan en una etiqueta de apertura. Por ejemplo, la etiqueta de imagen: `<img...>.`
Estas etiquetas pueden cerrarse en la misma etiqueta de apertura, utilizando la barra inclinada “/” al final: `<img.../>`,

## Qué es el anidamiento de elementos
El anidamiento de elementos HTML consiste en envolver varias etiquetas en otras etiquetas.
Interpreta a cada elemento HTML como una caja donde puedes guardar diferentes elementos u otras cajas. Estas cajas tendrán diferentes tamaños y estarán colocadas junto a otras.
Aquellas etiquetas que envuelven a otras se las denomina “padres”. Es decir, `<section>` es padre de `<h1>`, `<p>`, `<ul>`, y a su vez `<ul>` es padre de 3 etiquetas `<li>`.
Las etiquetas que son el contenido de otras, se las denomina “hijos”. Es decir, las etiquetas `<h1>`, `<p>`, `<ul>` son hijos de `<section>`, y a su vez las etiquetas `<li>` son hijos de `<ul>`.

## Estructura básica de un documento HTML:
```HTML
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    
</body>
</html>

```
Etiqueta Doctype
La etiqueta `<!DOCTYPE html>` especifica que el archivo se maneje con la versión 5 de HTML.

### Etiqueta html
La etiqueta `<html>` define el elemento raíz de un documento HTML. Todos los demás elementos deben estar contenidos dentro de este elemento raíz. En esta etiqueta se especifica el lenguaje de la página web mediante la propiedad lang.

### Etiqueta head
La etiqueta `<head>` define la metainformación, es decir, toda información que no es contenido como tal de la página web. Por ejemplo, los enlaces a archivos CSS y JavaScript, el título y la imagen que aparecen en la pestaña del navegador. Esto es importante para motores de búsqueda como Google.

### Etiqueta body
La etiqueta `<body>` define el contenido de la página web. Debe ser hijo cercano de `<html>` y padre de todas las etiquetas HTML, excepto por aquellas que definan metainformación.

### Comentarios de HTML
Los comentarios de HTML consiste en señalar algo que se ignorará. Para establecer un comentario HTML se lo envuelve entre `<!-- y -->`, independiente de la cantidad de líneas.
```HTML
<!-- Este es un comentario de una línea -->
<!--
Este es un comentario de varias líneas
-->
```

## HTML SEMÁNTICO
`<div>`

Nos indica Propiedades adecuadas para cada una de las cosas, el codigo sea mas claro, ayuda a ser accesible.


# CSS
Una declaración de CSS es un bloque que especifica el conjunto de estilos que se añadirán a un elemento HTML. Su estructura contiene lo siguiente:

1. Selector: define el elemento o conjunto de elementos a los cuales se añadirán los estilos.
2. Propiedad: es el nombre del estilo de CSS.
3. Valor: es el valor que tomará la propiedad.

## Propiedades iniciales de CSS
Antes de empezar con CSS utilizaremos algunas propiedades de CSS.

**color:** establece el color del texto de un elemento.
**background-color:** establece un color de fondo al elemento.
**font-size:** establece el tamaño de la fuente.
**width:** establece la anchura de un elemento.
**height:** establece la altura de un elemento.

## TIPOS DE SELECTORES
### Selector de Tipo
Selecciona todos los elementos que coincidan con el nombre de la etiqueta HTML.

```CSS
div {
    /* Todos los div en el documento */
}
```
### Selector de clase
Selecciona todos los elementos que coincidan con las etiquetas HTML que contengan el atributo class.
```CSS
<!--archivo HTML-->
<div class="card"> Soy una carta </div>
```