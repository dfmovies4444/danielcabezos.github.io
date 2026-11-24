# Web de Daniel Cabezos Roig

Web estática (HTML, CSS y JS, sin servidor). Funciona en cualquier alojamiento gratuito de páginas estáticas.

## Publicarla gratis en GitHub Pages

1. Crea una cuenta en https://github.com (gratis).
2. Pulsa **New repository**. Nombre: `TUUSUARIO.github.io` (tu usuario exacto + `.github.io`). Márcalo como **Public** y pulsa **Create repository**.
3. En el repositorio vacío, pulsa **uploading an existing file** y arrastra el **contenido** de esta carpeta: `index.html`, `README.md` y la carpeta `assets` entera. Pulsa **Commit changes**.
   - El navegador admite archivos de hasta 25 MB. El vídeo de *El molí de vent* pesa 20 MB, así que cabe.
4. Ve a **Settings → Pages**. En *Build and deployment* elige **Deploy from a branch**, rama **main** y carpeta **/ (root)**, y pulsa **Save**.
5. En uno o dos minutos la web estará en `https://TUUSUARIO.github.io`.
6. Abre `index.html` y cambia la línea `og:image` por la dirección completa: `https://TUUSUARIO.github.io/assets/img/og.jpg`. Así sale la imagen de vista previa cuando compartas el enlace por WhatsApp, LinkedIn o email.

Si algún día quieres un dominio propio (tipo `danielcabezos.com`), se conecta en **Settings → Pages → Custom domain**.

## Cambiar cosas

- **Textos**: todo está en `index.html`. Cada texto aparece dos veces, una en `<span lang="es">` y otra en `<span lang="en">`. Si cambias uno, cambia también su traducción.
- **Añadir un vídeo de YouTube**: copia un bloque `<div class="row">` de "Otros trabajos" y cambia el ID del vídeo en `data-yt` y `data-thumb`. El ID es lo que va después de `v=` en el enlace, o después de `youtu.be/`.
- **Añadir un render**: guarda la imagen en `assets/img` (mejor en `.webp`, aunque `.jpg` también vale) y copia uno de los `<figure>` de la sección "Animación y 3D".
- **Vídeos propios**: en MP4 (H.264) y por debajo de 25 MB. Si pesa más, súbelo a YouTube como **Oculto** e insértalo como los demás.
- **Actualizar el CV**: sustituye `assets/cv/CV-Daniel-Cabezos-Roig.pdf` por el nuevo con el mismo nombre.
- **Quitar el efecto blanco y negro**: en `index.html`, busca la regla `.frame img` y borra `filter:grayscale(1) contrast(1.06);`.

## Réquiem (Google Drive)

Para que se reproduzca dentro de la web, el archivo de Drive tiene que estar compartido como **Cualquier persona con el enlace → Lector**.

## Estructura

```
index.html          la web entera (estructura, estilos y código)
assets/img/         renders, fotogramas y retrato en WebP
assets/video/       El molí de vent (20 MB) y el loop de portada
assets/cv/          tu CV en PDF (sin la dirección de la calle) para el botón «Descargar CV»
assets/fonts/       tipografías Anybody y Newsreader (licencia SIL OFL)
```
