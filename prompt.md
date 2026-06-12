<rol>
Sos un desarrollador web full-stack senior y diseñador UI/UX especializado en sitios de turismo y agencias de viajes de alto impacto visual. Dominás HTML5 semántico, CSS3 moderno (custom properties, Grid, Flexbox, animaciones con @keyframes) y JavaScript vanilla. Tu código es limpio, accesible y visualmente memorable. Siempre entregás productos listos para producción.
</rol>

<proyecto>
Construí la landing page de "Nómada Viajes" — una agencia de viajes boutique ficticia especializada en experiencias de viaje auténticas y personalizadas alrededor del mundo. Su propuesta de valor es diseñar itinerarios únicos adaptados a cada viajero, lejos del turismo masivo. El público objetivo son adultos de entre 28 y 55 años que buscan viajes con sentido, calidad y atención personalizada.

Identidad de marca:
- Nombre: Nómada Viajes
- Eslogan: "Cada destino, una historia."
- Color primario: #1A6B5A (verde selva profundo)
- Color acento: #F4A261 (naranja atardecer)
- Fondo base: #0C1B26 (azul noche)
- Superficie / tarjetas: #112233
- Texto principal: #F2F7F5
- Texto secundario: #85AEAD
- Borde sutil: #1C3040
- Fuente titular: "Playfair Display" de Google Fonts (pesos 600, 700, 900 — elegancia y aventura)
- Fuente cuerpo: "Inter" de Google Fonts (pesos 400, 500, 600)
- Íconos: Font Awesome 6 Free vía CDN
- Referencia estética: revista de viajes premium, oscura y exuberante — verde, naranja y noche
- Tono de voz: inspirador, cálido, sofisticado — invita a soñar y luego a reservar
</proyecto>

<tarea>
Construí una landing page completamente autocontenida en un único archivo index.html.
- Todo el CSS dentro de un bloque <style> en el <head>.
- Todo el JavaScript dentro de un bloque <script> justo antes del </body>.
- Google Fonts y Font Awesome 6 cargados exclusivamente con etiquetas <link> de CDN.
- Sin referencias a archivos locales ni a URLs de imágenes externas.
- Sin datos de contacto reales: no incluir teléfonos, direcciones físicas ni usuarios de redes sociales reales. Los emails deben usar el dominio ficticio de la agencia (ej: contacto@nomadaviajes.com).
- El archivo debe funcionar correctamente al abrirlo directo en el navegador sin servidor.
</tarea>

<secciones_requeridas>
Implementá exactamente estas 7 secciones en este orden. Cada una debe estar comentada con <!-- ========== SECCIÓN: NOMBRE ========== -->

──────────────────────────────────────────
SECCIÓN 1 — CABECERA (Header con menú de navegación)
──────────────────────────────────────────
Requisito del PDF: Header con menú de navegación.

- Barra fija (position: fixed) en la parte superior, z-index elevado.
- Transición al hacer scroll (> 60px): agregar backdrop-filter: blur(10px), fondo semitransparente y sombra inferior sutil.
- Izquierda: SVG inline de una brújula estilizada (en color acento naranja) + "Nómada Viajes" en Playfair Display, negrita.
- Centro: menú de navegación con los enlaces — Destinos, Servicios, Nosotros, Testimonios, Contacto. Cada enlace hace smooth-scroll a su sección correspondiente.
- Derecha: botón "Reservar Ahora" con forma de píldora, fondo degradado verde → naranja, hover con ligera escala.
- Mobile (< 768px): ocultar enlaces y botón; mostrar botón hamburguesa (☰ / ✕) que despliega menú vertical de ancho completo con transición CSS suave.

──────────────────────────────────────────
SECCIÓN 2 — HERO SECTION (Sección principal con título impactante y CTA)
──────────────────────────────────────────
Requisito del PDF: Hero Section con título impactante y botón de llamada a la acción.

- Altura: 100vh. Contenido centrado verticalmente y horizontalmente.
- Píldora / badge sobre el título: "✦ Experiencias de viaje a medida desde 2009" con borde degradado verde y naranja.
- Título H1 (font-size ≥ 64px, Playfair Display, font-weight 900): "El mundo te espera. Nosotros te llevamos."
- Subtítulo (18px, Inter, color secundario, max-width 540px): "Diseñamos itinerarios únicos en más de 80 destinos. Viajá con propósito, viajá con Nómada."
- Dos botones CTA uno al lado del otro:
  · "Explorar Destinos" — relleno, degradado verde → naranja, forma de píldora, ícono fa-arrow-right.
  · "Conocer Más ↓" — ghost/contorno, mismo border-radius, ícono fa-compass.
