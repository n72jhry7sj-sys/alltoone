# All to one — Versión web 2.0 (prototipo local)

## Publicación en GitHub Pages

Sube los archivos **index.html, manifest.webmanifest, icon.svg y sw.js** directamente a la raíz del repositorio `alltoone` (no subas la carpeta contenedora ni el ZIP). GitHub → Add file → Upload files → Commit changes. En Settings → Pages usa `Deploy from a branch`, `main`, `/ (root)`. Espera a que Actions marque la publicación correcta y recarga la página.

## Qué funciona en esta versión

- Calendario familiar y eventos con fecha/hora.
- Convivencia semanal desde el lunes 23/11/2026, con Carla como entrante; excepciones y lunes sin colegio, reparto de festividades y visualización de periodos.
- Actividades de Enzo y cancelaciones puntuales.
- Tareas, compra, menú semanal.
- Gastos de Enzo: categorías habituales, conceptos personalizados, aplicación mensual, importe, recibo pagado, pagador, reparto 50/50 y transferencias entre familias.
- Historial local de todos los cambios.
- Asistente de reglas para eventos, compras, tareas y gastos, con confirmación antes de guardar.

## Limitaciones de seguridad importantes

**No hay autenticación real, sincronización, almacenamiento privado ni notificaciones push en esta versión.** Los datos se guardan en `localStorage` de cada navegador. La interfaz de fotos y documentos es informativa; la subida está bloqueada deliberadamente. No subas DNI, informes médicos, fotos de menores ni datos sensibles a GitHub o a este prototipo. La etiqueta «actor» solo sirve para identificar registros de prueba, no verifica identidades.

## Próxima fase para uso familiar real

1. Crear proyecto Supabase y configurar Auth para Miguel, Michelle y Carla con correos individuales.
2. Crear tablas y políticas RLS que restrinjan toda lectura/escritura a los tres usuarios autorizados, y un bucket privado para documentos y fotos.
3. Migrar las operaciones del navegador a Supabase, con historial de auditoría en servidor y notificaciones sincronizadas.
4. Probar permisos y acceso con cuentas diferentes antes de subir información real. Las notificaciones push y correos requieren configuración adicional.

## Precisión del convenio

Las fechas especiales se muestran como una guía con franjas del convenio descritas en la conversación. En particular, los días de Reyes de enero se asignan según el año civil mostrado; el bloque de Fin de Año del 1 de enero corresponde al año de inicio (31 de diciembre anterior). Antes de usar el calendario para decisiones reales, confirmar los detalles exactos del convenio y las excepciones acordadas.

## Datos de versiones anteriores

Esta versión usa una clave local nueva (`alltoone_v2`) y **no migra automáticamente los datos de prueba de versiones anteriores**. No borres el almacenamiento del navegador anterior si necesitas conservarlos. Solicita una migración específica antes de reemplazar datos importantes.


## Versión 2.1
En Convivencia, pulsa un día para editar directamente quién tiene a Enzo, guardar un cambio puntual o restablecer la asignación según el calendario. Se conserva el almacenamiento local `alltoone_v2` de la versión 2.0.
