# Coffea — Landing Page

Landing page estática de una sola página para la cafetería ficticia **Coffea**. Construida con **HTML5 semántico** y **CSS3** puro, sin JavaScript, frameworks ni preprocesadores.

## Stack

- **HTML5** semántico
- **CSS3** con custom properties, Flexbox, Grid y `scroll-snap`
- **Sin JavaScript**
- **Sin** Tailwind, Sass, bundlers ni CMS

## Estructura del proyecto
coffea-landing/
├── index.html
├── 404.html
├── netlify.toml
├── README.md
├── css/
│ ├── tokens.css
│ ├── base.css
│ ├── layout.css
│ ├── utilities.css
│ └── components/
│ ├── header.css
│ ├── hero.css
│ ├── categories.css
│ ├── product-card.css
│ ├── carousel.css
│ ├── promo.css
│ ├── testimonial-card.css
│ ├── newsletter.css
│ └── footer.css
└── assets/
├── img/
├── icons/
└── fonts/


## Convenciones

- **Nomenclatura BEM:** `.product-card`, `.product-card__title`, `.product-card--featured`.
- **Design tokens:** todo color, fuente, radio y espaciado referencia un token en `css/tokens.css`.
- **Mobile-first:** estilos base para 360px y `@media (min-width: ...)` hacia arriba.
- **Unidades:** `rem` para tipografía y espaciados, `clamp()` para títulos fluidos.
- **Layout:** Flexbox y Grid; `position: absolute` solo para superposiciones.
- **`@layer`:** tokens, base, layout, components, utilities.

## Cómo levantar en local

El proyecto no requiere build ni dependencias. Solo necesitás un servidor estático.

### Opción 1: Python (ya instalado en la mayoría de sistemas)

```bash
# Desde la raíz del proyecto
python3 -m http.server 8000

Abrir http://localhost:8000

opción 2 (en node.js) bash: npx serve .

Opción 3: Extensión Live Server (VS Code)
Instalar la extensión Live Server y hacer click en Go Live desde index.html.

Despliegue en Netlify
Deploy continuo desde Git
Pushear el repo a GitHub o GitLab.

En Netlify: New site from Git → elegir el repo.

Configuración:

Build command: (dejar vacío)

Publish directory: .

Netlify detecta netlify.toml automáticamente.

La rama main publica a producción. Cada PR genera un Deploy Preview.

Deploy manual
bash
# Instalar Netlify CLI
npm install -g netlify-cli

# Deploy
netlify deploy --prod --dir=.
Formulario de newsletter
El formulario usa Netlify Forms (data-netlify="true"). Las suscripciones se ven en el panel de Netlify → Forms. No requiere backend ni JavaScript.

Assets
Los assets gráficos deben exportarse desde Figma y guardarse en assets/. Importante: las URLs de assets de Figma expiran a los 7 días. Exportar y versionar en el repo.

Licencia
Los assets gráficos del template Community de Figma pueden tener licencia de stock. Confirmar licencia antes de publicar o reemplazar por imágenes propias.




