# Curso de HTML y CSS - Inicio 19/06/2025

En este curso aprenderé:

Los fundamentos de HTML moderno y semántico.

CSS y diseños de interfaces, flex-box y CSS Grid.

También como utilizar componentes y patrones de diseño.

Diseño responsivo para que se puede visualizar en cualquier dispositivo de distinto tamaño de pantalla.

También aprenderé a como utilizar los 7 pasos de la creación de una web profesional

- Planificación
- Boceto
- Diseño
- Construcción
- Prueba
- Optimización
- Lanzamiento

Como encontrar recursos gratuitos como imágenes, fuentes e iconos.

Leer documentación, corregir errores y usar herramientas de desarrollo web.

También se realizarán muchos proyectos.

Nota: Todas lo escrito en este README será escrito por mi, lo que quiero decir es que no habrá copia y pega de conceptos, solo anotaciones mías.

---

## Una descripción general de alto nivel del desarrollo web

Cuando visitamos una página, el navegador realiza una petición en la dirección de la web (la URL), el servidor recibe esta petición y le da una respuesta, esta respuesta contiene los archivos necesarios para que el navegador pueda mostrar la página, archivos como index.html, styles.css, script.js e incluso imágenes de ser necesario. El navegador se encarga de leer los archivos recibidos y empezar a mostrar (renderizar) la página web.

Los únicos lenguajes que puede entender el navegador web son Html, CSS y JavaScript

La parte del Front-end la componen los tres lenguajes principales HTML, CSS y JavaScript.

Una página web estática significa que el servidor manda los archivos tal y como son, sin cambios en su información.

Una página web dinámica es aquella que sus datos o información mostrada está en constante cambio, como los e-commerce, los sitios dinámicos suelen tener una Back-End desarrollado para poder transformar la página, utiliza un lenguaje para back-end y una base de datos donde se almacena los datos. La información cambia según los datos que contenga la base de datos.

Los 3 cores de una página web:

- HTML -> Se encarga de tener todo el contenido, sean imágenes, textos, botones, listas, videos, etc.
- CSS -> Su tarea es de darle presentación, estilizar los elementos del contenido html.
- JavaScript -> Es para agregar interactividad, dinamismo, animaciones a la web.

<br>
<br>
<br>

# Fundamentos de HTML

## ¿Qué es HTML?

Html es un lenguaje de marcado, sus siglas significan Hyper Text Markup Language (Lenguaje de marcado de hyper texto), es uno de los lenguajes principales de la web, el navegador no entiende otro lenguaje que no sea html para estructurar y describir contenido.

Html tiene muchos elementos para lo que es describir contenido, texto, imágenes, párrafos, enlaces, títulos, videos, etc.

### Anatomía de un elemento HTML

![Anatomía de un elemento html](/images-readme/anatomy-element-html.png)

- Abertura de un elemento -> Nombre del elemento que usaremos
- Contenido -> En caso de la imagen es texto, pero también puede ser un elemento hijo.
- Cierre de un elemento -> Similar a la abertura pero con "/", en algunos elementos se omite.

## Estructura de un documento HTML

Podemos crear archivos html con la extension .html:

index.html

La página principal de la web siempre será el archivo index.html

La estructura principal de un documento HTML se compone de 4 elementos.

```
<!DOCTYPE html>
<html>
<head> </head>
<body> </body>
</html>
```

Toda estructura de un documento html debe empezar con DOCTYPE html y `<html>`

El `<head>` sirve para configurar la página web y describir el sitio web, como el título, agregar descripción, configurar el viewport, conectarla a recursos externos.

El `<body>` es el contenedor que servirá para mostrar los elementos en pantalla, todo lo que se verá estará dentro de body.

## Elementos de Texto

Elementos de tipo texto son:

- `<h1> - <h6>` -> Son encabezados, títulos que nos sirven para diferenciar secciones según jerarquía, donde h1 es el mas importante y debe ser el único titulo principal.
- `<p>` -> Sirve para encerrar un párrafo, texto simple.
- `<strong>` -> Convierte en negrita el texto, usando semántica, el texto tendrá significado para el navegador.
- `<em>` -> Da énfasis al texto, también usa semántica para dar significado.

## Listas

Las etiquetas que conforman una lista son 3: <b>ol</b>, <b>ul</b>, <b>li</b>.

Elementos tipo lista:

