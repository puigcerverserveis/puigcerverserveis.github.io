# AGENT RUNBOOK

## Git y entregas
- Antes de ejecutar `git add`, `git commit` o `git push`, confirma con el usuario y ejecuta los tres pasos seguidos si lo autoriza.
- Flujo sugerido tras OK del usuario: `git status` → `git add -A` → `git commit -m "chore: update landing content"` (ajusta mensaje) → `git push`.
- No reverta cambios ajenos ni use comandos destructivos; si el repo esta sucio, respete cambios existentes.

## Contexto del proyecto
- Web estatica GitHub Pages para Grupo Puigcerver: servicios generales vivienda/local.
- Idiomas: ES/EN/FR/CA mediante `data-i18n` en `index.html`.
- Contacto: tel +34 672 737 607; email `grupopuigcerver@gmail.com`; WhatsApp `https://wa.me/34672737607`.
- Urgencias: radio aprox. 1h (~60 km) desde Valles Occidental hacia Barcelones; fuera de radio, visita concertada/pago previo.

## Estilo y edicion
- Usar ASCII; evitar caracteres especiales y tildes en codigo si no son necesarios.
- Mantener CTA y mensajes prellenados coherentes en los 4 idiomas.
- No añadir librerias ni dependencias; mantener HTML/CSS/JS plano.

## Validaciones rapidas
- Previsualizar local: `python -m http.server 8000` y abrir `http://localhost:8000`.
- Revisar que selector de idioma actualiza textos y enlaces de WhatsApp.
