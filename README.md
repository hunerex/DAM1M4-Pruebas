# DOCUMENTACIÓN TÉCNICA: ROOT - A WOODLAND GAME WEBSITE

## Estructura de Carpetas Completa

```
DAM1M4-TrabajoHTML/
│
├── index.html                 (Página principal - Hero, mecánicas, SVG, scroll anim)
├── instrucciones.html         (6 pasos detallados + tarjetas interactivas)
├── historia.html              (Carrusel + 5 secciones narrativas)
├── contacto.html              (Mapa, info contacto, formulario con regex)
├── about.html                 (Equipo, video YouTube, valores, premios)
│
├── css/
│   ├── global.css             (Resets, variables CSS, tipografía, utilidades)
│   ├── layout.css             (Header, footer, grids responsivos, hamburguesa)
│   ├── components.css         (Botones, cards, hero, formularios, carrusel)
│   └── animations.css         (Keyframes puras, scroll triggers, parallax, SVG)
│
├── assets/
│   ├── img/
│   │   ├── logo.jpg           (Logo Root 60x60px)
│   │   ├── hero.jpg           (Hero background 1920x1080px)
│   │   ├── captura1.jpg       (Setup inicial)
│   │   ├── captura2.jpg       (Birdsong phase)
│   │   ├── captura3.jpg       (Daylight action)
│   │   ├── captura4.jpg       (Battle resolution)
│   │   ├── captura5.jpg       (Evening phase)
│   │   ├── captura6.jpg       (Victory screen)
│   │   ├── card1.jpg          (Marquise faction card)
│   │   ├── card2.jpg          (Eyrie faction card)
│   │   ├── card3.jpg          (Alliance faction card)
│   │   ├── card4.jpg          (Vagabond faction card)
│   │   ├── imagen1.jpg        (Marquise invasión)
│   │   ├── imagen2.jpg        (Eyrie en torre)
│   │   ├── imagen3.jpg        (Alliance revuelta)
│   │   ├── imagen4.jpg        (Vagabond solitario)
│   │   ├── imagen5.jpg        (Batalla multi-facción)
│   │   ├── imagen6.jpg        (Riverfolk comercio)
│   │   ├── imagen7.jpg        (Lizard Cult ritual)
│   │   ├── imagen8.jpg        (Woodland panorámico)
│   │   ├── team1.jpg          (Alejandro Martín)
│   │   ├── team2.jpg          (María García)
│   │   ├── team3.jpg          (Carlos Ruiz)
│   │   ├── team4.jpg          (Elena Sánchez)
│   │   ├── team5.jpg          (David López)
│   │   └── team6.jpg          (Sandra Vega)
│   │
│   └── svg/                   (Opcional: SVGs externos)
│       └── woodland-orb.svg   (SVG del orbe animado)
│
└── README.md                  (Este archivo)
```

---

## Especificaciones Técnicas

### Meta Tags SEO
- **Title Tags:** Únicos por página, keywords en español
- **Meta Descriptions:** <160 chars, keywords naturales
- **Charset:** UTF-8 (crítico para acentos españoles)
- **Viewport:** width=device-width, initial-scale=1.0
- **Schema.org:** BoardGame markup en index.html

