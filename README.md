# OPTICpress · Flujo de automatización

**OPTICpress** es una línea de montaje automatizada que convierte la web anticuada de una óptica en un sitio **WordPress** moderno, sin trabajo manual repetitivo.

Este repo contiene la **visualización del pipeline** con la estética de **n8n**: **34 nodos** en **10 fases**, con badges de tiempo por paso.

> ⏱ **~5 min/web automático · +2 h de diseño (solo la 1ª vez).**

## Qué hace

Extrae el contenido de la web vieja (Locomotive) → lo audita y estructura con **IA (Claude)** → lo reconstruye sobre un diseño mejorado → instala y rellena **WordPress** (SSH + WP-CLI + REST API) → QA y publicación. La persona solo aporta el criterio de diseño la primera vez y da el visto bueno final. **Cuanto más se usa, más patrones aprende y más se automatiza.**

## Ver el flujo

- **En vivo (GitHub Pages):** `https://codekadigital.github.io/opticpress/`
- **Local:** abre `index.html` en el navegador.

## Leyenda

| Color | Significado |
|-------|-------------|
| 🟣 Magenta | IA · Claude |
| ⬛ Pizarra | Servidor · SSH |
| 🔵 Azul WP | WordPress |
| 🟢 Verde-agua | Datos / HTTP |
| 🟪 Violeta | Librería de patrones |
| 🟩 Verde | Condición (gate) |
| 🟠 Ámbar ✋ | Paso humano (control de calidad) |

## Archivo

- `index.html` — página autónoma (HTML/CSS/JS, sin dependencias externas). Tema claro/oscuro.
