# Dinamita PDF – Web v2 (estático)

Funciones 100% en navegador:
- Unir PDFs
- Dividir PDF por rangos (descarga en ZIP)
- Imágenes → PDF
- PDF → PNG (render con pdf.js)

> **Requisitos**: acceso a Internet para cargar librerías desde CDN.
> Si lo necesitas 100% offline, coloca las librerías en `vendor/` y cambia los `<script>` a rutas locales.

## Despliegue rápido

### Vercel
1. Crea un nuevo proyecto "Other / Static".
2. Sube esta carpeta tal cual (index.html + assets/).
3. Deploy. Abre la URL pública.

### Netlify
1. Arrastra la carpeta al panel de Netlify (Drop site).

### GitHub Pages
1. Crea repo, sube archivos a la rama principal.
2. En Settings → Pages elige "Deploy from a branch" (main / root).

## Librerías usadas (CDN)
- pdf-lib
- jszip
- FileSaver
- pdf.js (para PDF→PNG)

## Notas
- Si abres el `index.html` directamente como archivo local (file:// o content://), es posible que el navegador bloquee los scripts externos: súbelo a hosting.
- DPI más alto = más calidad en PNG, pero tarda más y consume memoria.
