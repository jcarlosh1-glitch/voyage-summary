# Instrucciones para Claude en este repositorio

## Herramientas que hay que usar cuando hagan falta

Lista sacada del vídeo "5 MCP servers every Claude Code user needs right now" (InsiderForce,
https://youtube.com/shorts/aX7QAfld7hs). Para cada una, qué usar en estas sesiones en la nube:

1. **Búsqueda en internet en tiempo real** (en el vídeo: Perplexity MCP).
   Usar la búsqueda web (WebSearch) para datos actuales: precios, puertos, normas, novedades.
   No responder de memoria cuando el dato puede haber cambiado.
2. **Controlar un navegador** (en el vídeo: Playwright MCP).
   Playwright y Chromium ya están instalados en el contenedor. Usarlos para abrir la app,
   pulsar botones, rellenar formularios y hacer capturas antes de dar un cambio por bueno.
3. **Leer una página web entera y limpia** (en el vídeo: Firecrawl MCP).
   Usar el agente web-fetch con la URL y la pregunta. Si el sitio bloquea la lectura
   automática, decirlo y no inventar el contenido.
4. **Generar imágenes y vídeos** (en el vídeo: Higgsfield MCP).
   Higgsfield está conectado en esta cuenta. Usarlo cuando se pida una imagen o un vídeo,
   dando antes el coste estimado en créditos.
5. **Ver y manejar el Chrome del usuario** (en el vídeo: Chrome DevTools MCP).
   Equivalente: Claude in Chrome (skill chrome-browser). Solo funciona con el ordenador del
   usuario conectado a la sesión; pedir permiso antes de usarlo.

## Datos del proyecto

- Netlify publica solo la carpeta `public/` (ver `netlify.toml`); el resto del repositorio no se ve en la web.
  - `public/index.html`: portada (landing page) con el botón "Start a voyage summary".
    Rehecha a partir de la captura de la portada original; fondo `public/ship-bg.jpg`.
  - `public/app/index.html`: la app (Voyage Summary Builder para cruceros de Oceania), en /app/.
- Antes de sustituir algo publicado, mirar qué hay en la web y no perderlo.
- Se publica en Netlify, sitio `voyage-summary-jc`, dominio https://www.jccruisesummary.com.
- Cambios: rama de trabajo, solicitud de cambio (pull request) a `main`, y el usuario la
  aprueba. Netlify está conectado a GitHub y publica solo al aprobar; después comprobar que
  la web publicada coincide con `main`.
- El mapa usa la costa de Natural Earth (dominio público) y los puertos de UN/LOCODE más una
  lista de nombres añadidos a mano. Si el usuario da puertos que no salen, añadirlos ahí.
- Hablar con el usuario en español, sin tecnicismos.
