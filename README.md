# landing-page

Mejoras semánticas que me ayudó la IA con instrucciones de los requerimientos del laboratorio.
El prompt que usé fue:
Eres un experto creando landing pages. Tienes años de experiencia en html y css. Quiero que me ayudes a crear una landing page para un microfono de streaming, es de la marca fifine y el modelo es AM8. Te daré el dibujo de la estructura para que lo conviertas en codigo html y css. Pero tienes que tener en consideracion lo criterios de usuario que te diré a continuacion(aqui escribi los requerimientos que me dieron en el laboratorio)
El primer resultado que me dio, estuvo lleno de divs. Asi que le di la orden de que reemplazara los divs por etiquetas semanticas correctas y tenga en cuenta los requerimientos que le di, y esta fue su respuesta:


En el Header:

Reemplacé el div.header-container por un <section>
Convertí el logo en un verdadero <h1>
El menú de utilidades (carrito, login) ahora es un segundo <nav> con aria-label específico


En el Main:

Agregué un <article> como contenedor principal
Las secciones principales usan <section> correctamente
Reemplacé los div.hero-text por <article class="product-info">
Convertí la imagen del producto en un <figure> con <figcaption>


En la Sección de Precios y Métodos de Pago:

La sección de precio ahora usa semántica correcta
Los iconos de pago están dentro de elementos <figure>
El botón de CTA ahora está dentro de una <section> apropiada


En el Footer:

Reemplacé los div.footer-section por <article>
Los enlaces sociales ahora están dentro de un <nav> con aria-label



Jerarquía de encabezados:

Ajusté la jerarquía de encabezados para que sea correcta y lógica
<h1> para el logo de la marca
<h2> para el título del producto principal
<h3> para subtítulos de secciones

Todos estos cambios mejoran la semántica del documento sin afectar su apariencia visual.