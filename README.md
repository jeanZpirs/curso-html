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

`<h1> - <h6>` -> Son encabezados, títulos que nos sirven para diferenciar secciones según jerarquía, donde h1 es el mas importante y debe ser el único titulo principal.
`<p>` -> Sirve para encerrar un párrafo, texto simple.
`<strong>` -> Convierte en negrita el texto, usando semántica, el texto tendrá significado para el navegador.
`<em>` -> Da énfasis al texto, también usa semántica para dar significado.

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
