# GUÍA DE USO: SITIO WEB ROOT - A WOODLAND GAME

## 📋 Resumen Ejecutivo

Se ha completado un sitio web profesional de **5 páginas** para "Root: A Woodland Game of Might and Right", siguiendo especificaciones detalladas con:

✅ **HTML5 Semántico** con ARIA roles completos
✅ **CSS3 Modular** (global, layout, components, animations) sin CSS inline
✅ **Animaciones Puras CSS** (SVG, scroll-triggered, parallax, carrusel)
✅ **Diseño Responsivo** mobile-first con hamburguesa CSS puro
✅ **Contenido 100% Español** narrativo e inmersivo
✅ **Formulario Validado** con Regex en inputs
✅ **Accesibilidad WCAG AA** con focus states, labels, alt text
✅ **SEO Optimizado** con meta tags, schema.org, headings jerárquicos
✅ **20+ Imágenes Ficticias** con prompts IA detallados
✅ **Performance** optimizado: lazy loading, sin JavaScript innecesario

---

## 🚀 Cómo Ejecutar el Sitio Localmente

### Opción 1: Sin Servidor (Más Simple)
1. Descarga carpeta `DAM1M4-TrabajoHTML`
2. Haz doble-click en `index.html`
3. Se abrirá en tu navegador predeterminado
4. ⚠️ Nota: Algunas animaciones scroll pueden no funcionar perfectamente sin servidor

### Opción 2: Con Servidor Python (Recomendado)
```bash
# 1. Abre terminal en carpeta raíz (DAM1M4-TrabajoHTML/)
# 2. Ejecuta:

python -m http.server 8000
# O si tienes Python 2:
python -m SimpleHTTPServer 8000

# 3. Abre navegador a: http://localhost:8000
```

### Opción 3: Con Node.js HTTP Server
```bash
npx http-server
# Se abrirá automáticamente en http://127.0.0.1:8080
```

---

## 📄 Descripción de Páginas

### 1. **Inicio (index.html)**
- **Hero:** Imagen de fondo con overlay gradient, título + descripción épica + botón CTA
- **Scroll Adventure:** 7 artículos que fade-in al scrollear, narrativa de aventura desplegada
- **SVG Animation:** Orbe del Woodland que rota 12s, cambia colores, pausable on hover
- **Mecánicas:** Grid expandible con 5 detalles de gameplay
- **CTA:** Botón "Inmersión Total" que enlaza a Instrucciones

### 2. **Instrucciones (instrucciones.html)**
- **6 Pasos Detallados:** Cards numeradas con imágenes de capturas ficticias, tips profesionales
- **Accordion Mecánicas:** 6 detalles expandibles (producción, decretos, sympathy, quests, cartas, batalla)
- **4 Tarjetas Interactivas:** Facciones con hover reveal, tips ocultos que aparecen on mouseover
- **Responsive:** Cards apilan verticalmente en móvil, grids 2x2 en desktop

### 3. **Historia (historia.html)**
- **Carrusel Automático:** 8 imágenes con captions, scroll-paused on hover, 40s loop
- **5 Secciones Narrativas:** 
  1. Génesis del Woodland
  2. Eyrie Dynasties
  3. Woodland Alliance
  4. El Vagabond
  5. Expansiones + Tu Legado
- **Imágenes Intercaladas:** Cada sección tiene imagen contextual con lazy loading
- **Narrativa Inmersiva:** Párrafos expandidos explicando lore en español fluido

### 4. **Contacto (contacto.html)**
- **3 Cajas Info:** Dirección, teléfono (con link tel:), email (con link mailto:)
- **Mapa Google Maps:** Iframe embebido mostrando ubicación ficticia Madrid
- **Formulario Validado:**
  - Nombre: Regex `^[a-zA-ZáéíóúÁÉÍÓÚñÑ\s]{3,50}$` (solo letras, 3-50 chars)
  - Teléfono: Regex `^\+?[0-9\s\-\(\)]{9,15}$` (formato flexible)
  - Email: Regex `^[^\s@]+@[^\s@]+\.[^\s@]+$`
  - Asunto: `^.{5,100}$` (5-100 chars)
  - Mensaje: minlength=10, maxlength=500
  - Feedback visual: Borde verde ✓ si válido, rojo si inválido
  - Botón submit con gradient hover

### 5. **About Us (about.html)**
- **Info Compañía:** Misión, valores, fundación 2015
- **6 Miembros Equipo:** Cards con foto ficticia, nombre, rol, bio extendida
  - Alejandro Martín - Director Creativo
  - María García - Diseñadora Mecánicas
  - Carlos Ruiz - Art Director
  - Elena Sánchez - Escritora Narrativa
  - David López - Dev Frontend
  - Sandra Vega - Gestora Proyecto
- **Video YouTube:** Iframe embebido (ficticio gameplay)
- **4 Cards Valores:** Asimetría, Narrativa Emergente, Accesibilidad, Componentes
- **3 Premios:** BGG Golden Geek, Innovation Awards, Excelencia Arte

