---
name: Luis Serrano — Portfolio
designer: Luis Serrano
description: Sistema de diseño para portfolio de diseñador gráfico digital y creador audiovisual. Firma roja sobre base oscura, titulares condensados y fotografía de gran formato.
source: Design_luis.docx

colors:
  primary: "#FF2028"
  primary-hover: "#FF4A50"
  wine: "#650D16"
  royal: "#2448FF"
  lime: "#C4FF00"
  yellow: "#FFE600"
  orange: "#FF6A00"
  magenta: "#FF2DAA"
  violet: "#783BFF"
  cyan: "#00D9F5"
  background: "#101010"
  surface: "#202020"
  muted: "#B8B4AE"
  foreground: "#F4F0E8"
  white: "#FFFFFF"
  # Complementos razonables — [REVISAR]
  border-subtle: "#2E2E2E"
  overlay: "rgba(16, 16, 16, 0.85)"
  focus-ring: "{colors.foreground}"
  error: "{colors.primary}"
  success: "{colors.lime}"

typography:
  family-display: "Barlow Condensed"
  family-body: "Barlow"
  family-accent: "Ballet"
  display:
    family: "{typography.family-display}"
    weight: 800
    size-desktop: "96-160px"
    size-mobile: "56-80px"
    line-height: 0.95
    letter-spacing: "-0.02em"
    transform: uppercase
  h1:
    family: "{typography.family-display}"
    weight: 800
    size-desktop: "80px"
    size-mobile: "48px"
    line-height: 1.05
  h2:
    family: "{typography.family-display}"
    weight: 800
    size-desktop: "64px"
    size-mobile: "40px"
    line-height: 1.05
  h3:
    family: "{typography.family-display}"
    weight: 700
    size-desktop: "36px"
    size-mobile: "28px"
    line-height: 1.15
  h4:
    family: "{typography.family-body}"
    weight: 700
    size-desktop: "24px"
    size-mobile: "20px"
    line-height: 1.25
  lead:
    family: "{typography.family-body}"
    weight: 500
    size-desktop: "24px"
    size-mobile: "20px"
    line-height: 1.4
  body:
    family: "{typography.family-body}"
    weight: 400
    size-desktop: "18px"
    size-mobile: "16-18px"
    line-height: 1.5
    max-measure: "60-70ch"
  nav:
    family: "{typography.family-body}"
    weight: 600
    size: "16px"
    line-height: 1.25
  button:
    family: "{typography.family-body}"
    weight: 600
    size: "16px"
    line-height: 1.25
    letter-spacing: "0.03em"
    transform: uppercase
  label:
    family: "{typography.family-body}"
    weight: 600
    size: "14px"
    line-height: 1.3
    letter-spacing: "0.04em"
    transform: uppercase
  caption:
    family: "{typography.family-body}"
    weight: 400
    size: "14-16px"
    line-height: 1.4
    color: "{colors.muted}"
  link-inline:
    family: "{typography.family-body}"
    weight: 500
    decoration: underline
  # [REVISAR] Barlow Condensed no estaba en Tipografia/*.woff — solo Barlow regular. Añadir Barlow Condensed o usar Barlow SemiBold/ExtraBold como sustituto.

spacing:
  scale: [4, 8, 12, 16, 24, 32, 48, 64, 96, 128]
  container-max: "1440px"
  grid-desktop-columns: 12
  grid-desktop-margin: "48-64px"
  grid-desktop-gutter: "24px"
  grid-tablet-columns: 8
  grid-tablet-margin: "32px"
  grid-mobile-columns: 1
  grid-mobile-margin: "20px"
  section-gap-desktop: "96-128px"
  section-gap-tablet: "80px"
  section-gap-mobile: "56-72px"
  related-gap: "16-32px"
  list-item-gap: "8px"
  feature-split: "7/5"

rounded:
  default: "0px"
  button: "0px"
  card: "0px"
  image: "0px"
  input: "0px"
  badge: "0px"
  # Nota: se evitan píldoras. Todo recto. [REVISAR] si algún tag pequeño necesita 2px.