- `<ol>` -> Se utiliza para crear listas ordenadas, que son secuenciales, su semántica es presentar el texto de forma consecutiva, respetando el orden de los elementos.

- `<ul>` -> Se usa para listas que no son necesariamente ordenadas.

- `<li>` -> Van dentro de <b>ol</b> y <b>ul</b>, es como el item de la lista.

## Imágenes y atributos

Las imágenes se colocan con la etiqueta <b>`<img>`</b> utilizando el atributo <b>src</b> para darle el path/ruta del archivo y también se usa el atributo <b>alt</b> para que la imagen tenga una descripción, los dos atributos son obligatorios en la etiqueta <b>img</b>.

Ejemplo de código:

`<img  src="ruta/imagen.jpg" alt="texto descriptivo de la imagen" />`

### ¿Pero qué son los atributos?

Los atributos son modificadores que se añaden a las etiquetas para proporcionar información adicional, personalizar su comportamiento o definir características especificas. Ejemplo:

`<etiqueta atributo="valor">Contenido</etiqueta>`

De esta forma podemos decirle a la etiqueta tag `<img>` mediante los atributos la imagen que va a mostrar y su texto descriptivo.

## Enlaces

Los enlaces sirve para poder navegar entre páginas web, descargar videos, enviar correos o saltar entre secciones de una página web.

Para crear un enlace se utiliza la etiqueta `<a>` y el atributo <b>href</b>.

Ejemplo:
`<a href="https://www.ejemplo.com">Visitar Ejemplo</a>`

## Estructura de una página

Existen etiquetas que son para estructurar el contenido, mientras otras son para definir, hay etiquetas que nos dicen que parte hará en la página web.

Tenemos etiquetas como:

- `<header>` -> No confundir con la etiqueta `<head>`, este elemento indica que elementos son del encabezado de una página o un articulo.
- `<nav>` -> Lista los enlaces con los que se navegara por el sitio web.
- `<article>` -> Engloba contenido extra, que no tiene nada que ver con el contenido de la página actual.
- `<footer>` -> Es el pié de página, se coloca información adicional como contacto, redes, enlaces legales.

<br>
<br>

# ¿Qué es la semántica?

La semántica es el significado que tiene cada elemento, algunas representan imágenes, otro texto, listas, títulos, notas, direcciones, etc.

Es importante para el SEO en los motores de búsqueda, la accesibilidad para las personas que tienen alguna discapacidad visual.

<b>Es obligatorio cumplir con este concepto.</b>

<br>
<br>
<br>

# Fundamentos de CSS

## ¿Qué es CSS?

CSS es un lenguaje en cascada de estilos (Cascade Style Sheets), se encarga de dar estilos a los elementos html. Mientras que HTML crea el contenido que tendrá el sitio web, CSS proporciona el diseño, colores, tamaños, etc.

![Regla CSS - Anatomia](/images-readme/css_rule.png)

```
h1 {
  color: blue;
  text-align: center;
  font-size: 20px
}
```

## En linea, interno y css externo

Hay 3 formas de añadir CSS al documento HTML.

- En linea -> Se agrega directamente en el elemento html.

  `<p style="color: red">Hola mundo</p>`

- En el head y `<style>` -> En el `<head>` agregas la etiqueta `<style>` y escribir css ahi dentro usando selectores.

  ```
  <head>
    <style>
      h1 {
        color: blue;
      }
    </style>
  </head>
  ```

- En un archivo externo -> Creamos una archivo CSS (style.css) donde irá el código y lo enlazamos al html utilizando la etiqueta `<link>` dentro del `<head>`.

  ```
  <head>
  <link role="stylesheets" href="/ruta/style.css">
  </head>
  ```

Nota: <b>Recomendable siempre utilizar el método del archivo externo.</b>

## Estilizando texto

Para estilizar texto tenemos propiedades como:

- font-size
- font-family
- font-weight
- line-height
- text-transform
- color
- letter-spacing
- text-align

## Combinando selectores

Podemos selecciona el elemento directamente con el nombre de etiqueta pero lo malo es que seleccionará todos los elementos que tengan el mismo nombre, por ejemplo `<h2>`.

Para combinar selectores y especificar uno podemos descender

```
HTML
<article>
  <header>
    <h2>Hola</h2>
  </header>
</article>

CSS
article header h2 {
  color: red;
}
```

