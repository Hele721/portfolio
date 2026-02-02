PROMPT (original):
Teniendo en cuenta mis líneas de diseño y decisiones técnicas descritas en `project-brief.md` y `project-inspiration.md` (y respetando los tokens de `assets/css/_variables.css`), analiza estos 5 portfolios de ilustradores [https://ning-h.com/
https://www.kasiasiwosz.com/
https://www.olhalazarieva.com/
https://www.julesstudio.co/
https://studiopuntocero.com/concursos/].

## Volcado de entrega (archivos destino)

- `docs/prompt-analisis-galerias.md`: pega este prompt + la respuesta completa.
- `project-inspiration.md`: añade las 3 URLs analizadas y 3 bullets de “patrones transferibles” (sin copiar).
- `project-brief.md`: incorpora 2 decisiones concretas (layout + contenido) en Key Sections / Design Direction.

Objetivo pedagógico: detectar **patrones transferibles** (no copiar estética).

Para cada uno, evalúa:

1. **Diseño Visual (Awwwards criteria)**

   - Estética general (1-10)
   - Tipografía y jerarquía
   - Uso de color y contraste
   - Composición y espaciado

2. **UX de Galería**

   - Facilidad para explorar proyectos
   - Claridad de navegación
   - Información por proyecto (título, descripción, tags)
   - Call-to-actions efectivos

3. **Técnica**

   - Tipo de layout (grid, masonry, custom)
   - Responsive behavior
   - Performance (carga de imágenes)
   - Micro-interacciones

4. **Insights Accionables (aplicables a mi brief)**
   - 3 patrones que puedo reutilizar sin copiar (con explicación)
   - 3 riesgos/antipatrones a evitar (con explicación)
   - 2 decisiones concretas para mi galería (layout + contenido), justificadas con mi `project-brief.md`

Devuelve:

- Tabla comparativa (Diseño / UX / Técnica)
- “Decisiones para mi proyecto” (bullets)
- Checklist de verificación (qué revisar al implementarlo)


RESPUESTA:

Resumen rápido
- Alcance: evalué los cinco sitios y extraje patrones transferibles orientados a portfolios ilustrativos y editoriales.
- Restricciones técnicas: respetar tokens en `assets/css/_variables.css` (escala de espacios, paleta neutra/primaria, tipografías, etc.) y objetivos del `project-brief.md` (audiencia editorial, accesibilidad, responsive, performance).

Análisis por sitio

1) https://ning-h.com/
- Diseño Visual (Awwwards)
  - Estética general: 8/10 — minimal, experimental, foco en motion y composición.
  - Tipografía y jerarquía: uso de escalas grandes y espaciados extremos; jerarquía clara entre títulos y captions.
  - Uso de color y contraste: paleta muy neutra con acentos en imágenes; buen contraste para texto principal.
  - Composición y espaciado: generoso uso de whitespace y secciones con alineaciones asimétricas.
- UX de Galería
  - Facilidad para explorar: alta — el contenido se presenta en bloques visuales grandes; navegación por scroll clara.
  - Claridad de navegación: simple, anchoring en proyectos; menú compacto.
  - Información por proyecto: mínima — grandes imágenes, poco texto; título y link a caso.
  - Call-to-actions: escasos; foco en visualización más que conversión.
- Técnica
  - Tipo de layout: grid/columnas adaptadas con detalles de custom layout y animaciones basadas en transform/clip-path.
  - Responsive behavior: bien adaptado, prioritiza mobile-first con reconstrucción visual en desktop.
  - Performance: riesgo por imágenes pesadas y animaciones; probable uso de AVIF/WebP para optimizar.
  - Micro-interactions: hover/scroll-triggered motion sutil, buen ritmo.
- Insights accionables
  - Patrones reutilizables: foco en imágenes grandes; entradas con short-read; transiciones suaves al entrar en vista.
  - Riesgos a evitar: exceso de motion que sacrifique accesibilidad y performance; falta de metadatos en tarjetas.
  - Decisión aplicable: destacar 1-2 proyectos hero con visual grande en la home; thumbnails optimizados con lazy-loading.

2) https://www.kasiasiwosz.com/ (no es ilustrador; ejemplo de diseño orientado a conversión)
- Diseño Visual
  - Estética general: 7/10 — tipográfico, editorial, orientado a confianza y autoridad.
  - Tipografía y jerarquía: tipografía muy cuidada; bloques de texto con claro ritmo editorial.
  - Uso de color y contraste: paleta sobria, contrastes pensados para lectura.
  - Composición y espaciado: estructura en secciones amplias, lectura cómoda.
- UX de Galería (ajuste: site de servicios)
  - Facilidad para explorar: alta en contenido textual; no es galería visual tradicional.
  - Claridad de navegación: excelente, CTAs claros para booking/contact.
  - Información por proyecto: si hubiera casos, serían detallados; aquí el modelo es textual.
  - Call-to-actions: muy efectivos (book/contacts).
