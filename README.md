# Nature Company Resto

Web institucional del restaurante Nature Company Resto (Martínez, GBA). Astro + Tailwind CSS v4, sitio 100% estático, sin backend.

## Stack

- Astro 7 (`output: "static"`)
- Tailwind CSS v4 (`@tailwindcss/vite`, tokens en `src/styles/global.css`)
- `@astrojs/sitemap` para `sitemap-index.xml`
- Tipografías: Instrument Serif (títulos) + Archivo (cuerpo), vía Google Fonts

## Comandos

| Comando           | Acción                                      |
| :----------------- | :------------------------------------------ |
| `npm install`       | Instala dependencias                        |
| `npm run dev`       | Servidor local en `localhost:4321`          |
| `npm run build`     | Build de producción a `./dist/`             |
| `npm run preview`   | Previsualiza el build de producción         |

## Estructura

```
src/
├── assets/images/   fotos y logo (optimizados por astro:assets)
├── components/      Nav, Hero, Pilares, Chef, Menu, Gallery, Reservas, Encontranos, Footer
├── layouts/         Layout.astro (SEO, JSON-LD, fonts)
├── pages/           index.astro
└── styles/          global.css (tokens de marca)
```

## Deploy

Pensado para Vercel (sitio estático). Antes de deployar, actualizar `site` en `astro.config.mjs` y el dominio canónico en `Layout.astro` si cambia `naturecompany.com.ar`.
