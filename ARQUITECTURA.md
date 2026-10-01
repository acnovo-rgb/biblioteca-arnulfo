# ARQUITECTURA.md

# Arquitectura del Proyecto

## Arquitectura de GitHub Pages Estático

Este proyecto utiliza la arquitectura de **GitHub Pages estático** para servir las páginas web de la biblioteca personal.

### Flujo de Trabajo
1. **Excel como Datos Maestros**: El archivo `Biblioteca Personal.xlsx` es la fuente de verdad para todo los datos de la biblioteca.
2. **Páginas Generadas Estáticamente**: Las páginas HTML se generan a partir de los datos del Excel.
3. **Dominio Personalizado**: Solo después de la validación del sitio temporal en GitHub Pages se configura el dominio personalizado.
4. **Control de Versiones**: Los cambios se compromitan siempre para que el historial de Git proporcione capacidad de rollback.

### Estructura de Archivos
- `index.html` - Página de aterrizaje temporal
- `catalogo.html` - Catálogo de libros
- `resenas.html` - Reseñas de libros
- `archivo.html` - Archivo de contenido
- `RECUPERACION.md` - Procedimientos de recuperación
- `ARQUITECTURA.md` - Documentación de arquitectura

### Hosting
- GitHub Pages (rama main, directorio raíz)
- URL temporal: https://acnovo-rgb.github.io/biblioteca-arnulfo
- URL de producción: biblioteca.arnulfonovo.com
