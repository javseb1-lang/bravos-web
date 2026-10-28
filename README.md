# Club de Ajedrez Bravo’s

Web informativa de clases virtuales, con temarios, galería, Bravos Quiz y contacto por WhatsApp.

## Arquitectura

- Editor: Visual Studio Code.
- Control de versiones: Git y un repositorio de GitHub.
- Publicación: Netlify conectado al repositorio.
- Sitio: HTML, CSS y JavaScript; no requiere instalar dependencias ni compilar.
- No utiliza una base de datos. Las imágenes y los videos se guardan en `dist/assets/`.

## Archivos principales

- `dist/index.html`: estructura, secciones y textos generales.
- `dist/style.css`: diseño, colores y animaciones.
- `dist/script.js`: interacción, galerías, módulos y reproductores.
- `dist/content.js`: temarios y configuración de videos, anuncio de noviembre, módulo extra, TikTok y URL del juego.
- `dist/assets/`: logos, fotos y archivos multimedia.
- `netlify.toml`: configuración de publicación; carpeta pública `dist`.
- `CONTENIDO.md`: instrucciones para incorporar el contenido pendiente.

## Primeros pasos con Git Bash

1. Extraer el ZIP y abrir la carpeta `bravos-web` en VS Code.
2. Abrir Git Bash dentro de esa carpeta.
3. Crear un repositorio vacío en GitHub, sin README, licencia ni gitignore.
4. Ejecutar:

```bash
git init
git branch -M main
git add .
git commit -m "Publicacion inicial de Bravos"
```

5. Conectar el repositorio usando su URL real:

```bash
git remote add origin URL_REAL_DEL_REPOSITORIO
git push -u origin main
```

No ejecutar el comando con el texto URL_REAL_DEL_REPOSITORIO: sustituirlo por la URL que entregue GitHub.

## Publicar con Netlify

Importar el repositorio de GitHub como un proyecto nuevo.

- Rama de producción: `main`.
- Directorio base: raíz del repositorio, vacío en el formulario.
- Comando de construcción: vacío.
- Directorio de publicación: `dist`.

`netlify.toml` ya declara el directorio público. Comprobar el acceso que se desea dar a la página antes de compartir la URL con alumnos.

## Actualizar después

Editar solo los archivos necesarios en VS Code, revisar la vista previa local y ejecutar:

```bash
git status
git add .
git commit -m "Describe el cambio realizado"
git push
```

Netlify publicará los cambios de la rama conectada. No es necesario volver a importar la carpeta completa ni reemplazar todo el código.

## Vista previa en la computadora

Abrir la carpeta con VS Code y servir `dist` con un servidor local. Si ya está instalada la extensión Live Server, abrir `dist/index.html` con ella. Alternativamente, si Python está instalado:

```bash
python -m http.server 5500 --directory dist
```

Después abrir `http://localhost:5500/`.

## Bravos Quiz

El crédito enlaza a JAVSEB: https://javseb.netlify.app/. Bravos Quiz se presenta como complemento de las clases. La consulta específica del juego fue retirada; el contacto de la escuela sigue siendo WhatsApp +591 72560021.

El video de una clase y el video demostrativo de Bravos Quiz utilizan fuentes independientes.