- Fondo: degradado radial animado con @keyframes usando verde #1A6B5A y azul noche #0C1B26 a baja opacidad, con movimiento lento e infinito.
- Elemento decorativo: composición SVG/CSS pura de un mapamundi estilizado (círculo con líneas de latitud y longitud, puntos de destino) en verde con trazos naranjas. Sin etiquetas <img> con URLs externas.

──────────────────────────────────────────
SECCIÓN 3 — DESCRIPCIÓN / SOBRE NOSOTROS
──────────────────────────────────────────
Requisito del PDF: Descripción / Sobre Nosotros.

- Título H2: "Quiénes somos"
- Párrafo principal (2–3 oraciones, max-width 700px, centrado): descripción de la agencia, su filosofía de viaje personalizado y sus años de experiencia.
- Tres tarjetas de estadísticas en fila horizontal (responsive: columna en mobile):
  · "+80" / "Destinos en 5 continentes" / ícono fa-earth-americas
  · "+12.000" / "Viajeros satisfechos" / ícono fa-users
  · "15 años" / "Creando experiencias" / ícono fa-star
- Cada estadística: número grande (≥ 48px, Playfair Display, degradado verde → naranja), etiqueta abajo, ícono arriba.
- Los números se animan de 0 al valor final con JavaScript vía IntersectionObserver al entrar en el viewport.
- Fondo: #112233 para separar visualmente del hero.

──────────────────────────────────────────
SECCIÓN 4 — SECCIÓN DE SERVICIOS O CARACTERÍSTICAS PRINCIPALES
──────────────────────────────────────────
Requisito del PDF: Sección de Servicios o Características principales.

- Título H2: "Nuestros Servicios"
- Subtítulo: "Todo lo que necesitás para un viaje sin preocupaciones."
- CSS Grid de 6 tarjetas de servicio:
  · 1 columna en mobile, 2 en tablet (≥ 768px), 3 en desktop (≥ 1200px).
  · Tarjeta 1: fa-globe | "Paquetes Internacionales" | "Armamos paquetes completos a medida con vuelos, alojamiento y actividades en los cinco continentes."
  · Tarjeta 2: fa-person-hiking | "Viajes de Aventura" | "Trekking, safaris, expediciones y actividades de naturaleza para los viajeros más intrépidos."
  · Tarjeta 3: fa-heart | "Viajes Románticos" | "Lunas de miel y escapadas en pareja diseñadas para crear recuerdos que duran toda la vida."
  · Tarjeta 4: fa-users | "Tours Grupales" | "Grupos pequeños con guías especializados para una experiencia íntima y enriquecedora."
  · Tarjeta 5: fa-ship | "Cruceros y Navegación" | "Itinerarios fluviales y marítimos por los destinos más icónicos y los más secretos del mundo."
  · Tarjeta 6: fa-headset | "Asistencia de Viaje" | "Acompañamiento permanente antes, durante y después de tu viaje para que no estés solo en ningún momento."
- Hover en tarjetas: translateY(-6px) + box-shadow con resplandor verde de baja opacidad.
- Animación: fade-in escalonado (0ms, 100ms, 200ms, 300ms, 400ms, 500ms) vía IntersectionObserver.

──────────────────────────────────────────
SECCIÓN 5 — TESTIMONIOS O RESEÑAS DE CLIENTES
──────────────────────────────────────────
Requisito del PDF: Testimonios o Reseñas de clientes.

- Título H2: "Lo que dicen nuestros viajeros"
- Tres tarjetas de testimonio en fila responsive (columna en mobile):
  · Tarjeta 1: ★★★★★ | "Viajamos con Nómada para nuestra luna de miel a Islandia y fue perfecto. Cada detalle estuvo cuidado al máximo. Volvimos transformados." | Avatar "ML" con degradado verde → naranja | Martina López y Rodrigo Cano, Luna de Miel en Islandia
  · Tarjeta 2: ★★★★★ | "El viaje familiar a Japón superó todas nuestras expectativas. Los chicos quedaron fascinados y nosotros también. El guía local fue extraordinario." | Avatar "PF" | Paula y Diego Ferreyra, Familia — Tokio y Kioto
  · Tarjeta 3: ★★★★★ | "Hice el trekking en la Patagonia chilena con el grupo de aventura. Una experiencia de vida que no podría haber organizado mejor solo. 100% recomendable." | Avatar "SM" | Santiago Morales, Torres del Paine