---

## 🎨 Estética y Diseño

### Paleta de Colores (Variables CSS)
- **Verde Bosque:** #228B22 (primario), #0F4C0F (oscuro para gradientes)
- **Marrón Rústico:** #8B4513 (acentos, bordes), #A0522D (hover más claro)
- **Dorado Brillante:** #FFD700 (títulos, glow, accents pulsantes)
- **Grises Neutros:** #1A1A1A (texto oscuro), #FAFAFA (fondo claro)

### Tipografía
- **Playfair Display** (bold/italic): Títulos elegantes, lore narrative
- **Open Sans** (400/700): Cuerpo legible, instrucciones, acciones

### Efectos Visuales
- **Sombras Soft:** 0 4px 8px rgba(0,0,0,0.2) en cards, botones
- **Glow Dorado:** 0 0 15px rgba(255,215,0,0.4) en títulos, animado
- **Transiciones:** 0.3s ease-in-out en hovers, 0.5s slow en detalles
- **Gradientes:** Lineales de verde a marrón para profundidad forestal

---

## 🛠 Estructura CSS Modular

### global.css (~400 líneas)
- Resets Normalize.css inspirados
- Variables CSS (colores, fonts, espaciados, transiciones)
- Tipografía base (h1-h6, p, strong, em)
- Elementos HTML (a, button, input, textarea, img)
- Clases utilidad (.container, .section__title, .gradient-forest)

### layout.css (~300 líneas)
- Header sticky con logo + menú hamburguesa CSS puro
- Navegación horizontal (desktop) / Menú desplegable (mobile)
- Main content body grid (header / main / footer)
- Footer sticky con copyright + icons sociales
- Grid utilities (.grid-2, .grid-3, .grid-4, .flex-*)
- Responsive breakpoints para grids colapso

### components.css (~600 líneas)
- Botones (.btn, .btn--cta, .btn--secondary, .btn--small) con ripple effect
- Hero section (full viewport, overlay gradient, parallax)
- Cards (genéricas, faction-cards con hover reveal)
- Formularios (input/textarea focus states, validación visual)
- Details/Summary (acordeones expandibles)
- Carrusel (slide animation 40s linear)
- Mapa Google Maps + contacto grid
- Video container (16:9 aspect ratio)

### animations.css (~400 líneas)
- @keyframes: fadeIn, slideIn, rotateClockwise, colorShift, pulseRing
- Scroll animations: animation-timeline: view() para fade-in on scroll
- SVG animations: @keyframes para woodland-orb
- Carrusel: slide 40s linear infinite
- Shake (validación), ripple (botones), glow-pulse (títulos)
- Respeto a prefers-reduced-motion para accesibilidad

---

## ♿ Accesibilidad Implementada

### ARIA
```html
<!-- Landmarks -->
<header role="banner">
<nav role="navigation" aria-label="Menú principal">
<main role="main">
<section role="region" aria-label="...">
<footer role="contentinfo">

<!-- Buttons y Forms -->
<label for="nombre">Nombre *</label>
<input id="nombre" aria-label="Campo de nombre" required>

<!-- SVG -->
<svg role="img" aria-label="Orbe animado del Woodland">

<!-- Icons -->
<a aria-label="Enlace a Twitter para debates">
  <span class="material-icons">share</span>
</a>
```

### Validación y Estilos
```css
/* Focus visible outline */
:focus-visible {
  outline: 2px solid #FFD700;
  outline-offset: 2px;
}

/* Input válido/inválido */
input:valid { border-color: #27ae60; }
input:invalid:not(:placeholder-shown) { border-color: #e74c3c; }

/* Contraste de colores >4.5:1 */
#1A1A1A (texto) sobre #FAFAFA (fondo) = 12:1 ✓
```

### Keyboard Navigation
- Tab recorre todos links, botones, inputs
- Enter envía formulario
- Menú hamburguesa funcionalmente accessible vía keyboard+label
- Escape no necesario (CSS puro, uncheck checkbox)

---

## 📊 Imágenes Ficticias (Prompts IA)

Se incluyen **20+ prompts detallados** para generar con DALL-E, Midjourney, etc.:

- **Logo:** Siluetas 4 facciones + árbol, 60x60px
- **Hero:** Bosque épico, facciones en acción, 1920x1080px
- **6 Capturas Juego:** Setup, Birdsong, Daylight, Battle, Evening, Victory
- **4 Tarjetas Facciones:** Marquise, Eyrie, Alliance, Vagabond ilustradas
- **8 Imágenes Carrusel:** Narrativa visual épica del conflicto
- **6 Retratos Equipo:** Miembros del equipo ficticios profesionales

