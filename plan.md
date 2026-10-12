# Plan: msdos-manual-html5

## Resumen
Manual de referencia offline para comandos básicos de MS-DOS, construido en HTML5, CSS3 y JavaScript vanilla, con buscador en tiempo real, modos claro/oscuro, soporte de impresión y optimización completa de SEO y accesibilidad.

## Objetivos
- [x] Proveer una guía completa para comandos MS-DOS esenciales (DIR, COPY, DEL, MD, CD, REN, TYPE, CHKDSK, ATTRIB).
- [x] Incluir buscador en vivo, navegación secuencial y modos de visualización claro/oscuro.
- [x] Ser completamente estático y sin dependencias externas.
- [x] Soporte de impresión optimizado (`@media print`) para generar PDFs de referencia.
- [x] Optimización de accesibilidad ARIA y meta etiquetas SEO.

## 🏗️ Arquitectura

- **Patrón**: MPA (Multi Page Application) estática con navegación secuencial y buscador cliente.

```text
msdos-manual-html5/
├── index.html             # Portada, buscador y tabla de contenidos
├── commands/              # Páginas individuales para cada comando (DIR, COPY, DEL, etc.)
│   ├── attrib.html
│   ├── cd.html
│   ├── chkdsk.html
│   ├── copy.html
│   ├── del.html
│   ├── dir.html
│   ├── md.html
│   ├── ren.html
│   └── type.html
├── assets/
│   ├── css/styles.css     # Estilos globales y modo oscuro/impresión
│   └── img/
│       ├── favicon.svg
│       └── msdos-logo.svg
├── README.md
└── plan.md
```

## 🧠 Paradigma de Programación

- **Imperativo/Procedimental + Event-Driven**
- Las funciones de búsqueda y filtrado en el cliente son **imperativas** (búsqueda en el DOM).
- La interacción con el buscador es **event-driven** (listeners de teclado/entrada `input` y `keydown`).

---

## 🌐 Propósito de Visibilidad y Destino Remoto

- **Visibilidad**: `Público (Open Source / Portafolio)`.
- **Plataforma Remota Asignada**: `GitHub`.
- **Plataforma de Despliegue CI/CD**: `GitHub Pages` / `Cloudflare Pages`.
- **Justificación**: Manual offline de comandos MS-DOS con buscador y estilos de impresión, contenido didáctico libre ideal para GitHub Pages.

---

> ⚠️ **Auditoría de UI / DESIGN.md:** La interfaz actual no cumple con las directrices visuales de [DESIGN.md](../DESIGN.md) (requiere paleta HSL, Google Fonts modernas y profundidad/glassmorphism). Pendiente refactor visual.
## Estado actual
- Estado: ✅ **Completado**
- 9 páginas de comandos completas con sintaxis, banderas, ejemplos prácticos y navegación anterior/siguiente.
- Buscador interactivo en portada con atajo <kbd>Esc</kbd>.
- Modo oscuro y estilos de impresión (`@media print`).

## Tareas realizadas
- [x] Rellenar todas las páginas de comandos con su sintaxis, opciones y ejemplos detallados.
- [x] Asegurar que el buscador en `index.html` funcione correctamente con los comandos.
- [x] Implementar la navegación "anterior/siguiente" entre las páginas de comandos.
- [x] Verificar la funcionalidad de los modos claro/oscuro y la impresión.
- [x] Mejorar la accesibilidad y el SEO con metadatos OpenGraph y atributos semánticos.

## Stack / Tecnologías
- HTML5, CSS3 (variables CSS, `@media print`, `prefers-color-scheme`)
- Vanilla JavaScript
