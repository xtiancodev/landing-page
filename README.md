# LABORATORIO 01

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


# LABORATORIO 02

## 📱 Breakpoints de Media Queries

Para asegurar que la página sea responsiva y se vea bien en distintos tamaños de pantalla, se utilizaron los siguientes breakpoints:

---

### 🔹 `@media (max-width: 992px)`
- Se usa para adaptar el diseño en tablets o laptops pequeños.
- Ajusta el número de columnas en la galería de imágenes a 2 por fila.

---

### 🔹 `@media (max-width: 768px)`
- Aplica para pantallas de tablets verticales y móviles grandes.
- El menú de navegación cambia su distribución para evitar que los elementos se amontonen.
- El contenedor principal del encabezado se apila en vertical (`flex-direction: column`).
- El contenido del `footer` también se organiza en columna para mejor lectura.

---

### 🔹 `@media (max-width: 600px)`
- Orientado a móviles pequeños.
- La galería de imágenes cambia a 1 sola columna por fila para mayor legibilidad.

---

## 💡 Notas
- Se utilizó `display: flex`, `flex-wrap`, `justify-content` y `align-items` para lograr una disposición adaptable.
- El enfoque fue cumplir con las historias de usuario para lograr una experiencia visual fluida en distintas resoluciones.

# LABORATORIO 03
# 💻 Proyecto Web – Página Responsiva con CSS Grid y Flexbox

Este proyecto consiste en una landing page principal, una página de testimonios y una página de compra, desarrolladas con HTML5 y CSS3. Todas las páginas son **completamente responsivas** y cumplen con el historial de usuario.

---

## 📄 Estructura del Proyecto

- `index.html`: Landing page del producto FIFINE AM8
- `testimonios.html`: Página con opiniones de usuarios organizadas en una grilla responsiva
- `compra.html`: Página simulada de proceso de compra con layout estructurado

---

## 📱 Breakpoints de Media Queries

Se utilizaron los siguientes puntos de ruptura para adaptar el diseño a distintos dispositivos:

### 🔹 `@media (max-width: 992px)`
- Ajuste de columnas en la galería de imágenes a 2 por fila.
- Pensado para tablets grandes y laptops pequeños.

### 🔹 `@media (max-width: 768px)`
- Reorganización de layout Grid a una sola columna (navbar, aside y main en stack vertical).
- Sidebar se mueve debajo del navbar.
- Footer se adapta a formato de columna.
- Menú de navegación con `flex-wrap` para evitar amontonamiento.

### 🔹 `@media (max-width: 600px)`
- Galería de imágenes en `index.html` se convierte en una sola columna para móviles.
- Tarjetas de testimonios (`.card`) se expanden al 100% del ancho para mayor legibilidad.

---

## 💡 Tecnologías y técnicas utilizadas

- HTML5 semántico (`<header>`, `<nav>`, `<main>`, `<aside>`, `<footer>`)
- CSS3 con variables personalizadas y diseño responsivo
- **CSS Grid**: usado en la estructura de páginas `testimonios.html` y `compra.html`
- **Flexbox**: usado para distribuir elementos en navegación, galería y secciones internas
- Buenas prácticas de accesibilidad: uso de `alt` en imágenes, `aria-label` en menús

---

## ✔️ Cumplimiento de Historias de Usuario

- ✅ HU1 – Página de testimonios con layout responsivo y filtros simulados
- ✅ HU2 – Página de compra con estructura clara y secciones informativas
- ✅ HU3 – Todas las páginas adaptadas a móviles con scroll horizontal evitado

---

## 📎 Notas finales

- El proyecto fue desarrollado con enfoque en la semántica, la accesibilidad y el comportamiento adaptativo.
- Los estilos están centralizados en un solo archivo `styles.css`.
- El código está comentado para facilitar su comprensión y evaluación.
