# ElegirBien Tech

Web estática en HTML. No necesita instalar nada: GitHub Pages la sirve tal cual.

## Antes de subirla (5 min)

1. **Usuario de GitHub.** Ya está puesto: poloni2.github.io.
2. **Contacto.** Ya está puesto: elegirbientech@outlook.com.

## Subirla a GitHub Pages (gratis)

1. Crea una cuenta en github.com.
2. Crea un repositorio **público** llamado exactamente `TUUSUARIO.github.io`.
3. En el repositorio: **Add file → Upload files** y arrastra todo el contenido de esta carpeta
   (no la carpeta, lo de dentro). Pulsa **Commit changes**.
4. **Settings → Pages → Source: Deploy from a branch → main → / (root) → Save.**
5. En 1-2 minutos la web está en `https://TUUSUARIO.github.io`.

## Que Google la encuentre

1. Entra en Google Search Console (search.google.com/search-console).
2. Añade la propiedad con tu dirección de la web y verifícala.
3. En **Sitemaps**, envía `sitemap.xml`.

## Añadir un artículo nuevo

1. Copia la carpeta `mejores-auriculares-estudiar-calidad-precio` y ponle el nombre del nuevo artículo
   (en minúsculas y con guiones, por ejemplo `mejor-portatil-estudiar-ingenieria`).
2. Dentro, en `index.html`, cambia: `<title>`, `description`, `canonical`, `og:` y el contenido de `<article>`.
3. En `index.html` de la raíz, copia un bloque `<li class="card">` y apúntalo al nuevo artículo.
4. En `sitemap.xml`, añade una línea `<url>` con la nueva dirección.
5. Sube los cambios a GitHub.

## Cuando tengas dominio propio

Crea un archivo `CNAME` con una sola línea (por ejemplo `elegirbientech.com`), cambia
`https://TUUSUARIO.github.io` por el dominio en todos los archivos y configura el DNS siguiendo
la guía de GitHub Pages ("Managing a custom domain").

## Cuando AdSense te apruebe

Pega su código en el `<head>` de **todas** las páginas, donde pone `ADSENSE`.
Antes, revisa `privacidad/index.html` y añade un aviso de cookies (lo exige la ley en la UE).