- Técnica
  - Tipo de layout: layout de contenido fluido, bloques responsivos.
  - Responsive behavior: orientado a lectura en móviles y escritorio.
  - Performance: buena práctica en optimización de texto; imágenes complementarias.
  - Micro-interactions: CTAs y link hover discretos.
- Insights accionables
  - Patrones reutilizables: copy editorial para casos; CTAs claros y visibles.
  - Riesgos: convertir un portfolio visual en un sitio demasiado textual; perder foco en imágenes.
  - Decisión aplicable: incluir una introducción editorial clara encima de la galería para contexto profesional.

3) https://www.olhalazarieva.com/
- Diseño Visual
  - Estética general: 8/10 — minimal, tipografía cuantificada, aspecto profesional y editorial.
  - Tipografía y jerarquía: uso efectivo de tipografía grande para headings y un sistema claro para secciones.
  - Uso de color y contraste: paleta neutra; contraste suficiente; imágenes con tratamiento consistente.
  - Composición y espaciado: diseño modular, ritmo constante entre secciones.
- UX de Galería
  - Facilidad para explorar: buena — slider/carousel para trabajos recientes, y enlaces a casos.
  - Claridad de navegación: clara, secciones definidas; el usuario entiende dónde están los casos.
  - Información por proyecto: título + breve excerpt + enlace a case study.
  - Call-to-actions: presentes (view case / contact), dirección clara a casos.
- Técnica
  - Tipo de layout: grid + slider; enfoque clásico con progressive enhancement.
  - Responsive behavior: sólido; el slider se vuelve stack en móvil.
  - Performance: uso de JPG/WEBP; buen balance entre imágenes y texto; posible lazy-loading.
  - Micro-interactions: animaciones tipográficas y transiciones limpias.
- Insights accionables
  - Patrones reutilizables: combinar grid y slider para “destacados” + tarjetas con excerpt.
  - Riesgos: slider sin fallback de accesibilidad; exceso de texto en mobile.
  - Decisión aplicable: tener sección "Trabajos recientes" como slider horizontal y galería principal en grid.

4) https://www.julesstudio.co/
- Diseño Visual
  - Estética general: 7/10 — profesional, corporativo ligero; estilo estudio/servicio.
  - Tipografía y jerarquía: clara y funcional; títulos y subtítulos bien diferenciados.
  - Uso de color y contraste: paleta con acentos de marca; buen contraste en CTAs.
  - Composición y espaciado: modular y limpio, bastante whitespace.
- UX de Galería
  - Facilidad para explorar: buena — sección de trabajo con cards y enlaces a casos.
  - Claridad de navegación: muy buena, con CTAs orientados a conversión (Book a call).
  - Información por proyecto: cards con etiquetas, tipo de trabajo y enlace a detalle.
  - Call-to-actions: fuertes y orientados a negocio.
- Técnica
  - Tipo de layout: grid de tarjetas con imágenes; enfoque clásico y accesible.
  - Responsive behavior: robusto; probable uso de CMS/Webflow con imágenes responsivas.
  - Performance: optimizada (AVIF/WEBP), imágenes con atributos srcset.
  - Micro-interactions: hover y micro-animaciones en cards.
- Insights accionables
  - Patrones reutilizables: tarjetas con meta (categoría, rol), CTAs orientadas a contacto; uso de logos de clientes como prueba social.
  - Riesgos: priorizar CTAs comerciales sobre la narrativa visual de proyectos.
  - Decisión aplicable: añadir meta etiquetas en cada tarjeta (rol, disciplina) y CTA "Ver caso".

5) https://studiopuntocero.com/concursos/ (estudio de arquitectura)
- Diseño Visual
  - Estética general: 7/10 — editorial y profesional, orientado a proyectos arquitectónicos.
  - Tipografía y jerarquía: clara, con labels para proyectos y extractos.
  - Uso de color y contraste: neutro; imágenes arquitectónicas dominan la paleta.
  - Composición y espaciado: rejilla de proyectos con separadores y excerpt.
- UX de Galería
  - Facilidad para explorar: buena — listado con enlaces por proyecto; cada item es clicable.
  - Claridad de navegación: clara; breadcrumb y categorías.
  - Información por proyecto: título + excerpt + enlace; imágenes preview.
  - Call-to-actions: foco en proyecto individual y contacto.
- Técnica
  - Tipo de layout: grid/listado con enlaces a cada proyecto.
  - Responsive behavior: sólido; estructuras típicas de WP adaptadas.
  - Performance: depende de imágenes; uso de thumbnails.
  - Micro-interactions: modestos, focus en contenido estático.
- Insights accionables
  - Patrones reutilizables: entradas listadas con excerpt y link directo; uso de categorías/filtrado por tipo.
  - Riesgos: no mostrar suficientes previews visuales en thumbnail pequeños; perder impacto.
  - Decisión aplicable: implementar filtrado por tipo/tags y thumbnails de mayor tamaño.

Tabla comparativa (Diseño / UX / Técnica)