### Accesibilidad (WCAG 2.1 AA)
- **ARIA:** role="banner", role="navigation", role="main", role="contentinfo", role="region"
- **Alt Text:** Descriptivos extensos en español (ej: "Ilustración de la Marquise de Cat conquistando el bosque")
- **Focus States:** Outline 2px solid #FFD700 con offset
- **Form Labels:** <label> asociados con for="" en todos campos
- **Color Contrast:** Ratio >4.5:1 (texto oscuro #1A1A1A sobre fondos claros)

### Performance
- **Lazy Loading:** loading="lazy" en todas imágenes
- **CSS Modular:** global.css < 15KB, components.css < 20KB
- **Sin JavaScript:** Menuero hamburguesa CSS puro (checkbox hack)
- **Image Optimization:** <200KB por imagen (1920x1080 hero, 300x400 cards)
- **Minificación:** Facilitar via minifier online (comentarios removidos)

### Responsividad
- **Mobile-First:** Base styles para <768px
- **Breakpoints:**
  - `@media (max-width: 768px)` - Tablets/móviles
  - `@media (min-width: 769px)` - Desktops
  - `@media (min-width: 1200px)` - Wide screens
- **Grids Flexibles:** `grid-template-columns: repeat(auto-fit, minmax(280px, 1fr))`
- **Typography Responsive:** `font-size: clamp(1rem, 2vw, 1.5rem)`

---

## Guías de Implementación de Imágenes

### Prompts IA para Generar Imágenes (DALL-E, Midjourney, etc.)

#### Logo
```
Crea un logo vectorial minimalista de 60x60px para "Root: A Woodland Game". 
Incluye siluetas de cuatro facciones (gato, ave, conejo, errante) rodeando 
un árbol estilizado. Colores: verde bosque #228B22 y dorado #FFD700. 
Estilo: Leder Games, profesional, memorable.
```

#### Hero Background
```
Fondo épico de bosque denso para 1920x1080px. Muestra clearing central 
rodeado de árboles antiguos, con siluetas de facciones en acción estratégica. 
Estilo realista-fantasía, colores dominantes verdes (#228B22) y marrones (#8B4513), 
iluminación crepuscular que sugiere intriga. Atmósfera de juego de mesa premium. 
Optimizado para web <200KB.
```

#### Capturas de Juego (6 total)
```
Captura ficticia de alta resolución de [FASE]. Muestra:
- Mapa modular con 12 clearings conectados
- Meeples de facciones en posiciones específicas
- Cartas repartidas, tokens VP visibles
- Mesa de madera, iluminación natural
- Estilo fotográfico realista de juego de mesa
- Resolución 1200x800px, optimizada para web

Ejemplos:
- captura1: Setup inicial (todos componentes desplegados)
- captura2: Fase Birdsong (cartas prep visibles)
- captura3: Daylight (warriors moviendo)
- captura4: Battle resolution (dados, hits resolviéndose)
- captura5: Evening phase (VP check, cards drawn)
- captura6: Victory screen (ganador celebrando)
```

#### Tarjetas de Facciones (4)
```
Ilustración de [FACCIÓN] en estilo Leder Games, 300x400px:

Card1 - Marquise: Gato antropomórfico en armadura industrial, talando árbol 
con maquinaria, colores marrón/oro, dominante presencia.

Card2 - Eyrie: Águila noble en torre celestial, rodeada de pergaminos 
(decretos), verdes/azules, majestuoso pero decadente.

Card3 - Alliance: Multitud de roedores (ratones, conejos, zorros) en cueva 
subterránea, símbolos de revolución, verdes/rojos revolucionarios.

Card4 - Vagabond: Figura misteriosa solitaria rodeada de ítems (espada, 
antorcha, monedas), sombras, dorados, oportunista.
```

#### Carrusel Historia (8 imágenes)
```
Serie de ilustraciones 1200x600px para carrusel historia:

imagen1: Invasión Marquise - Maquinaria felina talando bosque primordial
imagen2: Eyrie en Torre - Dinástica aviaria en roost elevado decadente
imagen3: Alliance Revuelta - Levantamiento guerrillero multiespecies
imagen4: Vagabond - Mercader solitario entre ruinas con ítems mágicos
imagen5: Batalla - Conflicto multi-facción épico en clearing central
imagen6: Riverfolk - Otters comerciantes en ríos del Woodland
imagen7: Lizard Cult - Rituales oscuros, sacrificios, dios reptil
imagen8: Woodland Panorámico - Vista aérea de todo territorio,conflictivo

Estilo: Consistente Leder Games, paleta #228B22/#8B4513/#FFD700, 
narrativo, histórico inspirado, 150-180KB cada.
```

#### Equipo (6 retratos)
```
Retratos profesionales 300x350px para equipo (estilo ilustración o foto 
profesional ficticia):

team1: Alejandro Martín - Director Creativo, aire de liderazgo visionary
team2: María García - Diseñadora, enfoque analítico, precisión
team3: Carlos Ruiz - Art Director, paleta rica, expresión creativa
team4: Elena Sánchez - Escritora, ambiente narrativo, profundidad
team5: David López - Dev Frontend, focus tecnológico, profesional
team6: Sandra Vega - Gestora, energía colaborativa, liderazgo

Estilo: Retratos corporativos pero cálidos, fondo sutil (verde/madera), 
luz profesional, cada uno refleja rol. 80-120KB cada.
```

---

## Notas de Testing y Debugging

### Verificación de Responsividad

#### Chrome DevTools Simulation
1. Abre DevTools (F12)
2. Simula dispositivos:
   - iPhone SE (375px) - Menú hamburguesa visible, grids collapse a 1 columna
   - iPad (768px) - 2 columnas máximo, aún hamburguesa
   - Desktop (1920px) - Full layout 3-4 columnas, menú horizontal
3. Prueba **orientation change** (horizontal/vertical)

#### Checklist Responsividad
- [ ] Menú hamburguesa se abre/cierra suavemente sin saltos
- [ ] Imágenes escalan manteniendo proporciones (max-width: 100%)
- [ ] Texto nunca se corta (no overflow-x)
- [ ] Botones >44px (touch-friendly en móvil)
- [ ] Cards apilan verticalmente en móvil
- [ ] Formulario inputs son usables con teclado
- [ ] SVG orb es visible y centrado en todos tamaños

### Verificación de Animaciones

#### Cross-Browser
- **Chrome/Edge:** Todas animaciones fluidas
- **Firefox:** Verificar @keyframes, transiciones suaves
- **Safari:** Scroll animations pueden necesitar -webkit-, parallax funciona
- **Mobile Safari (iOS):** Parallax deshabilitado, scroll-triggered anims fallback OK

#### Testing Animaciones Específicas
1. **Hero Fade-in:** Debería animar entrada suave 1s
2. **Scroll Adventure:** Artículos deberían fade-in al scrollear (view timeline)
3. **SVG Woodland Orb:** Debería rotar 12s linear infinito, pausar on hover
4. **Carrusel Historia:** Slide automático 40s, pausa on hover
5. **Card Hovers:** Scale 1.05 + shadow lift suave 0.3s
6. **Button Ripple:** Click CTA debería crear ripple effect (::before)

#### Fallbacks para Navegadores Antiguos
- Sin soporte scroll() timeline: Usar opacity inicial, JS polyfill, o accept no animation
- Sin soporte calc(): Fallback a fixed pixel values
- Sin soporte CSS Grid: Fallback a Flexbox para grids simples

### Validación de Formulario

#### Test Regex Patterns
```html
<!-- Nombre: ^[a-zA-ZáéíóúÁÉÍÓÚñÑ\s]{3,50}$ -->
✓ "Juan García" (válido)
✓ "María-José" (falla - need dash pattern)
✗ "JG" (demasiado corto)

<!-- Teléfono: ^\+?[0-9\s\-\(\)]{9,15}$ -->
✓ "+34 91 234 5678" (válido)
✓ "(91) 234-5678" (válido)
✗ "123" (demasiado corto)

<!-- Email: ^[^\s@]+@[^\s@]+\.[^\s@]+$ -->
✓ "usuario@ejemplo.com" (válido)
✗ "usuario@" (falta dominio)

<!-- Asunto: ^.{5,100}$ -->
✓ "Pregunta sobre reglas" (válido)
✗ "Hola" (demasiado corto)

<!-- Mensaje: minlength=10, maxlength=500 -->
✓ "Tengo una pregunta sobre Root..." (válido)
✗ "Hola" (demasiado corto)
```

#### Testing Manual del Formulario
1. Submit vacío → Ver asteriscos required
2. Email inválido (sin @) → Border rojo, aviso
3. Teléfono con letras → Falla pattern, feedback visual
4. Todo válido → Borde verde (input:valid) ✓
5. Focus estados → Outline dorado visible

### Verificación SEO

#### Lighthouse Audit
1. Abre DevTools → Lighthouse tab
2. Audit for: Performance, Accessibility, Best Practices, SEO
3. Targetear: Performance >85%, Accessibility >95%, SEO >90%

#### Checklist SEO Específico
- [ ] H1 único por página (no múltiples)
- [ ] H2-H3 jerárquicos (sin saltos)
- [ ] Meta description presente y <160 chars
- [ ] Keywords naturales en contenido (no keyword stuffing)
- [ ] Links internos descriptivos (no "click aquí")
- [ ] Alt text en todas imágenes
- [ ] Schema.org markup (BoardGame en index)
- [ ] Sitemap.xml generado (manual)
- [ ] robots.txt básico (allow: /)

### Testing de Accesibilidad

#### WAVE Chrome Extension
1. Instala WAVE (Web Accessibility Evaluation Tool)
2. Corre en cada página
3. Zero "Errors", minimizar "Warnings"

#### Screen Reader Testing (NVDA/JAWS)
- [ ] Texto leído en orden lógico
- [ ] Links tienen descripción (aria-label o context)
- [ ] Formulario campos labeled
- [ ] SVG tiene role="img" con descripción
- [ ] Header/footer/main landmarks identificables

#### Keyboard Navigation
- [ ] Tab navegador through todos links/botones
- [ ] Focus visible siempre (outline dorado)
- [ ] Menú hamburguesa accessible vía keyboard (aria-expanded)
- [ ] Formulario sumible con Enter
- [ ] Escape cierra menú

### Debugging Común

#### Problema: Imágenes no cargan
**Causa:** Rutas relativas incorrectas
**Fix:** Verificar rutas: `assets/img/logo.jpg` (no `../assets`)
**Check:** Abrir DevTools → Network tab, ver 404s

#### Problema: CSS no aplica
**Causa:** Typos en class names, CSS not linked
**Fix:** Verificar `<link rel="stylesheet" href="css/global.css">`
**Check:** DevTools → Styles tab, ver si CSS cargó

#### Problema: Menú hamburguesa no cierra en mobile
**Causa:** JavaScript inexistente (usamos CSS pure, necesita click)
**Fix:** Agregar `<label>` para `input[type="checkbox"]`
**Check:** Verificar checkbox está checked/unchecked

#### Problema: SVG no anima
**Causa:** @keyframes no aplicadas, o animation-play-state
**Fix:** Verificar `animation: rotateClockwise 12s linear infinite;` aplicado
**Check:** DevTools → Elements, ver computed styles

#### Problema: Scroll animations no funcionan
**Causa:** View timeline no soportado en navegador
**Fix:** Agregar fallback sin animation-timeline (initial opacity 1)
**Check:** Caniuse.com para animation-timeline support

#### Problema: Formulario no valida visualmente
**Causa:** input:invalid pseudo-class no styled
**Fix:** Agregar `input:invalid { border-color: red; }`
**Check:** Escribir email sin @, debería ver borde rojo

---

## Notas de Performance

### Optimización de Imágenes
1. **Compresión:** Usar TinyPNG o ImageOptim antes upload
2. **Formato:** JPEG para fotos, PNG para gráficos
3. **Responsive:** Generar versiones small (600w), medium (1200w)
4. **Lazy Loading:** `loading="lazy"` en todas imágenes (nativas browser)

### Minificación CSS
```bash
# Usar online minifier: https://minifier.org
# Pega global.css, descarga minificado
# Renombra a global.min.css, reemplaza link en HTML
```

### Caching Headers (si deploying)
```
Cache-Control: public, max-age=31536000 (1 año para assets)
ETag headers para invalidation
```

### Recomendaciones de Hosting
- Netlify (gratuito, fast deploys, CDN global)
- Vercel (si futuro Node.js)
- GitHub Pages (estático puro)
- Local: `python -m http.server` en carpeta raíz

---

## Pruebas Locales Paso a Paso

### Windows/Mac/Linux

1. **Descarga archivos** a carpeta `DAM1M4-TrabajoHTML/`
2. **Abre terminal** en la carpeta
3. **Inicia servidor local:**
   ```bash
   # Python 3
   python -m http.server 8000
   
   # O Node.js (si instalado)
   npx http-server
   
   # O simplemente abre index.html en navegador (sin servidor, rutas relativas funcionan)
   ```
4. **Navega a** `http://localhost:8000` o `file:///.../index.html`
5. **Prueba en DevTools:**
   - F12 → Responsive Design Mode
   - Test diferentes breakpoints
   - Check Console para errores
   - Check Network para asset loading

---

## Validación HTML/CSS

### W3C Validator
- Copiar HTML → https://validator.w3.org
- Esperar validación, fijar errores (ej: unclosed tags)

### CSS Validator
- Copiar CSS → https://jigsaw.w3.org/css-validator
- Esperar, revisar warnings (ej: vendor prefixes)

---

## Próximos Pasos para Producción

1. **Reemplazar imágenes ficticias** con reales (o generar con IA)
2. **Agregar sitemap.xml** (lista de páginas para SEO)
3. **Crear robots.txt** (controlar web crawlers)
4. **Setup analytics** (Google Analytics 4)
5. **SSL certificate** (HTTPS)
6. **Monitor Lighthouse** regularmente

---

## Créditos y Licencias

- **Playfair Display & Open Sans:** Google Fonts (Open License)
- **Material Icons:** Google (Apache 2.0)
- **HTML/CSS Código:** DAM1M4 Team (Educacional)
- **Root: A Woodland Game:** Leder Games (IP protegida, fines educativos)

---

**Documento generado:** Diciembre 11, 2025
**Versión:** 1.0 Final
**Status:** Producción Ready