# Contenido pendiente de Bravo’s

Editar `dist/content.js`; los archivos se sirven desde `dist/assets/`. El sitio no requiere un panel ni login para estas actualizaciones.

## Video de clase
Añadir un MP4 y completar `classVideo.src`, por ejemplo `assets/clase-bravos.mp4`. Opcional: `poster` y archivo WebVTT en `captions`. El reproductor utiliza controles y no reproduce automáticamente. El aviso Próximamente se sustituye al cargar el video.

## Anuncio de noviembre
Añadir la imagen y completar `novemberAnnouncement.image`, por ejemplo `assets/anuncio-noviembre.webp`. El afiche se mostrará completo, con apertura de la imagen al pulsarlo. Completar `alt`, `title`, `description` y `label` con el contenido real.

## Módulo extra
Completar `extraModule` con un objeto del mismo formato que los elementos de `modules`: `id`, `title`, `tone` (gold/navy/copper), `piece` (king/knight/rook), `photo`, `topics` (objetos con title y description), `footer`. Se inserta antes de `extraModuleBefore` (por defecto intermedio). No se muestra un módulo vacío ni se inventa contenido.

## Redes sociales
Facebook ya está conectado. Completar `socials.tiktok` con la URL oficial; se habilita el enlace automáticamente. WhatsApp permanece como único canal de contacto: +591 72560021.

## Animación
Gráficos vectoriales SVG integrados. No hacen falta PNG. La entrada se muestra una vez por sesión. Se respeta la preferencia de movimiento reducido del dispositivo y hay un control adicional en el pie de página.

## Bravos Quiz
La nueva sección utiliza el logo original y la explicación del club. Completar `quizVideo.src` con el video de demostración (por ejemplo `assets/bravos-quiz-demo.mp4`). `quizVideo.poster` y `quizVideo.captions` son opcionales. Este video es independiente de `classVideo`.
Completar `quizUrl` con la URL real de la app para habilitar el acceso directo; mientras esté vacío, ese acceso permanece oculto. El crédito «Creado por JAVSEB» enlaza a https://javseb.netlify.app/. La sección Bravos Quiz no tiene botón de consulta.