components:
  button-primary:
    background: "{colors.primary}"
    background-hover: "{colors.primary-hover}"
    text: "#000000"
    rounded: "{rounded.button}"
    min-height: "48px"
    press-scale: 0.98
    transition: "180ms ease-out"
  button-secondary:
    background: "transparent"
    background-hover: "{colors.foreground}"
    text: "{colors.foreground}"
    text-hover: "#000000"
    rounded: "{rounded.button}"
    min-height: "48px"
    border: "1px solid {colors.foreground}"
    transition: "180ms ease-out"
  nav-bar:
    background: "{colors.background}"
    text: "{colors.foreground}"
    active-indicator: "2px underline {colors.primary}"
    min-target: "44x44px"
  mobile-menu:
    background: "{colors.background}"
    open-duration: "220ms"
    link-size: "{typography.h3}"
  project-card:
    background: "transparent"
    rounded: "{rounded.card}"
    shadow: "none"
    image-zoom-hover: 1.03
    image-transition: "220ms ease-out"
    title-underline-hover: true
  filter-chip:
    text: "{colors.foreground}"
    active-indicator: "underline {colors.primary}"
    transition: "180ms ease-out"
  lightbox:
    background: "#000000"
    text: "{colors.foreground}"
  video-player:
    cover-play-button: "{colors.primary}"
    captions-required: true
  form-field:
    background: "{colors.surface}"
    text: "{colors.foreground}"
    border: "1px solid {colors.border-subtle}"
    border-focus: "1px solid {colors.foreground}"
    rounded: "{rounded.input}"
  focus-ring:
    outline: "2px solid {colors.focus-ring}"
    offset: "2px black separator"
    min-target: "44x44px"
  overlay-shadow:
    value: "0 12px 32px rgba(0, 0, 0, 0.35)"
    usage: "solo paneles superpuestos / lightbox / menu movil"
  divider:
    value: "1px solid {colors.border-subtle}"
  motion:
    fast: "150-220ms ease-out"
    reveal: "350ms ease-out + translateY max 16px"
    stagger: "60ms, max-delay 180ms"
    loader: "brief intro max 1200ms, skippable, never blocks content"
    parallax: "scroll-linked translateY/scale, subtle on mobile, full on desktop"
    marquee: "infinite loop for IMPACTO/DOMINIO/DRAMA strip"
    horizontal-drive: "vertical scroll drives horizontal track via sticky pin"
    hover-swap: "image swap/scale 1.08 on hover like helmet hall-of-fame"
---

# Overview

Portfolio de Luis Serrano, diseñador gráfico digital y creador audiovisual, dirigido a agencias, estudios, reclutadores y clientes.

Tres principios: **impacto** (escala y contraste), **dominio** (precisión y presentación de proyectos) y **drama** (luz, encuadre y ritmo).

Dirección: fuerza de cartel tipográfico + atmósfera audiovisual. Fondos oscuros `{colors.background}`, rojo firma `{colors.primary}`, titulares condensados `{typography.family-display}` y fotografía / video de gran formato. Ritmo por cambios de escala: momentos intensos seguidos de espacios de lectura tranquila.

Estructura: portada (nombre + perfil + pieza + `Ver proyectos` / `Contacto`) → selección de proyectos (identidad, social, editorial, motion) → sobre mí + habilidades / herramientas confirmadas + formación / experiencia → contacto. El CV descargable solo aparece cuando existe el PDF. Intro breve tipo loader permitida (máx 1.2s, se puede saltar).

El nombre en mayúsculas condensadas es identificación tipográfica inicial, no logotipo definitivo. Líneas finas, numeración y flechas sencillas orientan sin decorar en exceso.

Fuentes en este repo: `Tipografia/*.woff` (Barlow). [REVISAR] falta `Barlow Condensed` para `{typography.display}` — añadir `BarlowCondensed-ExtraBold.woff` y `BarlowCondensed-Bold.woff`, o confirmar sustituto.

## Colors

Base: rojo saturado sobre negro. Secundarios amplían, nunca reemplazan al rojo.

- `primary #FF2028` — firma. Botones principales, titulares grandes, indicadores, bloques de alto impacto.
- `primary-hover #FF4A50` — hover de botón principal y énfasis.
- `wine #650D16` — profundidad en fondos atmosféricos. Admite texto `{colors.foreground}`.
- `royal #2448FF` — acento secundario puntual. Texto `{colors.foreground}` encima.
- `lime #C4FF00` — acento eléctrico: etiquetas pequeñas, llamadas visuales. Texto negro encima.
- `yellow #FFE600` — resaltar información breve. Texto negro encima.
- `orange #FF6A00` — energía complementaria. Texto negro encima.
- `magenta #FF2DAA` — acento expresivo. Texto negro encima.
- `violet #783BFF` — bloques experimentales. Texto `{colors.foreground}` encima.
- `cyan #00D9F5` — acento fresco puntual. Texto negro encima.
- `background #101010` — fondo dominante. También texto sobre superficies luminosas.
- `surface #202020` — paneles, campos y áreas secundarias sobre oscuro.
- `muted #B8B4AE` — texto secundario sobre oscuro: fechas, categorías, descripciones auxiliares.
- `foreground #F4F0E8` — texto principal sobre oscuro, descanso visual.
- `white #FFFFFF` — contraste y fondos neutros de piezas.

