# Mantenimiento de la biblioteca

## Regla principal

Las actualizaciones rutinarias son cambios pequeños, localizados y versionados. No se reconstruye el sitio completo y no se toca GitHub Pages, el dominio ni DNS para agregar o actualizar libros, reseñas, progreso o calificaciones.

## Fuente de verdad

- Catálogo publicado completo: `catalogo-full.md` (662 registros en la migración inicial).
- Reseñas publicadas completas: `resenas-full.md` (102 reseñas en la migración inicial).
- Navegación: `index.html`, `resenas.md` y `archivo.md`.
- El archivo Excel maestro se conserva como respaldo y fuente de reconciliación; no es necesario regenerar todo el sitio para cada cambio.

## Actualización rutinaria

1. Identificar exactamente el libro o reseña que cambia.
2. Modificar solamente el archivo de contenido correspondiente.
3. Crear un commit con una descripción concreta del cambio.
4. Verificar el archivo directamente en GitHub.
5. Verificar la página publicada en GitHub Pages.

## Prueba de reversibilidad

Cada cambio rutinario debe poder revertirse mediante su commit sin reconstruir el catálogo, las reseñas ni la infraestructura.

## Infraestructura protegida

No modificar durante mantenimiento rutinario:

- configuración de GitHub Pages;
- dominio personalizado;
- DNS;
- registros de correo;
- archivos de recuperación o arquitectura.

## Despliegue del dominio

El dominio `biblioteca.arnulfonovo.com` solo se cambia después de verificar completamente la copia de GitHub Pages y mediante una operación de DNS separada y reversible.

## Recuperación

Antes de una modificación importante, conservar la versión estable mediante Git. Si una actualización falla, revertir únicamente el commit defectuoso. No reconstruir desde cero.
