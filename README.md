# EVOLU — landing page

Sitio estático de una sola página. Sin build, sin dependencias: `index.html` lo contiene todo
(CSS y JS en línea, sin recursos externos).

## Estructura

```
index.html    la landing completa
vercel.json   cabeceras y cleanUrls
```

## Publicación

El repositorio está conectado a Vercel. Cada push a `main` publica una versión nueva
automáticamente; no hace falta ejecutar nada más.

```bash
git add -A
git commit -m "descripcion del cambio"
git push
```

## Editar

Todo el diseño vive en el bloque `<style>` de `index.html`. Los colores son custom properties
en `:root` (y se redefinen para tema oscuro), así que un cambio de paleta se hace ahí.

## Pendiente antes de publicar

- Los botones "Añadir al carrito" apuntan a `#`: falta enlazar el checkout real.
- Precios en `$` sin moneda: `$44` / `$79` / `$29`.
- El pie indica que EVOLU es una marca ficticia y que los valores son de muestra.
