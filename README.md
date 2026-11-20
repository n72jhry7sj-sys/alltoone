# All to one — PWA familiar (prototipo local)

## Publicación gratuita en GitHub Pages
1. Crea un repositorio en GitHub (por ejemplo `all-to-one`).
2. Sube `index.html`, `manifest.webmanifest`, `icon.svg` y `sw.js` a la raíz.
3. En Settings → Pages → Build and deployment, selecciona Deploy from a branch, rama `main`, carpeta `/ (root)`.
4. Abre la dirección HTTPS proporcionada por GitHub Pages en Safari del iPhone.
5. En Safari, toca Compartir → Añadir a pantalla de inicio.

## Aviso de privacidad
Este prototipo usa localStorage y NO sincroniza entre móviles, no dispone de autenticación ni cifrado de datos local adicional. GitHub Pages publica el código y la interfaz; nunca incluyas información privada dentro de los archivos subidos. No uses esta versión para documentos sensibles ni información confidencial sobre menores. Exporta copias de seguridad desde Ajustes.

## Próxima fase
Conectar Supabase Auth + tablas con políticas Row Level Security por familia, roles, almacenamiento privado, gestión de invitaciones, y notificaciones opt-in. No incluir claves secretas en código cliente. Revisar reglas de convivencia y permisos antes de activar sincronización.

## Convivencia de Enzo (versión 1.1)
Semanas alternas: el adulto que termina su semana lleva a Enzo al colegio el lunes; el adulto entrante lo recoge a la salida, sin hora fija. El lunes aparece como transición (🎒). Se pueden introducir excepciones por día o intervalo. **IMPORTANTE:** fecha inicial 23/11/2026 y primer adulto Miguel son valores provisionales; confirmarlos en la pantalla Días. Los días sin colegio requieren ajuste manual.

## Convivencia (versión 1.2)
- Familia 1: Miguel/Michelle; Familia 2: Carla.
- Lunes 23/11/2026: Carla recoge a Enzo del colegio e inicia su semana.
- Cada lunes lectivo: familia saliente deja a Enzo en el colegio y entrante recoge a la salida.
- Si el lunes es festivo o no lectivo: cambio el domingo anterior a las 20:00. Añade ese lunes manualmente en «Lunes sin colegio».
- Los festivos escolares NO se descargan automáticamente. Las fechas deben verificarse e introducirse.
- La información se almacena únicamente en este navegador, sin sincronización.
