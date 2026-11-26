# Zafira Academia de Manejo

Sitio web informativo de una academia de conducción de autos y motos. Funciona como carta de presentación digital de la empresa: muestra sus cursos, instructores, vehículos y permite solicitar una clase práctica.

Proyecto académico desarrollado solo con **HTML y CSS** (sin JavaScript).

- **Repositorio:** https://github.com/danfer009/zafira-drive
- **Autor:** [Tu nombre completo]

## Cómo visualizar el sitio

1. Descarga o clona el repositorio:
   ```
   git clone https://github.com/danfer009/zafira-drive.git
   ```
2. Abre la carpeta del proyecto.
3. Abre `index.html` en el navegador (doble clic), o usa la extensión **Live Server** de VS Code (clic derecho sobre `index.html` → *Open with Live Server*).

Necesitas conexión a internet para que cargue la fuente Poppins (Google Fonts) y el mapa de la página de contacto.

## Páginas del sitio

| Archivo | Contenido |
|---|---|
| `index.html` | Portada con hero, botón de acción y 4 tarjetas de servicios |
| `sobre.html` | Historia, misión, visión, valores y testimonios |
| `instructores.html` | Tarjetas del equipo con foto, experiencia y licencia |
| `vehiculos.html` | Galería de autos y motos con filtros simulados |
| `cursos.html` | Tarjetas con precios y tabla comparativa |
| `agenda.html` | Formulario para solicitar una cita, con validación HTML5 |
| `contacto.html` | Datos de contacto en dos columnas y mapa incrustado |

El header con el menú y el footer se repiten en todas las páginas.

## Estructura de carpetas

```
zafira-drive/
├── index.html
├── sobre.html
├── instructores.html
├── vehiculos.html
├── cursos.html
├── agenda.html
├── contacto.html
├── css/
│   ├── reset.css
│   ├── variables.css
│   ├── layout.css
│   └── styles.css
├── assets/
│   └── img/
└── README.md
```

| Archivo CSS | Responsabilidad |
|---|---|
| `reset.css` | Quita los estilos por defecto del navegador |
| `variables.css` | Paleta, tipografía, espaciado, bordes y sombras |
| `layout.css` | Estructura general: header, menú, contenido y footer |
| `styles.css` | Componentes: botones, hero, tarjetas, tabla y formulario |

## Decisiones de diseño

### Paleta de colores

| Variable | Color | Uso |
|---|---|---|
| `--primary` | `#0D47A1` | Azul principal: header, títulos y detalles. Transmite confianza y profesionalismo |
| `--secondary` | `#FFB703` | Dorado: botones y resaltes. Atrae la atención hacia las acciones |
| `--accent` | `#06D6A0` | Verde menta: acentos |
| `--text` | `#1F2937` | Gris oscuro: texto y footer, con buen contraste |
| `--bg` | `#FAFAFA` | Fondo general, claro y limpio |
| `--white` | `#FFFFFF` | Tarjetas y texto sobre fondos oscuros |

### Tipografía

Se usa **Poppins** (Google Fonts) en pesos 400, 600 y 700, con `sans-serif` como respaldo. Una sola familia en todo el sitio mantiene la coherencia visual.

### Medidas

- Espaciado base: `--space: 16px`, con múltiplos calculados mediante `calc()`.
- Bordes redondeados: `--radius: 10px`.
- Sombra suave: `0 4px 12px rgba(0, 0, 0, 0.1)`.

### Layout

- **Flexbox:** header, menú de navegación, footer, filtros de vehículos y campos del formulario.
- **CSS Grid:** grupos de tarjetas (servicios, instructores, vehículos, cursos) y el formulario. Se usa `repeat(auto-fit, minmax(...))`, así las columnas se adaptan al ancho de pantalla.
- Contenido centrado con `max-width: 1100px`.

### Accesibilidad

- Etiquetas semánticas: `header`, `nav`, `main`, `section`, `article`, `footer`.
- `lang="es"` en todas las páginas y un solo `h1` por página.
- Menú con `aria-label` y `aria-current="page"` en la página activa.
- Imágenes con `alt` descriptivo e `iframe` con `title`.
- Formulario con `label for`, `required` y validación de correo y teléfono.
- Tabla con `caption`, `thead`, `tbody` y `th` con `scope`.
- Estados `:focus-visible` y `:focus` visibles al navegar con teclado.

## Requisitos técnicos

| Requisito | Estado |
|---|---|
| Etiquetas semánticas | Hecho |
| Formularios con `label for` y `required` | Hecho |
| Imágenes con `alt` descriptivo | Hecho |
| Navegación con `aria-label` | Hecho |
| Tabla con `thead`, `tbody`, `th`, `td` | Hecho |
| Variables CSS | Hecho |
| Layout con Grid y Flexbox | Hecho |
| Transiciones `:hover`, `:focus`, `:active` | Hecho |
| Animaciones con `@keyframes` (hero, botones, tarjetas) | Pendiente |
| Breakpoints (≤600px, 601–992px, ≥993px) | Pendiente |
| Modo oscuro con `prefers-color-scheme` (opcional) | Pendiente |

## Capturas de pantalla

| Escritorio | Tablet | Móvil |
|---|---|---|
| ![Escritorio](assets/capturas/escritorio.png) | ![Tablet](assets/capturas/tablet.png) | ![Móvil](assets/capturas/movil.png) |

## Créditos de imágenes

Las fotografías provienen de sitios con licencia gratuita. Completar con el autor y el sitio de cada una:

| Archivo | Autor | Fuente |
|---|---|---|
| `johan.jpg` | [Autor] | [Pexels / Unsplash] |
| `katherine.jpg` | [Autor] | [Pexels / Unsplash] |
| `luisa.jpg` | [Autor] | [Pexels / Unsplash] |
| `sebastian.jpg` | [Autor] | [Pexels / Unsplash] |
| `auto-manual.jpg` | [Autor] | [Pexels / Unsplash] |
| `auto-automatico.jpg` | [Autor] | [Pexels / Unsplash] |
| `suv.jpg` | [Autor] | [Pexels / Unsplash] |
| `auto-doble-pedal.jpg` | [Autor] | [Pexels / Unsplash] |
| `moto-125.jpg` | [Autor] | [Pexels / Unsplash] |
| `moto-150.jpg` | [Autor] | [Pexels / Unsplash] |

Las imágenes se optimizaron con [Squoosh](https://squoosh.app) (ancho de 800 px, MozJPEG, calidad 75).

Los íconos de redes sociales provienen de [Simple Icons](https://simpleicons.org) (licencia CC0).
## Notas

- Los datos de la academia (nombres, teléfonos, licencias, direcciones) son ficticios y con fines académicos.
- El botón "Solicitar cita" y los filtros de vehículos son simulaciones con enlaces `href`, porque el proyecto no usa JavaScript.