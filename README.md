# Hello World

Página estática simple lista para desplegar en Netlify.

## Estructura

- `public/index.html` — la página "Hello World".
- `netlify.toml` — configuración de Netlify (publica la carpeta `public`, sin paso de build).

## Deploy en Netlify

**Opción 1 — Desde la UI (recomendado):**
1. En [app.netlify.com](https://app.netlify.com) elige *Add new site → Import an existing project*.
2. Conecta GitHub y selecciona este repositorio y la rama a desplegar.
3. Netlify leerá `netlify.toml` automáticamente (publish directory: `public`). Pulsa *Deploy*.

**Opción 2 — Con Netlify CLI:**
```bash
npm install -g netlify-cli
netlify login
netlify deploy          # deploy de previsualización
netlify deploy --prod   # deploy a producción
```

## Ver localmente

Abre `public/index.html` en el navegador, o ejecuta `npx serve public`.