Combinamos los selectores para aplicar estilos a un elemento en especifico.

  <br>

## Selectores de clase y id

Tenemos dos tipos de selectores aparte de el selector de elementos.

- Selector clases -> Se aplica utilizando el atributo `class=""` en el elemento HTML, se puede reutilizar muchas veces y en varios elementos.

- Selector de id's -> Se aplica utilizando el atributo `id=""` en el elemento, no se usa para selector de css y si se usa solo puede haber un **id** con el mismo nombre en todo el documento html.

## Colores

Podemos utilizar colores con la notación RGB o Hexadecimales, los colores cubre rojo, verde y azul.

La notación RGB combina los colores de esta forma

`rgb(255, 255, 255, 0.5)` -> cada **255** representa un color, están en el orden rojo, verde y azul, donde va de 0 a 255, mínimo y máximo. El ultimo valor representa la transparencia que tendrá el color,

En la notación hexadecimal funciona de la misma forma

`#ffffff` -> son 6 caracteres, dos caracteres representan un color y van en el mismo orden, **ff** vendría a ser como **255** y **00** como 0.

Usualmente se utiliza la notación hexadecimal para colores comunes y RGBA para colores con transparencia.

## Pseudo-clases

Las pseudo-clases son una palabra clave que usan los selectores para definir un estado especial de un elemento.

```
p:first-child {
  color: red;
}
```

La pseudo-clase se aplica después del selector con `:pseudo-clase`, en el ejemplo se captura al elemento que sea el primer hijo.

Existe muchas pseudo-clases, en el glosario de pseudo-clases estará las que se mencionaron en el curso.

## Pseudo-clases en hipervínculos - Estilizando enlaces

Estilizar los hipervínculos se hace con pseudo-clases, identificando todos sus estados.

```
- Selecciona al enlace con atributo href
a:link {
  color: #1098ad;
  text-decoration: none;
}

- Aplica al sitio web visitado
a:visited {
  color: #1098ad;
}

- Cuando el puntero del mouse esta encima aplica estilos
a:hover {
  color: orangered;
  font-weight: bold;
  text-decoration: underline dotted orangered;
}

- Cuando se clickea al elemento aplica los estilos
a:active {
  background-color: black;
  font-style: italic;
}
```

## Chrome DevTools

Es una herramienta que nos brinda el navegador para poder visualizar el código de la página, tanto el html, el css y algunas cosas más.

![Chrome DevTools](/images-readme/chrome-dev-tools.png)

Podemos realizar configuraciones, testear, etc.

## Teoría de CSS: Conflicto entre selectores

Existe la posibilidad en la que varios selectores apunten a un mismo elementos, aplicando mismas propiedades de estilo pero con diferente, ahi salta la duda de que declaración css se está aplicando.

Pero en sí se aplican todas, lo que pasa después es quien toma la prioridad de selector y aplica el estilo final.

Son 6 niveles de prioridad.

- Nivel 5 -> Declaraciones marcadas con !important
- Nivel 4 -> Estilos en linea (en el elemento html)
- Nivel 3 -> Selectores de ID
- Nivel 2 -> Selectores de Clase o Pseudo-clases
- Nivel 1 -> Selector de elemento (p, div, li, etc)
- Nivel 0 -> Selector universal (\*)

Van de la más alta prioridad Nivel 5 a la mas baja Nivel 0.

En caso de que haya muchos selectores de un mismo nivel entonces se aplica el que esta escrito al último o final del código.

## Teoría de CSS: Herencia y el selector universal

La herencia funciona aplicando estilos al contenedor, como propiedades de tipo texto y entonces esta hereda a los elementos de tipo texto.

El selector universal selecciona a todos los elementos y aplica los estilos a todos los elementos, no aplica herencia en si.

```
* {
  color: red;
}
```

## Teoría de CSS: El modelo de caja de CSS

El modelo de caja es el espacio que ocupará el elemento en total:

Tenemos 4 espacios en un elemento:

- Contenido -> Es el contenido en sí mismo.
- Padding -> Es el relleno invisible que está alrededor del contenido.
- Border -> El borde que lo rodea.
- Margin -> Espacio que lo aparta de los otros elementos.

Por default el ancho es la suma de: borde izquierdo + relleno izquierdo + contenido + padding derecho + border derecho

