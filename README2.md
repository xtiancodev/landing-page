# Landing Page – FIFINE AM8

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
