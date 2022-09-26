<h1>HTML Y CSS  <a href="https://github.com/NoBody-UU/FrontEndBasic">Repositorio</a> </h1>
<h3>By:NoBody-Huber</h3>
<p>Esto es una pequeña guia acerca de html y css, espero te sirva, cualquier duda, aporte o lo que sea dc: NoBody#9666</p>

# HTML
## ETIQUETAS: <a href="https://htmlreference.io "> Guia Aqui </a>
```HTML
<img alt >: alt= atributo para poner una segunda opcion por si no se realiza la funcion primaria
<b>: Pone tu texto en negritas (pero esta etiqueta NO tiene sentido semántico).
<strong>: También pone tu texto en negrita, pero esta SÍ tiene sentido semántico (Google le da relevancia al texto que pongas ahí).
<i>: Pone tu texto en cursivas (pero esta etiqueta NO tiene sentido semántico).
<em>: También pone tu texto en cursivas, pero esta SÍ tiene sentido semántico (Google le da relevancia al texto que pongas ahí).
<br>: Hace un salto de línea, funciona como si diéramos un enter con el teclado .
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


# CSS <a href="https://htmlcolorcodes.com/es/">COLORES HTML</a>
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

/* archivo CSS */
.card {
    /* Todas las etiquetas con la clase "card" */
}
```
### Selector de identificador único (id)
Selecciona el único elemento que coincida con la etiqueta HTML que contenga el atributo id. Solo puede existir un valor id para todo el documento.Para seleccionar el elemento, se empieza por el símbolo de hashtag `#` y seguido el valor exacto del atributo `id` de la etiqueta. Puede ser cualquier valor que desees colocar.
```CSS
<!--archivo HTML-->
<button id="eliminar"> Eliminar  </button>

/* archivo CSS */
#eliminar {
    /* La única etiqueta con el id "eliminar" */
}
```
### Selector de atributo
Selecciona los elementos que coincidan con la etiqueta HTML que contenga el atributo y valor especificado.
```html
<!--archivo HTML-->
<a href="https://platzi.com"> Ir a Platzi </a>
```
Para seleccionar los elementos, se empieza por el nombre de la etiqueta, seguido de corchetes [] que contiene el atributo y valor especificado.
```css
/* archivo CSS */
a[href="url"] {
    /* Todas las etiquetas <a> con una propiedad href con valor "https://platzi.com" */
}
```
### Selector universal
Selecciona todos los elementos del documento mediante un asterisco *.
```CSS
* {
    /* Todos los elementos */
}```

### selectores combinadores
Un selector combinador es la unión de dos o más selectores básicos.
```css
selector1 selector2 selector3 {
    /* Estilos */
}
```
#### 1. Combinador de descendientes
Selecciona todos los elementos del selector de la derecha que son hijos del selector de la izquierda, independientemente de la profundidad. Estos selectores están separados por un espacio.
```css
padre hijos {
    /* Todos los hijos del padre */
}

div p{
    /* Todos los hijos <p> de <div>*/
}

.container img{
    /* Todos los hijos <img> de la clase "container"*/
}
```
#### 2. Combinador de hijo directo
Selecciona todos los elementos del selector de la derecha que son hijos directos del selector de la izquierda. Estos selectores están separados por `>`.
```css
padre > hijos_directos {
    /* Todos los hijos directos del padre */
}

div > p{
    /* Todos los hijos directos <p> de <div>*/
}

.container > img{
    /* Todos los hijos directos <img> de la clase "container"*/
}
```
#### 3. Combinador de elemento adyacente
Selecciona todos los elementos del selector de la derecha que están adyacente al selector de la izquierda. Estos selectores están separados por `+`.
```css
elemento + adyacente {
    /* Elementos adyacentes */
}

div + p{
    /* Todos los <p> adyacentes a <div>*/
}

.container + img{
    /* Todos los <img> adyacentes a la clase "container"*/
}
```
Adyacente significa que comparten el mismo padre y está situado inmediatamente hacia abajo de otro elemento. Por ejemplo, en el siguiente código, `<div>` está adyacente a `<h1>` y `<p>` está adyacente a `<div>.` Sin embargo, `<h1>` no está adyacente a `<div>` y `<div>` no está adyacente a `<p>`.
```html
<!--archivo HTML -->
<h1>Soy un título </h1>
<div>Soy un div</div>
<p>Soy un párrafo</p>
```
#### 4. Combinador general de hermanos
Selecciona todos los elementos del selector de la derecha que son hermanos del selector de la izquierda. Estos selectores están separados por `~`.
Hermanos significa que comparten el mismo padre y están situados hacia abajo de otro elemento. Por ejemplo, en el siguiente código, <div> y `<p>` son hermanos de `<h1>`, pero `<h1>` no es hermano de `<div>` y `<p>`.


## Tipos de selectores: pseudoclases y pseudoelementos
### Pseudoclases
Una pseudoclase define el estilo de un estado especial de un elemento.También podemos ver a las pseudoclases como estados de algún elemento (con el mouse encima, visitado, activo, etc.)

<a href="https://developer.mozilla.org/es/docs/Web/CSS/Pseudo-classes#indice_de_las_pseudo-clases_est%C3%A1ndar">Índice de pseudo-clases estándar.</a>

#### Sintaxis:

```css
selector : pseudoclase { 
    propiedad: valor;
}
```
### Pseudoselementos
Un pseudoelemento define el estilo de una parte específica de un elemento, elementos que escribimos desde CSS, por ejemplo, el `::after` y el `::before` nos puedes funcionar como divs, como su nombre lo dice, son elementos, pero no necesariamente están escritos desde el HTML 

<a href="https://developer.mozilla.org/es/docs/web/css/pseudo-elements#lista_de_pseudoelementos">Lista de pseudo-elementos.</a>

#### Sintaxis

```css
selector :: pseudo-elemento { 
    propiedad: valor;
}
```

## Cascada y especificidad en CSS
### la cascada en CSS
La cascada es el concepto que determina qué estilos se colocan sobre otros, priorizando a aquellos que se encuentren más abajo del código. Recordarás que CSS es la abreviación de Cascade Style Sheets, que traducido es hojas de estilos en Cascada.
Mira el siguiente código e identifica de qué color de letra tendrá la etiqueta `<h1>`.
```css
h1 {
    color: red;
}

h1 {
    color: blue;
}
```
La etiqueta `<h1>` tendrá un color `blue` de letra, esto porque está situado más abajo en el código. Esto ocurre con cada propiedad de CSS que se repita en algún punto más arriba del código.

### Especificidad en CSS
La especificidad consiste en dar un valor a una regla CSS sobre qué tan específico es el estilo, esto para que los navegadores puedan saber qué estilos aplicar sobre otros, independientemente de dónde se encuentren en el código. El estilo se aplicará donde la especificidad sea mayor.
La palabra reservada !important es un valor de toda propiedad CSS que provee una especificidad de 10000, por lo que se aplicará ante otros estilos. Esto es una mala práctica y no deberías utilizarlo.
```css
h1 {
  color: red;
}

h1 {
  color: green !important; //ESTE SERA EL COLOR A MOSTRAR
}

h1 {
  color: blue;
}

h1 {
  color: papayawhip;
}
```
