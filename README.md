# Root: A Woodland Game of Might and Right - Proyecto Completo

## 📋 Resumen del Proyecto

Este es un proyecto web profesional y responsivo basado en las especificaciones exactas del PDF proporcionado. Consiste en un sitio web de 5 páginas para el juego de mesa "Root: A Woodland Game of Might and Right".

---

## 📁 Estructura de Carpetas

```
DAM1M4-TrabajoHTML/
├── index.html              # Página principal (Hero, animación scroll, SVG)
├── instrucciones.html      # Guía con 6 pasos + tarjetas animadas ⭐ (PUNTO OBLIGATORIO)
├── historia.html           # Lore con carrusel CSS puro (sin JavaScript)
├── contacto.html           # Formulario con validación regex
├── about.html              # Equipo + vídeo YouTube
│
├── css/
│   ├── global.css          # Reset, tipografía, variables de color
│   ├── layout.css          # Header, footer, menú hamburguesa, grids
│   ├── components.css      # Hero, cards, forms, carrusel, etc.
│   └── animations.css      # Scroll animations, hover, SVG, transiciones
│
└── assets/
    └── img/                # CARPETA PARA IMÁGENES (ver lista abajo)
```

---

## 📸 Imágenes Requeridas para `assets/img/`

### Imágenes principales (obligatorias):
1. **logo.jpg** - Logo del juego (60x60px)
   - *Prompt IA:* "Professional logo for Root board game with faction symbols in stylized forest"

2. **hero.jpg** - Imagen de fondo hero
   - *Prompt IA:* "Epic fantasy woodland forest scene with mystical atmosphere, dark green and brown tones, high quality professional illustration"

### Capturas de instrucciones (instrucciones.html):
3. **captura1.jpg** - Setup inicial del juego
   - *Prompt IA:* "Root board game setup with game board, pieces, cards laid out on table"

4. **captura2.jpg** - Fase Birdsong
   - *Prompt IA:* "Root board game player taking preparation phase with decision cards"

5. **captura3.jpg** - Fase Daylight
   - *Prompt IA:* "Root board game mid-turn action phase with multiple pieces and cards"

6. **captura4.jpg** - Batalla
   - *Prompt IA:* "Root board game battle scene with dice rolled and combat happening"

7. **captura5.jpg** - Fase Evening
   - *Prompt IA:* "Root board game end of turn phase with scoring and card draw"

8. **captura6.jpg** - Victoria
   - *Prompt IA:* "Root board game victory screen showing winning player and final score"

### Tarjetas de facciones (instrucciones.html):
9. **card1.jpg** - Marquise de Cat
   - *Prompt IA:* "Professional illustration of cat faction leader - industrial, powerful, wooden aesthetic, high quality"

10. **card2.jpg** - Eyrie Dynasties
    - *Prompt IA:* "Professional illustration of bird/eagle faction noble in tower, elegant, decrepit, high quality"

11. **card3.jpg** - Woodland Alliance
    - *Prompt IA:* "Professional illustration of woodland rebellion alliance mice and foxes, underground, revolutionary, high quality"

12. **card4.jpg** - Vagabond
    - *Prompt IA:* "Professional illustration of wandering vagabond character with items and relics in forest"

### Imágenes del carrusel (historia.html - 8 imágenes):
13. **hero-marquise.jpg** - Marquise invasión
    - *Prompt IA:* "Marquise de Cat invasion of woodland, industrial machines, sawmills, conquest theme"

14. **hero-eyrie.jpg** - Eyrie en torre
    - *Prompt IA:* "Eyrie Dynasties in their high tower, birds flying, decadent castle, noble setting"

15. **hero-alliance.jpg** - Alliance revolución
    - *Prompt IA:* "Woodland Alliance underground revolution, hidden bases, sympathetic gathering, mystical"

16. **hero-vagabond.jpg** - Vagabond en ruinas
    - *Prompt IA:* "Lone vagabond wanderer in forest ruins with magical items and artifacts"

17. **hero-batalla.jpg** - Batalla épica
    - *Prompt IA:* "Epic multi-faction battle in woodland clearing with various creatures fighting"

18. **hero-riverfolk.jpg** - Riverfolk comercio
    - *Prompt IA:* "Riverfolk otter merchants trading on rivers, commerce, medieval market aesthetic"

19. **hero-lizard.jpg** - Lizard Cult
    - *Prompt IA:* "Lizard Cult mystical ritual with reptiles and sacred gardens, dark magical"

20. **hero-panorama.jpg** - Panorama Woodland
    - *Prompt IA:* "Beautiful panoramic view of ancient woodland forest, mystical, ancestral, peaceful"

### Secciones de lore (historia.html):
21. **lore-genesis.jpg** - Paraíso perdido
    - *Prompt IA:* "Ancient paradise woodland forest untouched, peaceful animals, golden age"

22. **lore-eyrie.jpg** - Eyrie decadencia
    - *Prompt IA:* "Eyrie nobility in decline, tragedy, broken dreams, gothic atmosphere"

