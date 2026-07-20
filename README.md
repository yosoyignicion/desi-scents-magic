# ✨ Desi Scents Magic

> **Alquimia botánica artesanal — Velas de Ritual & Wax Melts**

Bienvenido al repositorio de la web oficial de **Desi Scents Magic**, el pequeño taller artesanal de **Desi** (una amiga emprendedora 🧚🏽‍♀️). Un espacio digital que refleja la calidez, el misticismo y el amor por lo hecho a mano que hay detrás de cada vela y cada bombón de cera perfumada.

Puedes ver el resultado final aquí (GitHub Pages): [https://yosoyignicion.github.io/Desi-Scents-Magic/](https://yosoyignicion.github.io/Desi-Scents-Magic/)

---

## 🧭 Mapa del Proyecto

```
Desi-Scents-Magic/
├── desi_scents_magic.html   ← web completa (single-page)
├── README.md                ← ¡esto!
└── ... (en el futuro: assets, imágenes reales, etc.)
```

---

## 🌙 ¿Qué es Desi Scents Magic?

**Desi Scents** es un emprendimiento artesanal que fabrica:

- 🕯️ **Velas de Ritual** — vertidas a mano con cera de soja 100% natural, decoradas con flores del bosque y cristales naturales purificados bajo el influjo de la luna.
- ✨ **Wax Melts** (bombones de cera) — hiperconcentrados, para fundir en quemador y liberar fragancias duraderas por toda la casa.
- 🌿 **Aromas personalizados** — velas a medida con la gema, aroma e intención ritual que el cliente elija (paz, energía, enfoque, relajación).

Todo **orgánico, biodegradable y libre de tóxicos**. Desi pone el alma en cada lote ❤️

---

## 🎨 Diseño Conceptual / Misticismo Digital

### 🤔 La Idea

La web debía transmitir **exactamente lo que se siente al abrir una caja de Desi Scents**: calidez, fantasía, cuidado artesanal, un toque de misterio y la sensación de que estás adquiriendo algo único e irrepetible.

Nada de plantillas genéricas de Shopify. Esto es **un rincón mágico hecho a mano**, como sus productos.

### 🎭 Paleta Visual

| Color | Código | Significado |
|-------|--------|-------------|
| `magicDark` | `#05020a` | El lienzo del cosmos — oscuridad profunda que hace brillar cada detalle |
| `magicVoid` | `#0d071a` | El vacío estelar — fondos de sección con un susurro de púrpura |
| `magicGold` | `#f3cd6e` | La llama de la vela — dorado cálido que guía la mirada |
| `magicLilac` | `#c39bfb` | El aura fantasía — lila suave de hada |
| `golden hover` | `#ffe49e` | Brillo máximo — el destello cuando pasas el ratón |

### 📜 Tipografía Mágica

Usamos **3 fuentes** de Google Fonts, cada una con una función muy concreta:

1. **Bonheur Royale** (`mystic`) — la caligrafía mística que da título al hero. Esa fuente cursiva y fluida que parece escrita con pluma mágica.
2. **Cinzel** (`serif`) — la estructura clásica. Titulares, secciones, precios. Aporta el empaque elegante de una joyería mística.
3. **Montserrat** (`sans`) — el cuerpo de texto legible. Descripciones de productos, párrafos informativos. La lectura cómoda que no cansa.

### 🪄 Efectos Visuales Destacados

**✨ Cosmic Starfield (canvas interactivo)**
- El fondo de la web es un lienzo de estrellas + polvo de hadas que **sigue el cursor** (o el dedo en móvil).
- Cuando mueves el ratón aparecen destellos dorados y lilas que se desvanecen. Es la magia del "polvo de hadas".
- Las estrellas titilan suavemente con cambios de opacidad — 110 estrellas entre dorado y lila.

**🕯️ Llama de vela animada en SVG**
- En la sección "Alquimia" hay una vela ritual dibujada con SVG puro.
- La llama tiene su propia animación CSS (`flame-flicker`) que simula el parpadeo real del fuego.
- La vela flota suavemente arriba y abajo (`gentle-float`) — como si levitara en un altar.

**🏛️ Glassmorphism (cartas de cristal místico)**
- Todas las tarjetas (productos, testimonios, sección comunidad) usan `backdrop-filter: blur(16px)` con fondos semitransparentes.
- Al pasar el ratón se iluminan los bordes, la tarjeta se eleva 4px y aparece una sombra lila.

**✨ Texto con brillo (gold/lilac glow)**
- Los títulos principales tienen `text-shadow` con destellos.
- El texto dorado usa un gradiente (`text-gold-gradient`) que va del dorado claro al bronce.
- El texto lila hace lo mismo con tonos púrpura.

---

## 🧩 Estructura de la Web

Es una **Single Page Application (SPA)** con navegación por anclas — todo en un solo `.html`:

```
┌─────────────────────────────────────────────┐
│  🧙 HEADER FLOTANTE (glassmorphism)        │
│  [Desi Scents MAGIC]  INICIO | ALQUIMIA... │
├─────────────────────────────────────────────┤
│  🌟 HERO — "Wax Melts & Velas"             │
│  (Título místico + 3 pilares fundacionales) │
├─────────────────────────────────────────────┤
│  🔬 ALQUIMIA — Proceso artesanal           │
│  (SVG vela animada + descripción del taller)│
├─────────────────────────────────────────────┤
│  🛍️ COLECCIÓN — 4 productos destacados    │
│  (Catálogo con precios y carrito)           │
├─────────────────────────────────────────────┤
│  📦 COFRES — Pack Iniciación Alquímica     │
│  (Bundle especial con descuento)            │
├─────────────────────────────────────────────┤
│  💬 CLUB SECRETO — Comunidad Telegram      │
│  (Llamada a la acción comunidad)            │
├─────────────────────────────────────────────┤
│  ⭐ TESTIMONIOS — Almas Armonizadas        │
│  (3 reseñas de clientas reales)             │
├─────────────────────────────────────────────┤
│  🦶 FOOTER — Branding + CLP + Legal        │
│  (Compromiso de seguridad cosmética)        │
└─────────────────────────────────────────────┘
```

### Cada sección explicada:

1. **Header** — Nav fija con glassmorphism, logotipo en Bonheur Royale, y botón del carrito (que es una varita mágica ✨). Al hacer scroll se compacta automáticamente.

2. **Hero (Inicio)** — El gran impacto visual. Título con la caligrafía mística, subtítulo con la propuesta de valor, dos CTA principales (catálogo + proceso), y **los 3 pilares**: Velas de Ritual, Hechizo de Aromas (wax melts), Ingredientes Sagrados.

3. **Alquimia (Proceso)** — Explica cómo se hacen los productos. Incluye un SVG de vela animada con llama parpadeante y círculos de runas girando. 3 sellos de calidad: aromas premium, hecho a mano, 100% orgánico.

4. **Colección (Catálogo)** — 4 productos en grid responsivo (1→2→4 columnas). Cada uno con badge (edición mística, top ventas), emoji decorativo, descripción y botón de añadir al carrito con efecto hover.

5. **Cofres (Packs)** — Tarjeta destacada con el pack "Iniciación Alquímica", que incluye vela + wax melts + quemador cerámico con descuento.

6. **Comunidad (Club Secreto)** — Invitación al canal de Telegram con botón azul estilo Telegram.

7. **Testimonios** — 3 reseñas de clientas con iniciales en círculos decorativos.

8. **Footer** — Branding, enlaces rápidos, aviso de seguridad CLP (normativa europea de esencias).

---

## 🛒 Sistema de Carrito (JavaScript vanilla)

La web incluye un carrito de compra **completamente funcional como simulación**:

| Función | Descripción |
|---------|-------------|
| `addToCart()` | Añade producto con nombre, precio y emoji |
| `toggleCart()` | Abre/cierra el drawer lateral (cofre alquímico) |
| `changeQty()` | Aumenta/disminuye cantidad o elimina si llega a 0 |
| `removeItem()` | Elimina un artículo |
| `updateCartUI()` | Refresca el badge, total y lista de items |
| `showToast()` | Notificación tipo toast con glassmorphism |
| `simulateCheckout()` | Abre modal de pago PayPal simulado |
| `confirmSimulatedPayment()` | Finaliza la compra simulada |

El carrito usa un **drawer lateral** con animación slide (transform + transition). El badge de la varita mágica muestra el número de artículos con un contador animado.

---

## 🌌 Efecto Estelar (Canvas + JS)

El `canvas` del fondo es un **sistema de partículas** que renderiza:

- **110 estrellas** que titilan entre dorado (`#f3cd6e`) y lila (`#c39bfb`)
- **Polvo de hadas interactivo** que sigue al ratón
- **Detección táctil** — también funciona en móvil con `touchmove`
- **Limitador de distancia** — evita saturación al mover el ratón rápido

Datos técnicos:
- `maxStars = 110` estrellas
- `radius: 0.3 — 1.8px` (partículas pequeñas y elegantes)
- `decay: 0.015 — 0.04` (desvanecimiento controlado)
- `requestAnimationFrame` para animación fluida a 60fps

---

## 📐 Stack Técnico

| Tecnología | Para qué |
|------------|----------|
| **HTML5 semántico** | Estructura accesible y con sentido |
| **Tailwind CSS** (CDN) | Estilizado utility-first rápido, sin build step |
| **CSS3 personalizado** | Animaciones, glassmorphism, scrollbar, keyframes |
| **Canvas API** | Fondo estelar interactivo + polvo de hadas |
| **SVG inline** | Vela ritual animada con gradientes |
| **Google Fonts** | Bonheur Royale + Cinzel + Montserrat |
| **Font Awesome 6** | Iconos místicos (varitas, lunas, estrellas) |
| **JavaScript vanilla** | Carrito, notificaciones, canvas, interacciones |
| **GitHub Pages** | Hosting gratuito y部署 |

**Cero dependencias.** Sin React, sin build tools, sin backend. Un solo archivo HTML autocontenido.

---

## 🎯 Principios de Diseño Aplicados

1. **Mobile-first** — Todo el layout está pensado para móvil primero, con Tailwind responsive (`sm:`, `md:`, `lg:`).
2. **Glassmorphism consistente** — Las `.glass-card` se reutilizan en toda la web (header, productos, testimonios, packs).
3. **Microinteracciones** — Hover en tarjetas (elevación + brillo de borde), hover en botones (escala + sombra), scroll compacto del header.
4. **Teselación mística** — El divisor decorativo con lunas y estrellas aparece entre secciones clave.
5. **Nebulosas ambientales** — Círculos difuminados de fondo que pulsan suavemente (`.nebula-glow`) creando profundidad.
6. **Accesibilidad** — Atributos `aria-label`, contraste de color adecuado, texto legible en todas las escalas.

---

## 🚀 Cómo usar / Desplegar

### Localmente

Abre el archivo directamente en tu navegador:

```bash
firefox desi_scents_magic.html
# o
xdg-open desi_scents_magic.html
```

Como es HTML puro sin build, simplemente funciona.

### GitHub Pages (ya configurado)

El proyecto está configurado para publicarse con GitHub Pages (rama `main`, raíz del repositorio). Cualquier `push` a la rama principal despliega automáticamente:

```
https://yosoyignicion.github.io/Desi-Scents-Magic/
```

---

## 🔮 Próximos Pasos (ideas para el futuro)

- [ ] Reemplazar emojis por **imágenes reales** de los productos (fotos de las velas y wax melts)
- [ ] Añadir **más productos** al catálogo (nuevos aromas, ediciones limitadas)
- [ ] Formulario de **pedidos personalizados** (elección de aroma, gema e intención)
- [ ] **Galería de Instagram** embebida
- [ ] Implementar **pasarela de pago real** (PayPal Business / Stripe)
- [ ] Zona de **fidelización** con puntos por compra
- [ ] Carrusel de **reseñas con fotos** de clientas reales
- [ ] Sección **"El Proceso"** ampliada con fotos del taller

---

## 👩‍💻 Créditos

- **Desi** — Artesana, alquimista de velas y wax melts, dueña del taller mágico 🧚🏽‍♀️
- **IgniciónDev** (yo) — Diseño UX/UI, desarrollo web, efecto cosmos, carrito interactivo y esta documentación tan bonita 💜

> *Hecho con mucho amor para ayudar a una amiga a dar sus primeros pasos en el mundo mágico del emprendimiento artesanal.* 🌙✨

---

## 📝 Licencia

Proyecto público con fines de promoción de un pequeño negocio artesanal. Si te gusta el diseño, siéntete libre de inspirarte, pero recuerda: **la magia de Desi es única** como ella.

---

*"La magia está en los detalles hechos a mano."*
