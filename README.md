# Óptima Mercado

Sitio web estático para la revisión gratuita de facturas de luz de Óptima Mercado.

## Estructura

- `index.html`: página principal.
- `privacidad.html`: política de privacidad.
- `aviso-legal.html`: aviso legal.
- `cookies.html`: política de cookies.
- `404.html`: página de error para GitHub Pages.
- `robots.txt` y `sitemap.xml`: indexación básica.
- `public/`: logos, favicon y assets públicos.

## Publicar en GitHub Pages con Actions

Este proyecto está preparado para publicarse desde la raíz del repositorio mediante GitHub Actions.

1. Crea o abre el repositorio público en GitHub.
2. Desde esta carpeta, ejecuta:

```bash
git add .
git commit -m "Preparar web para GitHub Pages"
git push -u origin main
```

3. En GitHub, entra en `Settings` > `Pages`.
4. En `Build and deployment`, selecciona `GitHub Actions` como fuente.
5. El workflow `.github/workflows/pages.yml` publicará la web en cada push a `main`.

El dominio público y canónico del proyecto es:

```text
https://optimamercado.com/
```

Si cambia el dominio, actualiza a la vez `sitemap.xml`, `robots.txt`, los enlaces `canonical`, Open Graph y los datos estructurados del HTML.

## Notas

- La web no contiene formularios propios. Todos los botones de análisis apuntan al flujo externo de Óptima.
- Los assets principales tienen nombres seguros para GitHub Pages:
  - `public/favicon.png`
  - `public/optima-logo-color.png`
  - `public/optima-logo-white.png`
