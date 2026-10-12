# Manual de Comandos MS‑DOS (HTML5)

Manual de referencia offline para comandos básicos de MS‑DOS, construido completamente en HTML5, CSS3 y JavaScript vanilla.

## Comandos incluidos

- **DIR** — Mostrar lista de archivos y directorios
- **COPY** — Copiar archivos
- **DEL** — Eliminar archivos
- **MD / MKDIR** — Crear directorios
- **CD** — Cambiar directorio actual
- **REN / RENAME** — Renombrar archivos
- **TYPE** — Mostrar contenido de archivo de texto
- **CHKDSK** — Verificar disco
- **ATTRIB** — Cambiar atributos de archivos

## Estructura

```
msdos-manual-html5/
├─ index.html              # Portada con tabla de contenidos y buscador
├─ assets/
│  ├─ css/
│  │  └─ styles.css        # Estilos responsivos, modo claro/oscuro, impresión
│  └─ img/
│     ├─ msdos-logo.svg    # Logo MS‑DOS
│     └─ favicon.svg       # Favicon
├─ commands/
│  ├─ dir.html
│  ├─ copy.html
│  ├─ del.html
│  ├─ md.html
│  ├─ cd.html
│  ├─ ren.html
│  ├─ type.html
│  ├─ chkdsk.html
│  └─ attrib.html
└─ README.md
```

## Cómo usar

1. Abrir `index.html` en cualquier navegador moderno (Chrome, Firefox, Edge).
2. Usar el **buscador** para filtrar comandos por nombre o descripción.
3. Hacer clic en un comando para ver sintaxis, opciones y ejemplos.
4. Navegar entre comandos con los enlaces **anterior/siguiente**.

## Características

- **Responsivo**: funciona en escritorio, tableta y móvil.
- **Modo claro/oscuro**: respeta la preferencia del sistema (`prefers-color-scheme`).
- **Buscador en vivo** en la página principal.
- **Soporte de impresión** (`@media print`) para generar PDF desde el navegador.
- **Sin dependencias externas**: solo HTML5, CSS3 y JavaScript vanilla.
- **SEO básico**: meta tags Open Graph, description y keywords.
- **Navegación secuencial** entre páginas de comandos (anterior/siguiente).