Reglas:

- Una sección = neutros + un dominante. Segundo acento solo en detalles pequeños.
- Categorías siempre con nombre visible, nunca solo por color.
- Proyectos conservan su paleta original. Sin filtro rojo global, sin adaptar marcas.
- Contraste: 4.5:1 texto normal, 3:1 texto grande. Sobre claro, lectura y enlaces en negro; saturados solo como superficie / acento si no dan contraste como texto.
- [REVISAR] `border-subtle #2E2E2E`, `overlay rgba(16,16,16,0.85)`, `error {colors.primary}`, `success {colors.lime}` inventados por falta de dato.

## Typography

Familias: `{typography.family-display}` para display / H1-H3, `{typography.family-body}` para lectura e interfaz. Fuerza por condensación, peso y escala.

- **Display / portada:** `{typography.display}` — 800, 96–160px desktop / 56–80px móvil, lh 0.95, ls −0.02em. Mayúsculas, frases muy breves. Es estilo visual, no nivel de encabezado extra.
- **H1:** 800, 80px / 48px, lh 1.05. Un solo H1 por página, título principal interior.
- **H2:** 800, 64px / 40px, lh 1.05. Grandes secciones.
- **H3:** Bold 700, 36px / 28px, lh 1.15. Nombres de proyecto, subsecciones.
- **H4:** Barlow Bold 700, 24px / 20px, lh 1.25. Detalles en fichas.
- **Entradilla:** Barlow Medium 500, 24px / 20px, lh 1.4.
- **Cuerpo:** Barlow Regular 400, 18px / 16–18px, lh 1.5.
- **Listas:** igual que cuerpo + 8px entre items (`{spacing.list-item-gap}`).
- **Navegación:** SemiBold 600, 16px, lh 1.25. Área mínima 44×44px.
- **Botones:** SemiBold 600, 16px, lh 1.25, ls 0.03em. Mayúsculas en acciones breves.
- **Enlaces en texto:** Medium 500, mismo tamaño del párrafo, con subrayado.
- **Etiquetas:** SemiBold 600, 14px, lh 1.3, mayúsculas, ls 0.04em.
- **Secundarios:** Regular 400, 14–16px, lh 1.4, color `{colors.muted}` sobre oscuro.
- **Énfasis:** Bold 700 al mismo tamaño. Itálica solo para obras o énfasis puntual.

Orden semántico H1→H2→H3 sin saltos. Líneas 60–70ch. Sin párrafos enteros en mayúsculas. Sin condensación artificial. Sin cortes ni desbordes; el tamaño se adapta al contenedor.

## Layout

Ancho máximo `{spacing.container-max}` 1440px.

- Desktop ≥1200px: 12 columnas, márgenes 48–64px, gutter 24px. Destaque full-bleed permitido; asimetría 7/5 (`{spacing.feature-split}`) manteniendo alineaciones.
- Tablet 768–1199px: 8 columnas, márgenes 32px, secciones 80px.
- Móvil 320–767px: 1 columna, márgenes 20px, secciones 56–72px.

Escala de espaciado `{spacing.scale}`: 4, 8, 12, 16, 24, 32, 48, 64, 96, 128. Secciones desktop 96–128px; elementos relacionados 16–32px. El vacío dirige la mirada.

Móvil: composiciones apiladas, títulos siempre horizontales, imágenes con protagonismo, fichas en secuencia. Orden visual = orden de lectura / DOM. Imágenes en tamaños adecuados, carga progresiva fuera del primer viewport. Portada rápida; video pesado nunca bloquea.

Scroll suave a ancla con offset para la barra fija. Experiencia estilo Lando Norris permitida: scroll vertical que mueve pista horizontal (horizontal-drive con sticky pin), títulos fijos por tramo, parallax entre capas y marquee en loop. En móvil se simplifica a 1 columna y el horizontal pasa a swipe manual.

## Elevation & Depth

Profundidad por contraste, escala y fotografía — no por sombras generalizadas.

- Tarjetas y superficies habituales: sin sombra (`{components.project-card.shadow}`).
- Solo superpuestos (menú, lightbox, panel flotante): `{components.overlay-shadow}` — `0 12px 32px rgba(0,0,0,0.35)`.
- Niveles con `{colors.background}` vs `{colors.surface}`, sin volumen extra.
- Títulos sobre imagen solo con zona de lectura clara o scrim que garantice contraste.
- [REVISAR] valor de scrim / gradiente sobre imagen no especificado — sugerido `linear-gradient(rgba(0,0,0,0.55), rgba(0,0,0,0.15))`.