| Sitio | Diseño (estética/jerarquía/espacio) | UX Galería (explorar/info/CTAs) | Técnica (layout/responsive/perf) |
|---|---:|---:|---:|
| ning-h.com | 8 — experimental, gran uso de whitespace y motion | 8 — navegación por scroll, foco visual fuerte | 7 — custom layouts, requiere optimización de imágenes |
| kasiasiwosz.com | 7 — editorial, tipografía muy cuidada | 8 — CTAs claros, orientado a conversión (no galería) | 8 — texto-first, ligero en imágenes |
| olha… | 8 — minimal profesional, tipografía fuerte | 8 — slider + grid, buen acceso a casos | 8 — balance imágenes/texto, accesible si se implementa bien |
| julesstudio.co | 7 — studio-professional, limpio | 8 — cards con meta y CTAs fuertes | 8 — probable uso de CMS con imágenes responsivas |
| studiopuntocero | 7 — editorial arquitectónico | 7 — listado claro, categorías | 7 — WP-based, depende de optimización de assets |

Insights accionables (aplicables a tu brief)

3 patrones reutilizables (sin copiar estética)
- 1) Jerarquía visual con "hero projects": una o dos piezas destacadas en la home con imagen grande y enlace a case study. Explicación: atraen la atención del reclutador editorial y permiten mostrar proceso + resultado rápido.
- 2) Tarjetas enriquecidas con metadatos: título, tipo (editorial/ilustración), año/cliente y 2-3 tags. Explicación: facilita filtrado y permite que quien revisa identifique experiencia relevante rápidamente.
- 3) Progressive gallery: grid responsivo + un carrusel/slider para "recientes" o "destacados". Explicación: combina escaneo rápido (grid) con narrativa secuencial (slider) para proyectos que necesitan contexto.

3 riesgos / antipatrones a evitar
- 1) Exceso de motion sin controles de accesibilidad: puede provocar problemas para usuarios con vestibular o disminuir performance.
- 2) Thumbnails demasiado pequeños o comprimidos: reducen el impacto visual de ilustraciones; usar previews grandes y crop controlado.
- 3) Falta de contexto en cada proyecto: imágenes sin título/rol/brief obligan a adivinar tu aportación; siempre añadir 1-2 líneas de contexto.

2 decisiones concretas para tu galería (layout + contenido)
- Decision (layout): Grid responsivo con tres breakpoints — mobile (1 col), tablet (2 cols), desktop (3 cols) + un hero strip en top con 1 proyecto destacado (imagen grande). Justificación: respeta la estrategia mobile-first, permite mostrar trabajos en tamaño editorial y se alinea con tokens de spacing y max-width en `assets/css/_variables.css`.
- Decision (contenido por tarjeta): cada tarjeta incluirá: imagen (cover), título, rol breve (ej. "Ilustración editorial — revista X, 2024"), 2 tags (estilo/tema), y CTA "Ver caso" que abre case minimal con 1 párrafo de contexto, galería de imágenes optimizadas y créditos. Justificación: orientado a empresas editoriales que necesitan entender rápidamente encaje profesional y ver evidencia visual.

Checklist de verificación (qué revisar al implementarlo)
- Estructura y tokens
  - [ ] Usar variables de `assets/css/_variables.css` para espaciado, tipografía y colores (no hardcodear valores).
  - [ ] Mantener --max-width y --container-padding para constancia editorial.
- Accesibilidad
  - [ ] Alt en todas las imágenes; textos de enlace comprensibles (no sólo "click here").
  - [ ] Controles para motion (reduce-motion), y pausa/stop para animaciones importantes.
  - [ ] Contrastes de texto >= WCAG AA (usar --color-text-* tokens).
  - [ ] Navegación por teclado en galería y en modal/case views.
- Performance
  - [ ] Thumbnails en WebP/AVIF con srcset; lazy-loading nativa (loading="lazy").
  - [ ] Dimensiones en HTML para evitar layout shift (width/height o aspect-ratio).
  - [ ] Minimizar JS para animaciones; preferir transform/opacity.
- UX / Content
  - [ ] Tarjeta muestra título, rol breve y tags legibles en mobile.
  - [ ] CTA "Ver caso" visible y consistente; fallback a página si JS falla.
  - [ ] Filtrado por tags/categorías implementado progresivamente.
- QA y pruebas
  - [ ] Probar en móvil, tablet y desktop; chequear breakpoints definidos.
  - [ ] Lighthouse audit (performance, accessibility, best practices) — objetivo 90+ en accesibilidad y performance > 80.
  - [ ] Revisar carga desde conexiones lentas (3G throttling).

Decisiones para mi proyecto (resumen corto para implementar)
- Layout: Grid responsive (1/2/3 columnas) + hero project destacado en la parte superior.
- Contenido: Tarjeta con cover, título, rol breve, 2 tags y CTA "Ver caso" que abre case con contexto, galería optimizada y créditos.

---

Fin de la respuesta. Si quieres, puedo:
- Pegar esta misma respuesta dentro de `project-inspiration.md` y `project-brief.md` (ya puedo hacerlo).
- Generar los componentes HTML/CSS para la galería respetando `assets/css/_variables.css`.
- Crear un prototipo Figma simple (exportable) con las decisiones mencionadas.

