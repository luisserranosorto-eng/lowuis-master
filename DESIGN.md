---
name: Lowuis — Sistema de diseño
designer: Luis Eduardo Sorto
description: Sistema visual aplicado al portafolio publicado de diseño gráfico y creación audiovisual.
source: Design_luis.docx
last_updated: 2026-10-19
---

# Sistema de diseño Lowuis

Este documento describe el sistema visual que se aplica al portafolio publicado. Es la referencia para mantener coherencia entre la página principal, las fichas de proyecto y las versiones de escritorio y móvil.

## Identidad visual

Lowuis combina una base oscura con rojo intenso, tipografía a gran escala y fotografía o video de alto contraste. La firma LOWUIS funciona como un gesto editorial. El sitio alterna momentos de impacto visual con bloques de lectura breve para dejar que cada proyecto conserve su propia personalidad.

El tono es directo y cinematográfico. El rojo organiza la navegación, las acciones y los acentos; no se utiliza como filtro global sobre el trabajo.

## Color

| Rol | Valor | Uso |
| --- | --- | --- |
| Rojo principal | `#FF2028` | Acciones, titulares de énfasis, indicadores y franjas de tarjetas. |
| Negro | `#000000` | Fondo profundo y contraste. |
| Carbón | `#101010` | Fondo predominante de interfaz. |
| Blanco cálido | `#F4F0E8` | Texto principal sobre fondo oscuro. |
| Gris | `#B8B4AE` | Texto secundario e información auxiliar. |

Azul, lima, amarillo, naranja, magenta, violeta y cian pertenecen a las piezas de proyecto. Se usan cuando el proyecto lo requiere, no como colores fijos de la interfaz.

### Reglas de color

- Cada sección parte de neutros y usa un acento dominante cuando hace falta.
- Las categorías se escriben siempre como texto; el color no es el único indicador.
- Se conservan las paletas originales de Apple, BIG HERO, Marty Supreme, MALA FE, GALA OBSESSION y el resto de los proyectos.
- El texto mantiene contraste suficiente sobre imágenes y video mediante zonas de lectura, fondos o sombras sutiles.

## Tipografía

La familia principal es **Barlow**. Se usa para lectura, navegación, etiquetas, botones y titulares sans serif, principalmente en sus pesos Bold y ExtraBold.

**Manufacturing Consent** se reserva para la firma LOWUIS, HOLA y acentos editoriales. **Ballet** funciona como recurso expresivo puntual. Ninguna de las dos sustituye a Barlow como tipografía de interfaz o de lectura.

| Uso | Familia y tratamiento |
| --- | --- |
| Firma y acento editorial | Manufacturing Consent, tamaño expresivo. |
| Titulares | Barlow ExtraBold, mayúsculas cuando la composición lo pide. |
| Subtítulos y acciones | Barlow SemiBold o Bold. |
| Lectura | Barlow Regular o Medium. |
| Información secundaria | Barlow Regular en gris. |

Los titulares usan escalas fluidas para mantener jerarquía en escritorio y móvil. El texto se adapta al contenedor y no se fuerza fuera de la pantalla.

## Retícula y composición

El sitio trabaja con un ancho amplio y márgenes que se reducen de forma progresiva en tabletas y móviles. La navegación puede ocupar una retícula más abierta que el contenido para quedar cerca de las esquinas sin perder aire.

- Las galerías de proyecto usan una, dos o tres columnas según la pieza y el ancho disponible.
- Apple organiza seis imágenes verticales en dos filas de tres columnas en escritorio; su video se presenta debajo, centrado y con el mismo ancho de una pieza de la retícula.
- MALA FE y GALA OBSESSION agrupan formatos horizontales, verticales y carteles sin deformarlos.
- Marty Supreme intercala piezas a tres columnas con imágenes de ancho completo para marcar ritmo.
- Las imágenes conservan su proporción; se usa `object-fit` sólo cuando una composición requiere recorte controlado.

En móvil, la lectura pasa a una secuencia vertical. Se preservan márgenes, jerarquía tipográfica y relación de aspecto, evitando desplazamiento horizontal.

## Componentes

### Navegación

La cabecera es fija y transparente, con desenfoque para mantener legibilidad sobre el contenido. El nombre **Luis Sorto.** conduce al inicio. En pantallas pequeñas aparece el botón **Menú**, que muestra los enlaces de Inicio, Sobre mí, Habilidades, Proyectos y Contacto.

### Tarjetas de proyecto

Las tarjetas muestran siempre nombre y disciplina. Las piezas audiovisuales pueden mostrar una vista previa silenciosa y cuentan con respaldo visual mientras cargan. Las tarjetas enlazan a una ficha independiente de cada proyecto.

### Videos

Apple, BIG HERO y Marty Supreme tienen una pieza principal al entrar en su ficha y un video adicional al final con controles visibles. El sonido se intenta activar en la pieza principal cuando el navegador lo permite; los controles de reproducción, línea de tiempo y volumen quedan disponibles para la persona usuaria. Las vistas previas y videos secundarios se mantienen sin sonido.

### Contacto

El bloque de contacto usa una frase editorial, correo visible, botón **Escríbeme**, control de copiado con respuesta temporal, enlace a Instagram y **Volver arriba**. No se añaden formularios ni datos no confirmados.

## Movimiento y rendimiento

Las entradas por scroll son cortas y usan desplazamientos reducidos. La galería visual final revela piezas progresivamente; las imágenes prioritarias se preparan antes de entrar en pantalla para evitar huecos de carga.

Los videos secundarios se cargan al acercarse a la sección. La experiencia respeta `prefers-reduced-motion`: se reduce el movimiento y el contenido continúa disponible sin depender de la animación.

## Accesibilidad y adaptación

- Controles con áreas táctiles cómodas, texto visible y foco de teclado.
- Etiquetas y categorías legibles sin depender sólo del color.
- Imágenes y videos con texto alternativo o etiqueta contextual según su uso.
- Interfaz adaptable a escritorio, tableta y móvil sin desbordes horizontales deliberados.
- Contenido esencial accesible aun cuando las animaciones no se reproduzcan.

## Reglas de uso

**Sí**

- Usar el rojo como firma y acento de interacción.
- Mantener fondos oscuros, alto contraste y esquinas rectas.
- Conservar proporciones y paletas propias de cada proyecto.
- Dar protagonismo a la tipografía y a los medios audiovisuales.

**No**

- No deformar imágenes ni comprimir texto para forzar una composición.
- No añadir efectos, formularios, redes o información que no existan en el sitio.
- No reemplazar las categorías textuales por color o iconos solamente.
- No convertir el rojo en un filtro que borre la identidad de los proyectos.
