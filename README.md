# Flujo de automatización · Migración web de ópticas

Visualización, con la estética de **n8n**, del pipeline que automatiza la migración de webs de ópticas (Locomotive → WordPress) con rediseño UX/UI, usando **Python + Claude + WP-CLI + REST API**.

**34 nodos** organizados en **10 fases**, con badges de tiempo por paso:
`⏱ ~5 min/web automático · +2 h de diseño (solo la 1ª vez)`.

## Ver el flujo

- **En vivo (GitHub Pages):** _se activa tras el primer despliegue_ → `https://codekadigital.github.io/optik-flujo-n8n/`
- **Local:** abre `index.html` en el navegador.

## Cómo leerlo

| Color | Significado |
|-------|-------------|
| 🟣 Magenta | IA · Claude |
| ⬛ Pizarra | Servidor · SSH |
| 🔵 Azul WP | WordPress |
| 🟢 Verde-agua | Datos / HTTP |
| 🟪 Violeta | Librería de patrones |
| 🟩 Verde | Condición (gate) |
| 🟠 Ámbar ✋ | Paso humano |

Los dos pasos humanos (Rediseño y Aprobación) son los puntos de control de calidad. Al madurar la librería de patrones, más webs entran por la rama *"Sí, existe patrón"* y saltan el rediseño manual: el sistema se vuelve más autónomo con el uso.

## Archivo

- `index.html` — página autónoma (HTML/CSS/JS, sin dependencias externas). Tema claro/oscuro.
