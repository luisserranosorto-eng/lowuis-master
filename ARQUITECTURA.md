---
name: Lowuis — Arquitectura del portafolio
designer: Luis Eduardo Sorto
description: Estructura y comportamiento del portafolio publicado.
source: Arquitectura-CV.docx
last_updated: 2026-10-19
---

# Arquitectura del portafolio Lowuis

Este documento describe la arquitectura del portafolio publicado: una página principal con fichas independientes para cada proyecto.

## Estructura principal

- **Inicio:** portada LOWUIS con el perfil de diseñador gráfico y creador audiovisual.
- **Sobre mí:** retrato, presentación de Luis Sorto y una selección visual en movimiento.
- **Habilidades:** mensaje de capacidades, diseño de empaque, diseño de campañas, software y galería visual.
- **Proyectos:** filtros por Todos, Identidad, Editorial, Audiovisual, Modelado 3D y Empaque.
- **Contacto:** frase editorial, correo, botón Escribeme, control de copiado, Instagram y Volver arriba.

## Navegación

La cabecera permanece visible sobre el contenido. **Luis Sorto.** dirige al inicio y, en pantallas pequeñas, el botón **Menú** abre los enlaces de navegación. El desplazamiento entre secciones es suave y contempla la altura de la cabecera fija.

## Inicio y presentación

La portada ocupa la altura disponible y presenta LOWUIS, Portafolio y las líneas de perfil. Una franja tipográfica y transiciones visuales conectan la entrada con Sobre mí. El retrato HOLA combina fotografía y texto adaptable: en escritorio el contenido se sitúa a la derecha del personaje y en móvil se recompone para conservar legibilidad.

## Habilidades y contenido visual

La sección reúne el mensaje **Proyectos que impactan**, habilidades de dirección creativa, diseño y producción, y un bloque de softwares. La galería posterior utiliza imágenes y videos de distintos proyectos como composición audiovisual. Las piezas visibles al inicio se preparan para reducir sus tiempos de aparición.

## Proyectos

La galería principal incluye Apple, BIG HERO, Marty Supreme, MALA FE, GALA OBSESSION, Siza, El Ágora, Prozine, Raid, Inspira Kleenex, Johnnie Walker Ruby Stand y Johnnie Walker Ruby Personaje. Cada tarjeta conserva nombre y disciplina. Los filtros reorganizan las tarjetas sin recargar la página. Las miniaturas de video permanecen silenciosas y tienen una imagen de respaldo durante la carga.

## Fichas de proyecto

Cada tarjeta abre `proyecto.html` con el identificador del proyecto. La ficha incluye portada, categoría, contexto cuando existe, galería de imágenes y videos, y un enlace para volver a Proyectos.

Apple, BIG HERO y Marty Supreme incluyen reproducción principal y un video final con controles. Raid e Inspira Kleenex agrupan primero las piezas de empaque y después los desplegables. Los proyectos Johnnie Walker documentan un stand y un personaje dentro de Modelado 3D. Las galerías respetan las proporciones originales de cada pieza y se ajustan por proyecto.

## Comportamiento responsive

El sitio usa consultas de medios para reorganizar retículas, tipografía, navegación y galerías. En móvil se prioriza una lectura vertical sin desplazamiento horizontal deliberado. La navegación, los enlaces y los controles de video permanecen utilizables en pantallas táctiles.

## Rendimiento y accesibilidad

Las imágenes fuera de la primera pantalla usan carga progresiva cuando corresponde. Las piezas críticas de las composiciones finales se preparan antes de entrar en pantalla. Los controles conservan texto visible, tamaños táctiles, foco de teclado y una alternativa de movimiento reducido.
