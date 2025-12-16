# Grupo Puigcerver - embudo web local

Web estatica en GitHub Pages para Grupo Puigcerver (servicios generales para vivienda y pequeno local), orientada a contacto directo y contenidos territoriales sin spam.

## Estructura base
- `index.html`: landing principal con CTA a telefono y WhatsApp.
- `style.css`: estilos basicos con variables listas para iterar diseno.
- `blog/`: articulos por zona (barrio, calle, urbanizacion, nucleo pequeno).
- `assets/img/`: imagenes por articulo (prompts en `TASKS.md`, no generadas aun).
- `TASKS.md`: plan de tareas de infraestructura, contenidos y escalado.

## CTA y mensaje estandar
- Llamada directa: `tel:+34672737607`.
- WhatsApp: `https://wa.me/34672737607?text=Hola%20Grupo%20Puigcerver%2C%20tengo%20un%20problema%20en%20[describe]%20en%20[zona]%20con%20urgencia%20[alta/media/baja].`
- Snippet de respuesta rapida sugerido: "Gracias por escribir a Grupo Puigcerver. Para ayudarle rapido: 1) Que ocurre, 2) Direccion o zona, 3) Urgencia (hoy / 48h / programar)."

## Foco territorial
- Prioridad: norte de Rubi y zonas con menor competencia.
- Cada articulo debe mencionar la zona, problemas habituales y enlazar a zonas cercanas y a la landing.

## Flujo de trabajo rapido
1) Clonar el repo y leer `TASKS.md`.
2) Editar HTML/CSS manteniendo rutas relativas para Pages.
3) Previsualizar local: `python -m http.server 8000` y abrir `http://localhost:8000`.
4) Deploy: push a `main`; GitHub Pages publica desde la raiz. Anadir `.github/workflows/pages.yml` si falta para despliegue automatico.

## Mejora y escalado (detalle en `TASKS.md`)
- Diseno: iterar colores y tipografia via variables en `style.css`.
- Contenido: publicar 3-5 articulos semilla y ampliar con zonas/urbanizaciones.
- Medicion y formularios: placeholders listos; anadir GA/Plausible y formulario cuando se apruebe.
- Campanas: preparar base para conectar Google Ads y landings especificas sin postureo ni spam.