23. **lore-alliance.jpg** - Alliance poder
    - *Prompt IA:* "Woodland Alliance uprising and revolution, power from below, momentum"

24. **lore-vagabond.jpg** - Vagabond libertad
    - *Prompt IA:* "Vagabond wanderer free in wilderness, independence, mysterious, shadowy"

25. **lore-riverfolk.jpg** - Riverfolk comercio
    - *Prompt IA:* "Riverfolk trade routes and commerce on rivers, wealthy otters, prosperity"

26. **lore-lizard.jpg** - Lizard primordial
    - *Prompt IA:* "Lizard Cult ancient primordial power, sacrifice, sacred, mystical"

27. **lore-legacy.jpg** - Legado
    - *Prompt IA:* "Root board game legacy and lasting impact, epic stories, community, victory"

### Equipo (about.html):
28. **avatar-1.jpg** - Tu avatar
    - *Prompt IA:* "Professional portrait of game developer, creative, professional headshot"

29. **avatar-2.jpg** - Cole Wehrle
    - *Prompt IA:* "Professional portrait of game designer Cole Wehrle, thoughtful, visionary"

30. **avatar-3.jpg** - Kyle Ferrin
    - *Prompt IA:* "Professional portrait of artist illustrator, creative, artistic"

31. **avatar-4.jpg** - Equipo Leder Games
    - *Prompt IA:* "Group photo of game design team working together at table"

32. **avatar-5.jpg** - Comunidad
    - *Prompt IA:* "Diverse gaming community playing board games together, happy, inclusive"

---

## ✅ CHECKLIST DE REQUISITOS CUMPLIDOS

### Estructura y Organización
- ✅ 5 páginas HTML (index, instrucciones, historia, contacto, about)
- ✅ 4 archivos CSS organizados (global, layout, components, animations)
- ✅ Carpeta assets/img/ para imágenes
- ✅ Rutas relativas (funciona offline)

### Header Común (Todas las páginas)
- ✅ Logo + Nombre del juego
- ✅ Menú horizontal con 5 enlaces
- ✅ Hamburguesa animada para móvil
- ✅ Estética profesional con gradientes

### Footer Común (Todas las páginas)
- ✅ Copyright alineado a la derecha
- ✅ Iconos Material Icons (Twitter, Instagram, Facebook, TikTok)
- ✅ Tooltips en hover
- ✅ Animaciones en hover (scale 1.2, color shift a dorado)

### Página Principal (index.html)
- ✅ Hero con imagen de fondo y overlay
- ✅ Animación de scroll (5 párrafos fade-in secuencial)
- ✅ SVG animado (orbe girando 360°)
- ✅ Sección "¿Cómo se juega?" con 6 mecánicas
- ✅ Enlace a instrucciones.html

### Página de Instrucciones (instrucciones.html) ⭐
- ✅ Título y introducción
- ✅ 6 pasos detallados con capturas grandes (grid 2-col)
- ✅ Sección de mecánicas con accordion (CSS puro)
- ✅ **4 TARJETAS ANIMADAS CON HOVER** (PUNTO OBLIGATORIO)
  - Tarjeta Marquise: imagen + hover scale 1.15 + rotate 3deg + inner glow
  - Tarjeta Eyrie: imagen + hover scale 1.15 + rotate 3deg + inner glow
  - Tarjeta Alliance: imagen + hover scale 1.15 + rotate 3deg + inner glow
  - Tarjeta Vagabond: imagen + hover scale 1.15 + rotate 3deg + inner glow

### Página de Historia (historia.html)
- ✅ Título y introducción
- ✅ **CARRUSEL CSS PURO (sin JavaScript)**
  - 8 imágenes que rotan automáticamente
  - Animación 40s linear infinite
  - Pausa en hover (animation-play-state)
  - Captions overlay fade-in
- ✅ 6 secciones de lore con historia narrativa
- ✅ Imágenes intercaladas con textos

### Página de Contacto (contacto.html)
- ✅ Dirección inventada
- ✅ Google Maps embed (iframe real)
- ✅ Teléfono con enlace tel:
- ✅ Email con enlace mailto:
- ✅ **FORMULARIO CON VALIDACIÓN REGEX**
  - Nombre: pattern="^[a-záéíóúñA-ZÁÉÍÓÚÑ\s]{3,60}$"
  - Teléfono: pattern="^\+?[0-9\s\-\(\)]{10,15}$"
  - Email: pattern="^[a-zA-Z0-9._%-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$"
  - Textarea con maxlength=1000 y contador
  - Validación en tiempo real con CSS .is-valid / .is-invalid
  - Mensajes de error y success

### Página About Us (about.html)
- ✅ Título y introducción
- ✅ 5 miembros del equipo con bios detalladas
- ✅ Cards con avatar, nombre, rol, bio
- ✅ Vídeo YouTube embed (iframe real)
- ✅ Sección de cierre con legado