- Estrellas: íconos fa-star de Font Awesome en naranja acento (#F4A261).
- Avatar de iniciales: div circular con degradado verde → naranja, iniciales en blanco y negrita.
- Tarjetas: borde 1px solid #1C3040, fondo #112233, hover con leve elevación.

──────────────────────────────────────────
SECCIÓN 6 — FORMULARIO DE CONTACTO (Maquetado visual)
──────────────────────────────────────────
Requisito del PDF: Formulario de contacto (maquetado visual, sin funcionalidad backend).

- Título H2: "Planeá tu próximo viaje"
- Subtítulo: "Completá el formulario y un asesor de viajes se contacta con vos en menos de 24 horas."
- Formulario centrado, max-width: 680px, margin: 0 auto.
- Campos requeridos con <label> visible y bien estilizado:
  · Nombre completo (type="text", placeholder="Tu nombre completo")
  · Email (type="email", placeholder="tu@email.com")
  · Destino de interés (type="text", placeholder="¿A dónde soñás ir?")
  · Cantidad de viajeros (select: 1 persona, 2 personas, 3–5 personas, Grupo de +6)
  · Mensaje (textarea rows=4, placeholder="Contanos más sobre el viaje que tenés en mente...")
- Botón: "Enviar Consulta →" — ancho completo, degradado verde → naranja, Inter 600.
- Al enviar: preventDefault(), ocultar el formulario, mostrar mensaje inline: "✓ ¡Consulta recibida! Te contactamos pronto. ¡Buen viaje! ✈" en color acento. Sin recarga de página.
- No incluir datos de contacto reales (sin teléfonos ni direcciones físicas).
</secciones_requeridas>

──────────────────────────────────────────
SECCIÓN 7 — PIE DE PÁGINA (Footer con enlaces a redes sociales)
──────────────────────────────────────────
Requisito del PDF: Pie de página con enlaces a redes sociales.

- Fondo: #060E15 (más oscuro que el fondo base).
- Layout multi-columna (2 columnas en mobile, 4 en desktop):
  · Columna 1: logo + eslogan "Cada destino, una historia." + íconos de redes sociales: fa-instagram, fa-facebook-f, fa-x-twitter, fa-youtube — todos href="#" con aria-label descriptivo en cada uno.
  · Columna 2: "Destinos" — Europa, Asia, América, Oceanía (todos href="#").
  · Columna 3: "Servicios" — Paquetes, Aventura, Cruceros, Grupos (todos href="#").
  · Columna 4: "Agencia" — Sobre Nosotros, Blog de Viajes, Trabajá con Nosotros, Contacto (todos href="#").
- Línea divisoria (border-top sutil) antes de la barra inferior.
- Barra inferior: "© 2026 Nómada Viajes. Todos los derechos reservados." centrado, texto secundario pequeño.

<requisitos_tecnicos>
CSS:
- Todas las variables de color, tipografía y espaciado como custom properties en :root.
- Mobile-first: estilos base para 320px, breakpoints con min-width en 768px y 1200px.
- Padding vertical de sección: 96px en desktop, 64px en mobile.
- Ancho máximo de contenido: 1200px, centrado con margin: 0 auto y padding horizontal de 24px.
- Transiciones: transition: all 0.25s ease en todos los elementos interactivos.
- Sistema de espaciado de 8px (todos los padding, margin y gap son múltiplos de 8).
- Cero atributos style inline — todo el estilo exclusivamente vía clases CSS.

JavaScript:
- IntersectionObserver para animaciones de scroll (fade-in + translateY de 24px a 0).
- Delays escalonados en tarjetas usando data-delay o nth-child.
- Hamburguesa: toggle de clase CSS (.activo), sin librerías externas.
- Contadores animados: de 0 al valor final, ~1500ms, easing easeOutCubic.
- Navbar: agregar clase .scrolled al superar 60px de scroll vertical.
- Formulario: success state con ocultamiento del form y mensaje de éxito.

HTML:
- Estructura: <header>, <nav>, <main>, <section id="...">, <footer>.
- Un único <h1> en hero. <h2> por sección. <h3> en títulos de tarjeta.
- aria-label en íconos interactivos (hamburguesa, redes sociales).
- id en cada sección coincidiendo con los href del navbar para smooth-scroll.
- scroll-behavior: smooth en el elemento html.
- Contraste WCAG AA mínimo en todo el texto.
</requisitos_tecnicos>

<formato_de_salida>
Entregá ÚNICAMENTE el HTML puro del archivo index.html.
- Sin bloques markdown (```html).
- Sin texto antes ni después del HTML.
- Sin comentarios placeholder del tipo "agregar contenido aquí".
- El primer carácter debe ser < (apertura de <!DOCTYPE html>).
- Documento HTML5 único, completo y válido con las 7 secciones íntegras.
</formato_de_salida>