La altura por default es: Borde superior + Padding superior + contenido + padding inferior + borde inferior.

## Usando margenes y paddings

Para crear espacio entre elementos podemos usar **margenes**, tenemos propiedades como:

- margin-bottom
- margin-top
- margin-left
- margin-right

Cuando dos margenes se encuentran, existe el colapso de margenes, entonces el margen que ocupa mas espacio predomina y elimina al menor, como si el menor no contara.

El uso de paddings se añade para crear un relleno en el elemento, esta entre el espacio total y el espacio de contenido. De la misma manera tenemos propiedades como:

- padding-top
- padding-bottom
- padding-left
- padding-right

Para crear espacio entre elementos siempre usar margenes.

## Añadiendo dimensiones

Podemos añadir dimensiones a los elementos con propiedades como **width** y **height**, estas propiedades manejan el tamaño del elemento.

Las unidades de medida pueden ser en **pixeles** o **porcentajes**, normalmente se utilizan porcentajes para imágenes grandes.

```
aside {
  width: 100px;
  height: 20%;
}
```

- **Width** -> Es el ancho del elemento
- **Height** -> El alto de elemento

## Centrando la página

Podemos usar un truco para centrar elemento en una web, primero para aplicar el truco es que el elemento tiene que tener un contenedor que encierre todos los elementos y un ancho especifico, después centrar en **CSS** aplicamos el truco.

```
.container {
  width: 800x;
  margin: 0 auto; <--- El truco
}
```

El contenedor se centrará porque aplicar automáticamente margenes de lado a lado

## Teoría de CSS: Tipos de caja

Los tipos de caja son el comportamiento que tendrá el elemento en el espacio dentro del documento HTML.

Tenemos 3 tipos de caja:

- Block -> Este tipo de caja hace que el elemento ocupe todo el ancho de la pantalla, creando un salto de linea para el siguiente elemento,

- Inline-Block -> Tiene propiedades del modelo de caja Block pero sin ocupar todo el ancho.

- Inline -> Ocupa solo lo que necesita de espacio pero el margen y padding no les afecta en top ni bottom.

```
.elemento {
  display: block / inline-block / inline
}
```

## Teoría de CSS: Posicionamiento absoluto

El posicionamiento absoluto de elementos se refiere a sacar del flow predeterminado del documento html, de arriba para abajo, en este caso el posicionamiento absoluto lo saca y se le puede colocar el cualquier parte del documento. Para realizarlo se necesita el contenedor donde se moverá con libertad el elemento absoluto.

```
.elemento__container {
  position: relative;
}

.elemento {
  position: absolute;
  top: 10px;
  left: 20px;
}
```

El contenedor tiene que tener la declaración **position: relative** para que se le reconozca.

El elemento que se moverá con libertad debe aplicar **position: absolute** y las propiedades **top, left, bottom y right**

Algo importante, si el elemento que será absoluto está dentro de dos contenedores article>header>elemento, y ambos contenedores tienen position relative, entonces el elemento absoluto reconocerá solo al primer contenedor como su contenedor.

## Pseudo elementos

Los pseudo elementos son selectores que no se pueden seleccionar en html pero si en CSS, por ejemplo podemos seleccionar sola la primera linea de un párrafo, la primera letra de un texto, etc.

También se puede crear elementos desde css a partir de un elemento de html utilizando los pseudo-elementos **::before** y **::after**.

```
p::first-line { color: red; }
p::first-letter { font-style: italic; }

h2::after {
  content: "TOP" <-- Contenido del pseudo-elemento;
  display: inline-block;
  ...
}

h2::before {
  content: "TOP" <-- Contenido del pseudo-elemento;
  display: inline-block;
  ...
}
```

# Diseños: Floats, Flexbox y CSS Grid

## Los 3 métodos para construir diseños

Tenemos tres formas de construir diseños en CSS, podemos usar

- Floats -> Los floats son parecidos al **position:absolute** solo que cuando un elemento es flotante, los demás flotan a su alrededor. (Ya no se usa actualmente)

- Flex-box -> Organiza los elementos de un contenedor de forma vertical o horizontal, unidimensional.

- CSS Grid -> Organiza elementos de forma bidimensional, creando una cuadricula que abarca columnas y filas.

## Usamos floats

Para utilizar floats usamos la propiedad **float** con su valor **left/right** según nos sea necesario.

