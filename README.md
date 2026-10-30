# Tolotti Ebanistas

Es un sitio web ficticio, inspirado en mi abuelo materno y su hermano que eran ebanistas. Me lo imaginé como un emprendimiento familiar dedicado a la ebanistería y fabricación de muebles de estilo clásico.

El proyecto es realizado en el marco de aprendizaje de la materia **CSS**, dentro de la Diplomatura de "Full Stack Development" de Coderhouse. Es la entrega final de la materia: integra HTML semántico, SCSS, Bootstrap, responsive, animaciones y SEO.

## Sitio publicado

[agostinatolotti.github.io/proyecto-css-agostinatolotti](https://agostinatolotti.github.io/proyecto-css-agostinatolotti/)

Está publicado en GitHub Pages, con autorización de la profe Lau, en lugar de Vercel o Netlify.

## Contenido

El sitio cuenta con las siguientes secciones:

- **Inicio**
- **Nosotros**
- **Servicios**
- **Proyectos**
- **Contacto**
- **Producto de la semana**

La consigna pide 5 páginas: Producto de la semana es una página extra, con la ficha del mueble que se publica cada semana.

## Tecnologías

- HTML5
- SCSS (Sass), compilado a un único CSS
- Bootstrap 5.3 (versión 5.3.8, por CDN)
- Animate.css (versión 4.1.1, por CDN)
- AOS (versión 2.3.1, por CDN)

## Estructura de archivos

- `index.html` en la raíz y las demás páginas en `pages/`.
- Estilos en SCSS en `scss/` y el CSS compilado en `styles/`.
- Imágenes, íconos y tipografías en `assets/`.

## Bootstrap

Componentes y estilos aplicados:

- **Navbar** responsive con menú hamburguesa (collapse) en todas las páginas, adaptado a la paleta del sitio.
- **Carruseles** en Inicio (El taller) y en Proyectos (Joyas destacadas y Mobiliario señorial). Como Bootstrap 5 pasa de a una diapositiva, armé cada una con varias fotos, para mostrar más de una pieza a la vez. Mobiliario señorial además avanza solo.
- **Acordeón** en Servicios, para las preguntas frecuentes.
- **Pseudoclases** :hover, :focus y :active con transition en links, botones, controles de los carruseles, imágenes de las galerías y campos del formulario.

## Animaciones

Animaciones propias:

- **Transiciones** sobre cambios de estado: zoom leve en las fotos y galerías, íconos del footer y de contacto que se mueven al pasar el mouse, títulos de las características que se subrayan y bocetos de Servicios que se enderezan.
- **@keyframes** propios: entrada suave del banner de Inicio, entrada en cascada de los links del menú en celular, latido del botón de Servicios y aparición suave del contenido al cambiar de página.
- Todas usan **transform** u **opacity**, con duraciones entre 200 y 500 ms y ease-out para las entradas.

Librerías:

- **Animate.css** en los títulos principales de cada página.
- **AOS** en las secciones que aparecen al hacer scroll, con distintos efectos según la página: en Nosotros, todo lo de Francisco entra desde la izquierda y todo lo de Enrique desde la derecha, y en Servicios cada palabra de "¿Qué fabrican?" llega con una animación diferente.

## SCSS

Todos los estilos están escritos en SCSS; styles.css es solo el resultado de la compilación.

- **Estructura en partials:** utilities (variables, mixins y extends), base (reset, tipografía, estilos globales, animaciones y accesibilidad), layout (header, nav, footer y secciones), components (botones, carruseles, intros y textos) y pages (un partial por página).
- **main.scss** es el único punto de entrada y solo contiene directivas @use. Cada partial importa por su cuenta las variables y mixins que usa.
- **Variables** para la paleta, las tipografías, los espaciados, los tamaños de texto, los bordes y las transiciones.
- **Mixins con parámetros:** columna y fila para las estructuras flex que más se repiten, y uno por breakpoint (celular, tablet, desktop y desktop grande) para las media queries.
- **Extend:** el placeholder %escudo-decorativo agrupa las propiedades que comparten los escudos de fondo de Servicios y Contacto, y se aplica con @extend.
- **Anidamiento y &** para pseudoclases, pseudoelementos y media queries, que ahora viven junto a cada regla.

Para compilar: `sass --watch scss/main.scss styles/styles.css`

## Responsive

Mobile first, con media queries anidadas a través de mixins: celular (hasta 767px), tablet (desde 768px), desktop (desde 1024px) y desktop grande (desde 1224px).

## SEO

- Cada página tiene su propio `<title>`, `<meta description>` y `<meta keywords>`.
- Todas las imágenes tienen su atributo `alt`.

Incluí `<meta keywords>` porque lo pide la consigna de la entrega final aunque sé que es una etiqueta obsoleta: Google la dejó de usar para posicionar en el 2009.

## Accesibilidad

En el partial de accesibilidad, que se carga último, está el bloque **prefers-reduced-motion**, que desactiva las animaciones para quienes tienen activada la opción de reducir el movimiento.

## Cronología

Creación del repositorio: 01/10/2026.
Proyecto trabajado localmente con anterioridad.

Preentrega 2: Entregado el 04/10/2026
(Layouts flexibles y espaciado preciso en el portafolio)

Preentrega 3: Entregado el 08/10/2026
(Maquetación con CSS Grid y Media Queries)

Preentrega 4: Entregado el 09/10/2026
(Integración de Bootstrap)

Preentrega 5: Entregado el 21/10/2026
(Animaciones y Transiciones)

Preentrega 6: Entregado el 27/10/2026
(Arquitectura SCSS y refactorización completa)

Entrega final: Entregado el 30/10/2026
(Sitio web estático de 5 páginas)

Autora: Agostina Tolotti.
