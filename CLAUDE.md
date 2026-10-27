# ElegirBien Tech — contexto para Claude

Web: https://poloni2.github.io · Repo: Poloni2/poloni2.github.io (rama `main`, GitHub Pages desde la raíz).

Guías de compra de tecnología para estudiantes, escritas por Marco (estudiante de 2º de Teleco).
Objetivo: aprender SEO y, cuando haya tráfico, monetizar con AdSense. Presupuesto: 0 €.

## Cómo responder a Marco
- Español de España. Frases cortas, al grano. Datos concretos antes que adjetivos, cero lenguaje de anuncio.
- Si pide una decisión, da una sola opción.
- Antes de que gaste dinero, dile cuánto puede perder en el peor caso.
- Si una idea es mala o arriesgada, dilo claro y con números.

## Cómo está hecha la web
- HTML estático a mano, sin generador ni dependencias. No hay que instalar ni compilar nada.
- `style.css`: estilos de toda la web (modo claro y oscuro, móvil primero).
- Cada página es una carpeta con `index.html`: `/`, `/sobre-mi/`, `/contacto/`, `/privacidad/`, y una carpeta por artículo.
- `sitemap.xml` y `robots.txt` en la raíz. `.nojekyll` para que GitHub no procese nada.
- Todas las páginas comparten la misma cabecera, menú y pie. Si cambias uno, cámbialo en todas.
- `index.html` de la raíz lleva la etiqueta de verificación de Google Search Console. No la quites.
- Todas las páginas llevan el script de GoatCounter justo antes de `</body>`:
  `<script data-goatcounter="https://elegirbientech.goatcounter.com/count" async src="//gc.zgo.at/count.js"></script>`
- Hay un comentario `<!-- ADSENSE: ... -->` en el `<head>`. Ahí irá el código de AdSense cuando lo aprueben.

## Publicar un artículo nuevo
1. Carpeta nueva con slug en minúsculas y guiones (p. ej. `mejor-calculadora-cientifica-ingenieria/`), copiando la estructura de `mejores-auriculares-estudiar-calidad-precio/index.html`.
2. Cambiar `<title>`, `description`, `canonical`, etiquetas `og:` y el `<article>`. Fecha en `<time datetime="AAAA-MM-DD">`.
3. Añadir una tarjeta `<li class="card">` en `index.html` de la raíz (la más reciente arriba).
4. Añadir la URL a `sitemap.xml` con `lastmod`.
5. Comprobar que se ve bien en móvil (390 px) y ordenador, sin scroll horizontal.
6. Commit y push a `main`. GitHub Pages publica en 1-2 minutos.

## Reglas de contenido
- Formato de guía: introducción personal, tabla comparativa rápida, producto por producto (lo mejor, lo peor, "Lo elegiría si…"), guía de compra, 3 preguntas frecuentes, conclusión con un ganador claro. Unas 1.500 palabras.
- Palabra clave principal en el título, la primera frase y un subtítulo (h2). No más de 4-5 veces en total.
- **El texto lo escribe Marco.** Claude prepara el guion, comprueba datos y corrige, pero no escribe el artículo entero: la experiencia propia es lo que diferencia la web.
- Nunca decir que Marco ha probado algo que no ha probado. Usar "he revisado", "lo elegiría porque…".
- Precios orientativos y con fecha. Comprobar que los modelos siguen a la venta y las cifras (batería, etc.) en la web del fabricante.
- Temas: 3 de tecnología para estudiantes y 1 de deporte con enfoque tecnológico al mes. Nada fuera de tema.

## Datos de Marco útiles para escribir (públicos en "Sobre mí")
- Usa iPhone 16 Pro tras años con Android; AirPods 4 (andando a clase, en el tren los fines de semana, vídeos en casa).
- Portátil Acer Nitro V16, sobremesa con monitor; ratón HP 420/425 Programmable Bluetooth (de sus mejores compras).
- Calculadora Casio fx-991SP CW. Toma apuntes en papel. Estudia sin música, sobre todo en casa.
- Gimnasio 3 días por semana y taekwondo; usa Boditrax 2.0. Dejó el reloj inteligente porque le molestaba.
- Le apasiona la astronomía. Prefiere Apple. No gasta en tecnología si no lo necesita.
- Mala compra: capturadora para jugar a Switch/PS4 en el PC.

## Calendario de artículos (sábado se escribe, domingo se publica)
- 24 oct: mejor calculadora científica para ingeniería
- 31 oct: ratón barato para portátil
- 7 nov: Black Friday en tecnología para estudiantes
- 14 nov: (deporte) auriculares para el gimnasio
- 21 nov: regalos tecnológicos para estudiantes por menos de 50 €
- 28 nov: AirPods 4 para estudiantes, ¿merecen la pena?
- 5 dic: telescopio calidad-precio para empezar
- 12 dic: (deporte) básculas de bioimpedancia, ¿son fiables?
- Ideas pendientes: portátil gaming para ingeniería (Acer Nitro V16), de Android a iPhone, capturadora para consola en el PC, por qué dejé el reloj inteligente, calculadoras permitidas en la PAU (publicar en marzo-abril).

## Fuera del repo
- Contacto público: elegirbientech@outlook.com (se reenvía al Gmail de Marco).
- Visitas: GoatCounter (panel elegirbientech.goatcounter.com, informe semanal por correo).
- Google Search Console verificado con prefijo `https://poloni2.github.io/` y sitemap enviado.
- Dominio propio: aún no. Cuando toque, un .com (~10-15 €/año); .tech descartado por la renovación cara.
- Tareas programadas en claude.ai (no dependen de este repo): guion del artículo (viernes 17:52), resumen de correo (viernes 16:51), resumen de visitas (domingo 19:51).
