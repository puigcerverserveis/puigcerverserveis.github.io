# Plan de tareas – Grupo Puigcerver

## 0. Arranque y criterios
- [ ] Confirmar tono: profesional, neutro, sin claims agresivos ni “24h barato”.
- [ ] Dejar claro foco territorial: norte de Rubí y zonas con menor competencia.
- [ ] Definir owner de ejecución y ritmo (diario/semanal) para publicar artículos locales.

## 1. Infraestructura base (GitHub Pages)
- [ ] Crear repo `puigcerverserveis.github.io` en GitHub (si no existe) y habilitar Pages desde `main`.
- [ ] Estructura mínima en raíz: `index.html`, `style.css`, `blog/`, `assets/`, `assets/img/`.
- [ ] Añadir `.github/workflows/pages.yml` (deploy automático de Pages) y verificación manual post-deploy.
- [ ] Incluir README con instrucciones de edición y previsualización local (simple `python -m http.server`).

## 2. Web principal (landing básica)
- [ ] Diseñar landing de una sola página (HTML+CSS sin framework) con bloques: hero, servicios genéricos, zona de trabajo, llamada a la acción.
- [ ] Redactar copy neutro: “Servicios generales para vivienda y pequeño local. Mantenimiento, reparaciones y soluciones técnicas sin encasillarnos en un gremio.”
- [ ] Botones visibles y repetidos (hero + footer):
  - [ ] Llamada directa `tel:+34672737607`.
  - [ ] WhatsApp con mensaje pre-rellenado: `https://wa.me/34672737607?text=Hola%20Grupo%20Puigcerver%2C%20tengo%20un%20problema%20en%20[describe]%20en%20[zona]%20con%20urgencia%20[alta/media/baja].`
- [ ] Sección “Zona de trabajo”: destacar norte de Rubí, urbanizaciones y calles con menor competencia; invitar a consultar si la zona no aparece.
- [ ] Footer con datos de contacto (tel, WhatsApp, email genérico si se quiere), enlace a GBP cuando esté disponible.

## 3. Automatización básica (WhatsApp)
- [ ] Definir mensaje estándar de filtro (Qué ocurre / Zona / Urgencia) y usarlo en CTA y respuestas rápidas.
- [ ] Crear snippet de respuesta rápida interno para WhatsApp Business: “Gracias por escribir a Grupo Puigcerver. Para ayudarle rápido: 1) Qué ocurre, 2) Dirección o zona, 3) Urgencia (hoy / 48h / programar).”
- [ ] Documentar en README el flujo de atención (quién responde, horarios, derivaciones).
- [ ] Dejar placeholders para futuras integraciones (formularios, CRM ligero) sin implementarlas todavía.

## 4. Contenidos territoriales (blog)
- [ ] Crear plantilla de artículo en `blog/` (HTML sencillo) con bloques: título, intro corta, problemas habituales, soluciones posibles, CTA a WhatsApp/tel, enlaces a zonas cercanas.
- [ ] Definir taxonomía: un artículo por barrio, calle relevante, zona interurbana, urbanización y núcleo pequeño con poca oferta.
- [ ] Generar listado inicial (15–30) de zonas priorizadas: norte de Rubí primero; añadir calles/urbanizaciones con baja competencia.
- [ ] Redactar 3–5 artículos semilla: ejemplos “Servicios de mantenimiento en [Zona X]”, “Problemas habituales en viviendas de [Barrio Y]”, “Soluciones técnicas para casas en [Zona interurbana Z]”.
- [ ] Incluir CTA en cada artículo con el mensaje WhatsApp pre-rellenado y enlace a la landing.
- [ ] Añadir navegación interna: enlaces a 2–3 zonas cercanas y retorno a landing.

## 5. SEO básico sin spam
- [ ] URLs limpias: `blog/servicios-mantenimiento-zona-x.html` (guiones, minúsculas).
- [ ] Títulos naturales y únicos; H1 claro y un H2 para “Problemas habituales” y otro para “Cómo los resolvemos”.
- [ ] Meta description sencilla (120–155 chars) describiendo zona y servicio; sin keyword stuffing.
- [ ] Open Graph básico (title, description) reutilizando el texto de la página.
- [ ] Sitemap simple (manual o generado) y `robots.txt` permitiendo indexación de blog y landing.
- [ ] Enlazado interno: cada artículo enlaza a zonas cercanas y a la landing; landing enlaza a 4–6 artículos clave.

## 6. Contenido visual (no ejecutar, dejar prompt)
- [ ] Definir prompt tipo para Nano-Banana (1 por artículo), imagen neutra y técnica:
  - Prompt sugerido: `Neutral technical photo of a residential building facade and maintenance tools, suburban Spanish neighborhood in [Zona], daytime, clean composition, no text, professional reportage style`.
- [ ] Guardar imágenes en `assets/img/[zona].jpg` y referenciarlas en cada artículo.
- [ ] Mantener peso ligero (web), compresión previa y atributo `alt` descriptivo.

## 7. Publicación y QA
- [ ] Probar vista local (desktop y móvil), verificar CTAs de tel/WhatsApp.
- [ ] Revisar ortografía y coherencia territorial (nombres de zonas correctos).
- [ ] Comprobar que todas las rutas relativas funcionan en GitHub Pages (sin rutas absolutas).
- [ ] Deploy a Pages y chequeo manual de caché/propagación.

## 8. Escalabilidad y futuras mejoras
- [ ] Diseño: preparar `style.css` con variables (colores, tipografía) para iterar fácilmente sin tocar HTML.
- [ ] Formularios: planificar `contacto.html` y `form` básico que envíe a email/Sheets/Make (futuro).
- [ ] Medición: añadir Google Analytics/GA4 o Plausible cuando se apruebe.
- [ ] Campañas: dejar sección en README con pasos para conectar Google Ads (tracking, conversiones, landings específicas).
- [ ] Catálogo de servicios: futura página “casos resueltos” con fotos y descripción corta (sin postureo).
- [ ] Scripts de generación: plantear generación de artículos desde CSV/JSON de zonas (a futuro) para escalar sin spam.

## 9. Checklist operativo (orden sugerido)
- [ ] Crear repo + activar Pages.
- [ ] Subir estructura mínima y workflow de deploy.
- [ ] Escribir landing con CTAs tel/WhatsApp y zona de trabajo.
- [ ] Documentar mensaje de filtro y snippet de respuesta rápida.
- [ ] Publicar 3–5 artículos semilla con interlinking y CTA.
- [ ] Preparar prompts de imágenes y placeholders en artículos.
- [ ] QA local + móvil; desplegar; validar enlaces y meta.
- [ ] Planificar siguiente batch de artículos por zonas/urbanizaciones.
