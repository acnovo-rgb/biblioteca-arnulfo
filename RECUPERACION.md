# RECUPERACION.md

## Documento de Recuperación y Procedimientos

### Producción
- **Target**: biblioteca.arnulfonovo.com
- **Hosting**: GitHub Pages
- **Repository**: acnovo-rgb/biblioteca-arnulfo
- **Branch**: main
- **Root**: /

### URLs
- **Current temporary Pages URL**: https://acnovo-rgb.github.io/biblioteca-arnulfo

### Fuente de Verdad
- **Source of truth**: Biblioteca Personal.xlsx

### Reglas Críticas
1. **Nunca** recrear "Mi ADN lector"
2. **Nunca** cambiar DNS hasta que el sitio temporal esté completamente verificado
3. **Antes** del cutover de DNS: preservar el CNAME anterior y registrarlo
4. **Rollback**: restaurar el CNAME anterior de biblioteca
5. **Nunca** alterar el root/apex, MX/email, o registros DNS no relacionados

### Verificaciones Previas al Cutover
- [ ] Verificar catálogo
- [ ] Verificar reseñas
- [ ] Verificar navegación
- [ ] Verificar HTTPS