Si todos los elementos de un contenedor son float, entonces el contenedor perderá su altura, como si dichos elementos no existieran dentro de él.

Se resuelve con un truco.

```
.element {
  float: right / left
}
```

El truco se **clear: both**, se aplica en el contenedor de los elemento flotantes para recuperar el tamaño de altura de los contenedores.

```
.parentElement {
  clear: both;
}
```

<br>

# Glosario de etiquetas HTML

Aquí almacenaré cada etiqueta usada para poder acceder fácilmente a ellas, los conceptos que tendrán serán los que yo crea que son.

`<!DOCTYPE html lang="">` -> Indica que se utilizará HTML 5 en el documento, por defecto siempre debe ir. 'lang' es para poner en que idioma estará la página.

`<html></html>` -> Es el contenedor principal de toda pagina html, este elemento indica al navegador que todo lo que esté dentro lo interprete como código HTML.

`<body>` -> Elemento que hace de contenedor a todos los demás elementos que se mostrarán en pantalla, todo lo que esté dentro de `<body>` se renderizara.

`<head>` -> Es un contenedor de meta datos y configuraciones esenciales para la página, no muestra nada en pantalla, solo define información técnica, enlaces a recursos.

`<title>` -> Se usa para colocar el titulo de la pestaña.

`<h1> - <h6>` -> Son elementos de encabezado, con este elemento defines títulos y subtítulos en una página web. La más importante es el H1 y va bajando en jerarquía h2,h3,h4...h6 es el mínimo.

`<p>` -> Es una etiqueta de las más básicas y esenciales, se utiliza para agrupar texto en bloques de contenido separados. No es decorativo, usar `<span>` en ese caso para aplicar estilos, no puede llevar elementos como `<div>`, `<h1> - <h6>` o otro `<p>` dentro.

`<em>` -> Se usa para dar énfasis semántico al texto, también indica que debe tener énfasis lingüístico.

`<strong>` -> También para dar énfasis semántico pero en este caso para marcar el texto como de alta importancia, seriedad o urgencia.

`<ol>` -> Se utiliza para crear listas ordenadas, que son secuenciales, su semántica es presentar el texto de forma consecutiva, respetando el orden de los elementos.

`<ul>` -> Se usa para listas que no son necesariamente ordenadas.

`<li>` -> Se utiliza para definir el item individual dentro de una lista.

`<img>` -> Sirve para insertar imágenes en un página web.

`<a>` -> Sirve para definir enlaces/link/hipervínculos.

`<header>` -> Encierra el encabezado de una web.

`<nav>` -> Identifica la lista de enlaces que sirven para navegar por la web.

`<article>` -> Representa un contenido individual que no tenga que ver con la web actual.

`<footer>` -> Pie de página de la web con información extra.

<br>

# Glosario de propiedades CSS

- **font-size** -> Configura el tamaño de letra
- **font-family** -> Define la tipografía
- **font-weight** -> El grosor de la tipografía
- **line-height** -> El espacio que hay entre lineas
- **text-transform** -> Minúsculas, mayúsculas o capitalizado
- **color** -> Color de la tipografía
- **letter-spacing** -> El espacio entre letras en un palabra
- **text-align** -> Alineamiento del texto.
- **border** -> Podemos agregar un borde al rededor del elemento.
- **background** -> Agrega fondo de colores, imágenes y configurar su presentación.
- **text-decoration** -> Agrega una decoración alrededor del texto.
- **margin** -> Crea espacio a los alrededores del elemento, no cuenta como tamaño del elemento en si.
- **padding** -> Crea relleno en el elemento, este si cuenta como tamaño del contenido.
- **width** -> Es el ancho del elemento
- **height** -> El alto de elemento
- **display** -> Define el comportamiento del elemento respecto al espacio

<br>

# Glosario de pseudo-clases en CSS

- **first-child** -> Captura si es el primer elemento de un contenedor.
- **last-child** -> Captura si es el ultimo elemento de un contenedor.
- **nth-child(0-9/even/odd)** -> Captura el elemento según el indice que le pasemos.
- **link** -> Identifica a los elementos que contengan el atributo href.
- **visited** -> Captura o aplica estilos al enlace que ha sido visitado.
- **hover** -> Aplica estilos al elemento que tiene el puntero del mouse apuntando.
- **active** -> Aplica los estilos cuando haces click.
