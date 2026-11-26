# Decomobi SRL — Sitio web corporativo

Sitio web estático de una sola página, independiente de MAD Center. Incluye sus imágenes, logos, menú responsive, animaciones suaves y botones de contacto.

**Dominio previsto:** `https://decomobi.tumaestrobolivia.com`

## Subir a un repositorio GitHub nuevo

1. En GitHub → **New repository**, crear `decomobi-web` (recomendado: **Public** para GitHub Pages gratuito) bajo `diegojuliovalen`.
2. Descomprimir el ZIP. Los archivos **index.html**, **CNAME**, **.nojekyll** y las imágenes ya están preparados en la raíz.
3. Dentro del repositorio → **Add file** → **Upload files**. Arrastrar el **contenido** de la carpeta extraída (no la carpeta ni el ZIP).
4. **Commit changes**, usando la rama `main`.
5. **Settings** → **Pages** → **Build and deployment** → **Source: Deploy from a branch** → **Branch: main** → **Folder: /(root)** → **Save**.
6. En **Settings** → **Pages** → **Custom domain** escribir `decomobi.tumaestrobolivia.com` y guardar. El archivo `CNAME` ya contiene ese nombre.
7. Ir a **GoDaddy** → cartera de dominios → **tumaestrobolivia.com** → **DNS** → **Añadir registro**:
   - Tipo `CNAME`
   - Nombre/Host `decomobi`
   - Valor/Apunta a `diegojuliovalen.github.io`
   - TTL: valor predeterminado.
8. Esperar a que GitHub confirme DNS/HTTPS. Cuando aparezca la opción **Enforce HTTPS**, activarla.

No modificar el registro `acceso`: seguirá apuntando a Tu Maestro Bolivia en Railway. Tampoco hace falta instalar Django o PostgreSQL para este one-pager.

## Archivos importantes

- `index.html`: página principal, diseño y comportamiento.
- `decomobi_logo_transparent.png`: logo de cabecera, colores originales y fondo transparente.
- `decomobi_logo_footer.png`: el mismo logo, letras claras para que se lea sobre el footer oscuro; fondo transparente.
- `client_01.png` a `client_10.png`: instituciones en estilo monocromático.
- `render_*.jpg`: renders referenciales.
- `CNAME`: dominio personalizado en GitHub Pages.
- `.nojekyll`: publica el sitio sin procesamiento Jekyll.

Para actualizar el sitio: modificar/subir archivos al mismo repositorio en `main`; GitHub Pages volverá a publicarlo.

**Contacto configurado:** llamadas `61004301`; WhatsApp `+47 98633976`.

Este sitio es estático: **no necesita Railway**. La página principal de Tu Maestro Bolivia y el subdominio `acceso.tumaestrobolivia.com` no se verán alterados.