### CSS - Especificaciones
- ✅ **SIN CSS INCRUSTADO en HTML** (todo en archivos externos)
- ✅ Google Fonts: 'Playfair Display' (títulos) + 'Open Sans' (texto)
- ✅ Colores exactos del PDF:
  - Fondo: #228B22 (verde bosque)
  - Secundario: #8B4513 (marrón madera)
  - Accent: #FFD700 (dorado)
  - Dark: #0F4C0F (verde oscuro)
- ✅ Sombras Pixelmator-style: box-shadow: 0 4px 8px rgba(0,0,0,0.3)
- ✅ Layout con Grid (3-col desktop, 1-col móvil) y Flexbox
- ✅ Transiciones 0.4s en hovers
- ✅ Reutilización completa de estilos

### Responsividad
- ✅ Desktop (1200px+): 3 columnas
- ✅ Tablet (768px-1024px): 2 columnas
- ✅ Mobile (< 768px): 1 columna
- ✅ Menú hamburguesa con animación en móvil
- ✅ Viewport meta tag
- ✅ Imágenes escalables

### Animaciones
- ✅ Scroll fade-in en adventure section (Intersection Observer)
- ✅ SVG rotación 12s linear infinite
- ✅ Card hover: scale 1.15 + rotate 3deg + glow
- ✅ Button hover: translateY(-2px) + glow
- ✅ Carrusel CSS: 40s linear infinite con keyframes
- ✅ Accordion: :checked + CSS toggle (sin JavaScript)
- ✅ Entrada de elementos staggered (animation-delay)
- ✅ Shake animation en campo form inválido

### Formulario Avanzado
- ✅ Validación con HTML5 + regex
- ✅ Feedback visual CSS (borders rojo/verde)
- ✅ Error messages dinámicos
- ✅ Success message con transición
- ✅ Contador de caracteres en textarea
- ✅ No envía (novalidate + preventDefault)

---

## 🚀 CÓMO USAR

1. **Descargar todos los archivos:**
   - 5 archivos HTML
   - 4 archivos CSS
   - Crear carpeta `assets/img/`

2. **Generar imágenes con IA:**
   - Usar prompts proporcionados arriba
   - Colocar en `assets/img/`
   - Nombres exactos: logo.jpg, hero.jpg, captura1.jpg, etc.

3. **Abrir en navegador:**
   - Doble-click en `index.html`
   - O usar Live Server en VS Code
   - Navegar con el menú

4. **Pruebas:**
   - Responsive: F12 → Toggle device toolbar
   - Formulario: Rellenar y probar validación
   - Carrusel: Esperar animación auto o hacer hover
   - Accordion: Hacer click en items
   - Cards: Hover sobre tarjetas de instrucciones

---

## 🎨 COLORES Y ESTÉTICA

```css
--color-primary: #228B22;      /* Verde bosque profundo */
--color-secondary: #8B4513;    /* Marrón madera rústica */
--color-accent: #FFD700;       /* Dorado brillante */
--color-dark: #0F4C0F;         /* Verde muy oscuro */
--color-light: #F5F5DC;        /* Beige claro */
--color-error: #C8102E;        /* Rojo */
--color-success: #2ECC71;      /* Verde éxito */
```

---

## 📱 BREAKPOINTS

- Desktop: 1200px+
- Tablet: 768px - 1024px
- Mobile: < 768px

---

## ✨ PUNTOS DESTACADOS

1. **Header y Footer:** Idénticos en todas las páginas, estética profesional AAAda.
2. **Instrucciones (⭐):** 4 tarjetas animadas con hover épico - PUNTO OBLIGATORIO CUMPLIDO.
3. **Historia:** Carrusel CSS puro 100% (sin JavaScript).
4. **Contacto:** Validación regex completa con feedback visual.
5. **About:** Vídeo YouTube real + equipo detallado.
6. **Responsive:** Funciona perfecto en móvil, tablet, desktop.
7. **Animaciones:** Scroll, hover, SVG, entrada staggered.
8. **Accesibilidad:** Contraste, focus visible, semantic HTML.

---

## 📝 NOTAS IMPORTANTES

- **CSS puro:** Sin Bootstrap, sin Tailwind, todo CSS vanilla bien organizado.
- **Contenido ampliado:** 500-800 palabras por página (como especifica PDF).
- **Rutas relativas:** Funciona sin servidor web.
- **Sin localStorage:** Sin APIs de browser storage (sandbox).
- **Validación:** Regex exhaustiva, no envía formulario (preventDefault).

---

## 🎯 PRÓXIMOS PASOS (Opcional)

1. Generar todas las imágenes con IA
2. Ajustar rutas si es necesario
3. Probar en diferentes navegadores
4. Optimizar imágenes (comprimir)
5. Añadir más contenido si es necesario

---

**Proyecto completado según especificaciones exactas del PDF.** 
Desarrollado con pasión por la excelencia en web design profesional. ✨

