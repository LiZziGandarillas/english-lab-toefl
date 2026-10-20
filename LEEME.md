# English Lab · TOEFL 2026

App de estudio pensada para celular. Incluye una semana de reinicio (19–25 de octubre de 2026), repaso aleatorio de Weeks 1–3, adelanto de Weeks 4–5, tarjetas de vocabulario, ejercicios de Reading/Listening/Speaking/Writing, una guía gramatical A1–C2 con búsqueda y micro-retos, racha local, registro de tiempo y exportación de reportes y respaldo.

## Abrir

- En PC: abre `index.html` en un navegador moderno.
- Para publicar e instalarla en el celular usando GitHub Pages, sigue el paso a paso de `PUBLICAR_EN_GITHUB_PAGES.md`. La app necesita servirse desde HTTPS.
- En celular: abre la URL HTTPS publicada y elige **Añadir a pantalla de inicio** (Android/Chrome) o **Añadir a pantalla de inicio** desde Compartir (iPhone/Safari).
- Al abrir por `file://`, la app funciona para practicar, pero la instalación PWA y el modo sin conexión requieren HTTP/HTTPS. La grabación de voz necesita permiso de micrófono y normalmente un origen seguro (HTTPS/localhost).

## Progreso y privacidad

El progreso se guarda en `localStorage` de ese navegador/dispositivo. Usa **Reporte → Respaldar progreso** para descargar un JSON y **Importar respaldo** al cambiar de navegador o teléfono. Las grabaciones de Speaking son temporales y se mantienen en la página; no se cargan a servidores. GitHub Pages publica el código y la interfaz, no los datos locales que registres al estudiar.

## Alcance actual

La puntuación de las prácticas escritas/orales es de autoevaluación y no equivale a un puntaje oficial ETS. El ejercicio de escucha usa síntesis de voz del dispositivo. Añadir contenido semanal requiere editar los arrays de datos al final de `index.html`; no hay sincronización en la nube ni tutor IA embebido todavía.
