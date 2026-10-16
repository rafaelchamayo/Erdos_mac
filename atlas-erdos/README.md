# Atlas de una vida matemática

Web estática mínima sobre el proyecto artístico dedicado a Paul Erdős. No necesita instalaciones ni compilación: abre `index.html` en un navegador.

## Archivos

- `index.html`: título, descripción, pie de imagen y créditos.
- `assets/styles.css`: diseño adaptable a móvil y escritorio.
- `assets/obra-provisional.svg`: collage geométrico de ejemplo, no es la obra final.
- `.nojekyll`: permite servir los archivos directamente en GitHub Pages.

## Añadir la obra final

1. Guarda tu imagen en `assets/obra.jpg` (o PNG/WebP).
2. En `index.html`, cambia `src="assets/obra-provisional.svg"` por `src="assets/obra.jpg"`.
3. Ajusta `width` y `height` a las dimensiones reales de la imagen. Se mostrará completa y sin recortes.
4. Escribe en `alt` una descripción de la obra y actualiza el pie de imagen.
5. Reemplaza los dos párrafos de la descripción, retira el aviso provisional y completa los créditos. Los comentarios del HTML señalan estos lugares.

## Publicar en GitHub Pages

1. Crea un repositorio público en GitHub, por ejemplo `atlas-erdos`.
2. Usa **Add file → Upload files** y sube el contenido de esta carpeta, manteniendo `assets/`. `index.html` debe quedar en la raíz del repositorio, no dentro de otra carpeta. Guarda los archivos con **Commit changes**. Si el selector oculta `.nojekyll`, puedes crearlo desde **Add file → Create new file**; debe estar vacío.
3. Abre **Settings → Pages**.
4. En **Build and deployment → Source**, elige **Deploy from a branch**.
5. Selecciona **main** y **/(root)**; pulsa **Save**.
6. Cuando termine la publicación, Pages mostrará el enlace, normalmente `https://TU-USUARIO.github.io/atlas-erdos/`.

Para actualizar la página, vuelve a subir los archivos modificados al mismo repositorio. GitHub Pages publicará los cambios automáticamente.

Guía oficial: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

El paquete no se ha subido a GitHub ni publicado. La imagen, descripción y créditos están marcados como provisionales. No hay JavaScript, fuentes externas ni servicios de terceros.
