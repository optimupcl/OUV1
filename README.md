# OptimUp — Logo Kit

Kit completo de logo procesado a partir del archivo original.
Todos los archivos tienen fondo transparente (excepto OG image y apple-touch-icon, que llevan fondo intencional).

## Archivos incluidos

| Archivo | Uso |
|---|---|
| `optimup_logo_1024.png` | Master de alta resolución. Usar para impresión, presentaciones, cualquier uso futuro. |
| `optimup_logo_512.png` | Versión web estándar. Usar en la sección "equipo" de la web como sello. |
| `favicon.ico` | Favicon multi-tamaño (16/32/48). El favicon clásico que entiende todo navegador. |
| `favicon-32x32.png` | Favicon moderno alta densidad. |
| `favicon-16x16.png` | Favicon moderno baja densidad. |
| `apple-touch-icon.png` | 180×180. Icono cuando alguien guarda tu sitio en pantalla de inicio de iPhone. |
| `android-chrome-192x192.png` | Icono PWA Android pequeño. |
| `android-chrome-512x512.png` | Icono PWA Android grande / splash screen. |
| `og-image.png` | 1200×630. Previsualización al compartir en WhatsApp, LinkedIn, Twitter, etc. |
| `site.webmanifest` | Manifiesto PWA. Le dice a Android cómo instalar tu sitio como app. |

## Instalación en la web

### Paso 1: subir archivos
Sube TODOS los archivos a la **raíz** de tu sitio (al mismo nivel que `index.html`).
En Netlify: arrastra los archivos a la carpeta del proyecto antes del deploy.

### Paso 2: agregar etiquetas en `<head>` del HTML
Pega este bloque dentro del `<head>` de tu `index.html`:

```html
<!-- Favicons -->
<link rel="icon" href="/favicon.ico" sizes="any">
<link rel="icon" type="image/png" sizes="32x32" href="/favicon-32x32.png">
<link rel="icon" type="image/png" sizes="16x16" href="/favicon-16x16.png">
<link rel="apple-touch-icon" sizes="180x180" href="/apple-touch-icon.png">
<link rel="manifest" href="/site.webmanifest">
<meta name="theme-color" content="#0f2a44">

<!-- Open Graph (previsualización al compartir) -->
<meta property="og:title" content="OptimUp">
<meta property="og:description" content="Optimización del sistema comercial">
<meta property="og:image" content="https://optimup.cl/og-image.png">
<meta property="og:url" content="https://optimup.cl">
<meta property="og:type" content="website">

<!-- Twitter Card -->
<meta name="twitter:card" content="summary_large_image">
<meta name="twitter:title" content="OptimUp">
<meta name="twitter:description" content="Optimización del sistema comercial">
<meta name="twitter:image" content="https://optimup.cl/og-image.png">
```

### Paso 3: usar el logo en la web (opcional)
Para incrustar el logo grande en la sección de equipo o donde quieras:

```html
<img src="/optimup_logo_512.png" alt="OptimUp" width="120" height="120">
```

## Notas

- El **OG image** lleva fondo navy con texto. Si querés cambiar el subtítulo (hoy dice "Optimización del sistema comercial"), avísame y lo regenero.
- El **apple-touch-icon** lleva fondo blanco a propósito: iOS no respeta transparencia y se ve mejor con fondo sólido.
- Después de subir y publicar, el favicon puede tardar unos minutos en aparecer (el navegador cachea el anterior). Forzá refresco con Ctrl+Shift+R.