## Shapes

Todo recto: `{rounded.default}` 0px en botones, imágenes, tarjetas y campos (`{rounded.button}`, `{rounded.card}`, `{rounded.image}`, `{rounded.input}`).

Divisores: `{components.divider}` 1px. Flechas y numeración como orientación. Nada de píldoras sistemáticas ni iconografía decorativa masiva. La identificación es el nombre tipográfico.

## Components

Interacción con cursor, táctil y teclado. Movimiento 150–220ms con desaceleración suave (`{components.motion.fast}`) + parallax, marquee y horizontal-drive (`{components.motion.parallax}`, `{components.motion.marquee}`, `{components.motion.horizontal-drive}`). Si `prefers-reduced-motion`: se reduce a cambios mínimos.

- **Navegación:** barra superior `{components.nav-bar.background}` fija. Anclas `Proyectos / Sobre mí / Contacto` con scroll suave + offset. Activa con subrayado `{colors.primary}`. Rueda / trackpad / táctil nativo.
- **Menú móvil:** botón `Menú`. Panel negro desde arriba ~220ms, enlaces grandes + `Cerrar`. Cierra con opción / `Cerrar` / `Escape`. Foco atrapado dentro, fondo bloqueado, retorno de foco al botón.
- **Botones:** primario `{components.button-primary}` — fondo `{colors.primary}`, texto negro, hover `{colors.primary-hover}` 180ms, press scale 0.98. Secundario `{components.button-secondary}` — transparente → claro con texto negro en hover. `Ver proyectos` → galería, `Contacto` → contacto. Foco visible siempre.
- **Enlaces:** subrayado visible. Nunca solo color.
- **Tarjetas de proyecto:** son enlaces. Hover: imagen ×1.08 en 220ms dentro de contenedor con `overflow:hidden` + subrayado de título + intercambio de imagen tipo hall-of-fame cuando haya hover; salida suave. Enter abre con foco. Nombre + disciplina siempre visibles, también en táctil.
- **Filtros:** `Todos / Identidad / Social / Editorial / Motion` (solo si hay volumen). Filtrado sin recarga, 180ms, subrayado rojo + `aria-pressed` / `aria-selected`. Sin robo de foco ni saltos. En móvil en varias líneas.
- **Galería / lightbox:** fondo negro, `Cerrar / Anterior / Siguiente` + contador. Flechas de teclado, `Escape` cierra, swipe en móvil con botones siempre visibles. Foco atrapado, retorno a la imagen origen. Sin recortes obligatorios.
- **Video:** portada + `Reproducir`. Controles nativos (play / pausa / volumen / seek / fullscreen). Subtítulos si hay diálogo. Vista previa muda en autoplay permitida en tarjetas y portada (se pausa fuera de pantalla y con `reduced-motion`). Sonido solo cuando el usuario lo activa.
- **Reveal on scroll + parallax + horizontal:** una sola vez para textos, 350ms + translateY ≤16px, stagger 60ms máx 180ms. Además: parallax entre LOWUIS/foto por scroll, franja IMPACTO/DOMINIO/DRAMA en marquee ligado a scroll, título de galería fijo por tramo y pista horizontal que avanza con el scroll vertical (estilo Lando).
- **Contacto:** email `mailto:` visible + `Copiar correo` → `Correo copiado` (fallback: seleccionar manualmente). Sociales solo confirmados, en pestaña nueva. `Descargar CV (PDF)` solo si existe el archivo.
- **Formulario (opcional):** labels siempre visibles, borde de foco destacado, `Enviar` → `Enviando` + disabled anti-doble, errores junto al campo conservando datos, reintento explicado, éxito solo con confirmación real.
- [REVISAR] estados disabled / error / éxito de campos, textos exactos de mensajes y endpoint del formulario no definidos.

## Do's and Don'ts

**Sí**

- Mantener `{colors.primary}` como firma; secundarios selectivos.
- Un punto focal por pantalla con escala y contraste.
- Conservar paletas y proporciones originales de proyectos.
- Titulares condensados pesados + lectura clara.
- Controles accesibles: teclado, foco visible, contraste, targets 44px.
- Mostrar participación real y contexto por proyecto.

**No**

- No juntar todos los saturados en una sección.
- No inventar experiencia, clientes, resultados ni datos de CV.
- Intro breve permitida (loader máx 1.2s, saltable). Sin destellos fuertes ni sonido automático.
- Hover puede revelar “Explorar proyecto” y previews mudas; la info esencial (nombre + disciplina) siempre visible.
- No deformar tipos ni encoger texto para forzar composición.
- No repetir tarjetas idénticas ni efectos sin propósito.
