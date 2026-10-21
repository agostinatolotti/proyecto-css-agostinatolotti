# Tolotti Ebanistas

Es un sitio web ficticio, inspirado en mi abuelo materno y su hermano que eran ebanistas. Me lo imaginé como un emprendimiento familiar dedicado a la ebanistería y fabricación de muebles de estilo clásico.

El proyecto es realizado en el marco de aprendizaje de la materia **CSS**, dentro de la Diplomatura de "Full Stack Development" de Coderhouse. Lo publiqué a partir de la preentrega n2, para evolucionar a partir de la misma según el contenido que veamos durante la cursada. 

## Contenido

El sitio cuenta con las siguientes secciones:

- **Inicio**
- **Nosotros**
- **Servicios**
- **Proyectos**
- **Contacto**
- **Producto de la semana**

## Tecnologías

- HTML5
- CSS
- Bootstrap 5.3 (versión 5.3.8, por CDN)
- Animate.css (versión 4.1.1, por CDN)
- AOS (versión 2.3.1, por CDN)

## Bootstrap

En la preentrega 4 había usado Bootstrap 6, que todavía está en versión alpha (de prueba). Siguiendo la devolución de la profe, lo migré a Bootstrap 5.3, que es la versión estable que usamos en la cursada.

Componentes y estilos aplicados:

- **Navbar** responsive con menú hamburguesa (collapse) en todas las páginas, adaptado a la paleta del sitio.
- **Carruseles** en Inicio (El taller) y en Proyectos (Joyas destacadas y Mobiliario señorial). Como Bootstrap 5 pasa de a una diapositiva, armé cada una con varias fotos para mantener el diseño que tenía con la versión anterior. Mobiliario señorial además avanza solo.
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

## Detalles

Accesibilidad: al final de la hoja de estilos está el bloque **prefers-reduced-motion**, que desactiva las animaciones para quienes tienen activada la opción de reducir el movimiento.

En esta entrega también cerré el responsive de todas las páginas, rediseñé Servicios, sumé una intro a Nosotros, armé la ficha del producto de la semana y optimicé el peso de las imágenes.

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

Autora: Agostina Tolotti.