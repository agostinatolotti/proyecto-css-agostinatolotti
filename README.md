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
- Bootstrap 6 (versión 6.0.0-alpha.1, por CDN)

## Bootstrap

Elegí usar Bootstrap 6, la última versión, así que hay algunas cosas como el loop de las galerías que no termina de funcionar bien, creo que es por eso. Otra cuestión a tener en cuenta es que cambiaron algunas nomenclaturas y se "homogeneizaron" un poco más con lo que veníamos viendo por suerte:

- El menú desplegable del navbar ahora se llama **drawer** (en Bootstrap 5 era **offcanvas**).
- Cambian los cortes de pantalla: **md** sigue en 768px, pero **lg** pasa de 992px a 1024px, **xl** de 1200px a 1280px y **xxl** (1400px) pasa a llamarse **2xl** (1536px).

Componentes y estilos aplicados:

- **Navbar** responsive con menú hamburguesa en todas las páginas, adaptado a la paleta del sitio.
- **Carruseles** en Inicio (El taller) y en Proyectos (Joyas destacadas, con fotos de ancho variable, y Mobiliario señorial, con las fotos laterales asomadas y avance automático).
- **Pseudoclases** :hover, :focus y :active con transition en links, botones, controles de los carruseles, imágenes de las galerías y campos del formulario.

Me fijé las diferencias de ambas versiones y preferí usar la nueva para que no me falle ningún componente, y quizás fue contraprocucente, pero todo sirve para aprender. Espero que siga siendo válido.

Creación del repositorio: 01/10/2026.
Proyecto trabajado localmente con anterioridad.

Preentrega 2: Entregado el 04/10/2026
(Layouts flexibles y espaciado preciso en el portafolio)

Preentrega 3: Entregado el 08/10/2026
(Maquetación con CSS Grid y Media Queries)

Preentrega 4: Entregado el 09/10/2026
(Integración de Bootstrap)

Autora: Agostina Tolotti.