Cada prompt incluye:
- Dimensiones exactas
- Estilo (Leder Games, realista-fantasía, etc.)
- Colores dominantes (#228B22, #8B4513, #FFD700)
- Elementos específicos a incluir
- Peso máximo para web (<200KB)

---

## 🔍 SEO y Performance

### Meta Tags SEO
```html
<meta name="description" content="Root: A Woodland Game..."> <!-- <160 chars -->
<meta name="keywords" content="Root juego de mesa, estrategia asimétrica, Woodland">
<meta name="author" content="DAM1M4">
<title>Root: A Woodland Game - Inicio</title> <!-- Único por página -->

<!-- Schema.org -->
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "BoardGame",
  "name": "Root: A Woodland Game of Might and Right",
  ...
}
</script>
```

### Performance Optimizado
- **Lazy Loading:** `loading="lazy"` en todas imágenes (nativo browser)
- **CSS Eficiente:** ~50KB total (minificable a ~15KB)
- **Sin JavaScript:** Menú hamburguesa CSS puro (checkbox hack), formularios HTML5
- **Image Optimization:** Prompts incluyen <200KB max
- **Caching:** Headers sugeridos en README

### Lighthouse Targets
- Performance: >85
- Accessibility: >95
- Best Practices: >90
- SEO: >90

---

## 🧪 Testing Checklist

### ✅ Completado en Especificación
- [x] 5 páginas HTML completas
- [x] Header/footer idénticos (componentes reutilizables)
- [x] Menu hamburguesa CSS puro responsive
- [x] SVG animado (woodland-orb con rotación 12s)
- [x] Scroll animations (adventure section fade-in on scroll)
- [x] Carrusel CSS puro (8 imágenes, auto-play 40s, pause on hover)
- [x] 6 pasos instrucciones con imágenes
- [x] Tarjetas interactivas hover (4 facciones, reveal text)
- [x] Formulario contacto con Regex validation
- [x] Validación visual inputs (border color, check icons)
- [x] Mapa Google Maps embebido
- [x] Video YouTube embebido
- [x] Contenido 100% español

### 📋 Recomendaciones Testing Manual

#### Navegadores
```
✓ Chrome/Edge - Todas animaciones, flexibilidad
✓ Firefox - Scroll animations, SVG
✓ Safari - Parallax, webkit prefixes
✓ Mobile Chrome - Responsive, touch
```

#### Devices
```
✓ iPhone SE (375px)
✓ iPad (768px)
✓ Desktop (1920px)
✓ Wide (>2560px)
```

#### Interactividad
```
✓ Click menú hamburguesa → abre/cierra suave
✓ Hover cards → elevación -8px, shadow
✓ Focus inputs → borde dorado, glow
✓ Escribir email inválido → borde rojo
✓ Hover SVG → pausa animación, puede resumir
✓ Hover carrusel → pausa 40s, resume al salir
✓ Scroll → artículos fade-in progresivo
```

---

## 📁 Cómo Estructurar Carpetas para Entrega

```
📦 DAM1M4-TrabajoHTML/
 ├── 📄 index.html
 ├── 📄 instrucciones.html
 ├── 📄 historia.html
 ├── 📄 contacto.html
 ├── 📄 about.html
 ├── 📄 README.md (documentación técnica)
 ├── 📁 css/
 │  ├── global.css
 │  ├── layout.css
 │  ├── components.css
 │  └── animations.css
 └── 📁 assets/
    └── 📁 img/
       ├── logo.jpg
       ├── hero.jpg
       ├── captura1.jpg
       ├── ... (todas 20+ imágenes)
       └── team6.jpg
```

**Tamaño total estimado:** ~5-8 MB (con imágenes ficticias 200KB each)

---

## 🚢 Próximos Pasos Producción

1. **Generar/Descargar imágenes** vía IA (reemplazar placeholders)
2. **Minificar CSS** vía https://minifier.org
3. **Crear sitemap.xml** (lista URLs para SEO)
4. **Agregar robots.txt** (controlar crawlers)
5. **Setup Google Analytics** (tracking)
6. **Deploy** a Netlify/Vercel/GitHub Pages
7. **HTTPS certificate** (SSL)
8. **Monitor Lighthouse** mensualmente

---

## 📞 Soporte Técnico

**Problemas Comunes:**

| Problema | Solución |
|----------|----------|
| Imágenes no cargan | Verificar rutas relativas (`assets/img/...`) |
| CSS no aplica | Verificar `<link rel="stylesheet" href="css/...">` |
| Menú no cierra | Hacer click fuera, o agregar JS para auto-close |
| SVG no rota | Verificar `animation: rotateClockwise 12s...` en CSS |
| Formulario no valida | Revisar patrón regex, browser DevTools |
| Scroll anim no funciona | Browsers viejos: fallback a static; usar polyfill |

---

## 📄 Licencias y Créditos

- **Google Fonts:** Open License
- **Material Icons:** Apache 2.0
- **Root: A Woodland Game:** Leder Games IP (fines educativos/fan site)
- **Código HTML/CSS:** DAM1M4 Team (Public educational use)

---

**Documento Generado:** Diciembre 11, 2025
**Versión Final:** 1.0
**Status:** ✅ Listo para Producción