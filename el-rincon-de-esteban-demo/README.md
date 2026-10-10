# El Rincón de Esteban — plantilla demo

Web estática (HTML + CSS + JS, sin build). Maqueta de demostración.

## Subir a GitHub
1. Crea un repositorio vacío en github.com (sin README).
2. En esta carpeta:
   git init
   git add .
   git commit -m "Primera versión"
   git branch -M main
   git remote add origin https://github.com/TU_USUARIO/TU_REPO.git
   git push -u origin main

## Publicar en Cloudflare Pages
1. Cloudflare → Workers & Pages → Create → Pages → Connect to Git.
2. Elige el repositorio.
3. Framework preset: None.
4. Build command: (vacío).
5. Build output directory: /
6. Save and Deploy.

## Antes de usarla con un cliente real
- Cambiar EJEMPLO.com por el dominio real en: index.html (canonical, og:url, JSON-LD), las 3 páginas legales, sitemap.xml y robots.txt.
- index.html: cambiar "noindex, nofollow" por "index, follow" y borrar la franja .demo.
- robots.txt: cambiar "Disallow: /" por "Allow: /".
- Formulario: poner FORM_ENDPOINT (Web3Forms o Formspree) en el script de index.html.
- Páginas legales: rellenar los campos [entre corchetes] y pedir revisión profesional.
- Añadir og:image, fotos reales y precios confirmados.
