# Publicar English Lab para usarla en el celular

Esta app es estática: no necesita servidor propio ni instalar nada en la computadora. GitHub Pages la servirá con HTTPS, necesario para instalarla como PWA y para habilitar la grabación de voz desde el navegador.

## Antes de empezar: visibilidad y datos

Con una cuenta gratuita, GitHub Pages requiere un repositorio público. Tanto el código como la página serán visibles para cualquiera con el enlace; no publiques aquí el resto de `MEXT English`, el correo del premio TOEFL ni el código de canje. El progreso de estudio y las grabaciones no se envían a GitHub: se guardan localmente en el navegador del celular. La app usa ejemplos genéricos y no incluye el nombre de tu empresa.

## A. Crear un repositorio dedicado

1. Inicia sesión en [github.com](https://github.com/).
2. Pulsa **+** (arriba a la derecha) → **New repository**.
3. En **Repository name**, escribe `english-lab-toefl`.
4. Elige **Public**. El sitio publicado también será público.
5. Deja desmarcadas las opciones para añadir README, `.gitignore` o licencia. Pulsa **Create repository**.

## B. Subir solo los archivos de App

1. En el Explorador de Windows abre la carpeta `MEXT English\App`.
2. Selecciona los archivos que están directamente dentro de `App` (por ejemplo, `index.html`, `manifest.webmanifest`, `sw.js`, `.nojekyll`, iconos PNG/SVG y los archivos `.md`). No subas carpetas de otras materias ni documentos TOEFL.
3. En el nuevo repositorio de GitHub pulsa **Add file** → **Upload files**.
4. Arrastra ahí los archivos seleccionados. Comprueba que `index.html` queda directamente en la raíz del repositorio, no dentro de otra carpeta.
5. En **Commit changes**, deja el mensaje sugerido y pulsa **Commit changes**.

## C. Activar GitHub Pages

1. En el repositorio entra a **Settings** → **Pages**.
2. En **Build and deployment**, en **Source**, elige **Deploy from a branch**.
3. En **Branch**, elige `main`; en la carpeta, elige `/(root)`; pulsa **Save**.
4. Abre la pestaña **Actions** y espera a que termine el despliegue con marca verde. La primera publicación puede tardar unos minutos.
5. Vuelve a **Settings** → **Pages**. Ahí aparecerá **Your site is live at** con una dirección parecida a:

   `https://TU-USUARIO.github.io/english-lab-toefl/`

6. Abre el enlace en una computadora o teléfono y confirma que aparece English Lab. En **Settings → Pages**, activa **Enforce HTTPS** si GitHub muestra esa opción.

## D. Añadirla a la pantalla de inicio

### Android (Chrome)

1. Abre la URL publicada en Chrome.
2. Espera unos segundos a que termine de cargar y toca el menú **⋮**.
3. Elige **Instalar aplicación** o **Añadir a pantalla de inicio** y confirma.
4. Abre English Lab desde el nuevo icono. Para usar el micrófono, acepta el permiso cuando Chrome lo solicite.

### iPhone (Safari)

1. Abre la URL publicada en Safari.
2. Toca **Compartir** (cuadrado con flecha hacia arriba).
3. Elige **Añadir a pantalla de inicio** y confirma.
4. Abre English Lab desde el icono. La grabación de Speaking requiere permiso de micrófono.

## E. Actualizar la app más adelante

Cuando haya una nueva versión, abre el repositorio, pulsa **Add file → Upload files**, sube los archivos actualizados y confirma **Commit changes**. Para que la app del teléfono adopte la versión recién publicada, abre la página con internet y recárgala; el service worker guardará los archivos para el uso sin conexión.

La racha y el progreso pertenecen al almacenamiento local de ese navegador. Antes de borrar datos del navegador o cambiar de teléfono, en **Reporte → Respaldar progreso** descarga el JSON. Luego usa **Importar respaldo** en el nuevo dispositivo.

## Si algo no aparece

- **404:** confirma que `index.html` está en la raíz y que Pages usa `main` + `/(root)`.
- **No aparece Instalar:** entra al sitio por HTTPS, recarga una vez y usa el menú del navegador para añadirlo a inicio.
- **Cambios viejos:** abre el sitio con internet y recárgalo; si sigue igual, cierra la PWA y vuelve a abrirla.
- **El micrófono no funciona:** prueba la URL HTTPS en Chrome/Safari y revisa los permisos del sitio.
