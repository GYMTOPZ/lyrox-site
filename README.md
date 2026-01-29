# JEN AI — lyrox.ai

Landing page for **JEN AI**, an AI-powered fitness coaching platform that handles client coaching 24/7 on WhatsApp, email, and SMS.

**Live:** [lyrox.ai](https://lyrox.ai)

---

## What is JEN AI?

JEN AI is a white-label AI coaching assistant for fitness coaches. It learns a coach's style and handles all client communication — workout programming, nutrition plans, form analysis, check-ins — across WhatsApp, email, and SMS. Coaches bring the clients, JEN does everything else.

### Key Metrics
- **$35K/mo** revenue
- **280** active clients
- **87%** margins
- **$0** customer acquisition cost
- **30%** churn (down from 70%)

---

## Tech Stack

**Zero dependencies. Single file. Deploy anywhere.**

| Component | Technology |
|-----------|-----------|
| Structure | Single `index.html` (~65KB) |
| Styling | Inline CSS, no frameworks |
| Animations | [GSAP 3.12](https://greensock.com/gsap/) + [ScrollTrigger](https://greensock.com/scrolltrigger/) |
| Text Effects | [SplitType](https://www.npmjs.com/package/split-type) |
| Smooth Scroll | [Lenis 1.0](https://lenis.studiofreight.com/) |
| Fonts | [Archivo](https://fonts.google.com/specimen/Archivo) + [Plus Jakarta Sans](https://fonts.google.com/specimen/Plus+Jakarta+Sans) (Google Fonts) |
| Hosting | [Vercel](https://vercel.com) |

External scripts loaded from CDN:
```
https://cdn.jsdelivr.net/gh/studio-freight/lenis@1.0.23/bundled/lenis.min.js
https://cdnjs.cloudflare.com/ajax/libs/gsap/3.12.5/gsap.min.js
https://cdnjs.cloudflare.com/ajax/libs/gsap/3.12.5/ScrollTrigger.min.js
https://unpkg.com/split-type
```

---

## Design System

Design inspired by [yolkk.com](https://www.yolkk.com) — adapted for JEN AI's brand and content.

### Colors
| Variable | Value | Usage |
|----------|-------|-------|
| `--white` | `#fffffd` | Primary text |
| `--black` | `#141414` | Background |
| `--green` | `#2e4f5e` | Accent, hover grid |
| `--green-dark` | `#16212a` | Card backgrounds, sections |
| `--grey-dark` | `#aeaeae` | Muted text, labels |
| `--mint` | `#00E5A0` | AI accent, highlights, CTA |
| `--grey` | `#f1f1f1` | Borders |
| `--review-yellow` | `#f1d511` | Star rating |

### Typography
- **Display/Headings:** Archivo (weights: 200–900)
- **Body:** Plus Jakarta Sans (weights: 400–700)
- **Base font-size:** 1.25rem
- **Heading scale:** h1: 6rem → h5: 1.25rem (responsive)

### Breakpoints
| Breakpoint | Target |
|-----------|--------|
| `991px` | Tablet |
| `767px` | Mobile landscape |
| `479px` | Mobile portrait |

---

## Page Sections

### 1. Page Transition Cover
Black overlay with "JEN AI" text. Fades in, then slides up with `power3.inOut` easing on page load.

### 2. Navbar
- Fixed, 80px height, transparent
- Scrolls → `rgba(20,20,20,.85)` with `backdrop-filter: blur(20px)`
- **Stagger link hover:** Per-character text animation with `text-shadow` trick (Yolkk-style)
- **Underline hover:** `::before` pseudo-element, `scaleX(0)` → `scaleX(1)`, `1.2s cubic-bezier(.625,.05,0,1)`
- **Sibling fade:** Hovering a nav link dims siblings to 50% opacity

### 3. Hero — "The Awakening"
- Full viewport height with starfield background
- **Starfield:** 3 layers of CSS `box-shadow` stars (1px/2px/3px) animating diagonally at 100s/125s/175s
- **Shooting stars:** 3 animated streaks, 15s cycle, grow from 5px to 800px height
- **Color overlays:** 3 blurred circles (`filter: blur(120px)`) that fade to 12% opacity
- **Mouse hover grid:** 100 invisible div boxes with `radial-gradient` that light up on hover
- **Blur-bento cards:** Glassmorphism — `backdrop-filter: blur(15px)`, `rgba(255,255,253,.05)` background
- **Hero text:** Word-by-word reveal using GSAP + SplitType after page transition

### 4. Marquees (3 instances between sections)
- GSAP-powered infinite scroll with `xPercent: -100`
- **Scroll direction reversal:** Marquee direction flips when user changes scroll direction
- **Parallax scrub:** Horizontal position tied to scroll via ScrollTrigger
- **Dual rows:** Large heading (opacity .3) + smaller subheadings in reverse direction
- Content duplicated via JS for seamless loop

### 5. Chat Demo — "This is how JEN coaches"
- iPhone mockup with WhatsApp-style chat interface
- Auto-plays coaching conversation on scroll (IntersectionObserver trigger)
- 6-message scripted conversation with typing indicators
- User can type their own messages (pre-scripted AI responses)
- Right column: 3 stat cards (24/7, <3s, $100/mo) with character-split reveal

### 6. Before / After — "The Transformation"
- Split grid: "Without JEN" (red accent) vs "With JEN" (mint accent)
- SVG icons with colored borders
- Center tagline with word-by-word reveal
- 3 stat cards with animated counters (scroll-triggered)

### 7. How It Works — 3 Steps
- Connect → AI Learns → Clients Thrive
- Cards start at 15% opacity, stagger-activate on scroll
- Active state: mint border glow, icon color change

### 8. Data Wall — Traction
- 5-column grid (Bloomberg terminal aesthetic)
- Animated counters: `requestAnimationFrame` with cubic ease-out
- $35K/mo · 280 clients · 87% margins · $0 CAC · 30% churn

### 9. Vision — "The Platform Play"
- Apple-style large text with word-by-word clip-path reveal
- "Shopify had stores. Uber had drivers. JEN AI has coaches."
- Scaling grid: 10 coaches → $840K, 40 → $3.36M, 100 → $8.4M

### 10. Footer
- 5-column grid (1.4fr 1fr 1fr 1fr .75fr)
- Starfield background + shooting star
- CTA buttons: "I'm a coach" (Yolkk button) + "I'm an investor" (secondary)
- Mouse hover grid overlay
- Links: Product, Company, Platform, Social

---

## Animation System

### `anm-scroll-text` (Custom attribute system)
Every text element uses data attributes to configure its reveal animation:

```html
<h2 anm-scroll-text anm-split="words" anm-distance="50%" anm-delay="0.2">
  Your text here
</h2>
```

| Attribute | Default | Description |
|-----------|---------|-------------|
| `anm-scroll-text` | — | Enables scroll-triggered reveal |
| `anm-split` | none | SplitType mode: `words`, `chars`, or `words,chars` |
| `anm-distance` | `40px` | Initial Y offset |
| `anm-delay` | `0` | Animation delay in seconds |
| `anm-duration` | `1.2` | Animation duration |
| `anm-ease` | `power3.out` | GSAP easing |
| `anm-chars-stagger` | `0.02` | Stagger between characters |
| `anm-words-stagger` | `0.06` | Stagger between words |

**Behavior:**
- Elements in viewport on load: animate after page transition (1.2s base delay)
- Elements below viewport: animate when 25% visible (desktop) or 15% (mobile)
- Animation: `clip-path` reveal + `translateY` + opacity

### Lenis + GSAP Integration
```js
lenis.on('scroll', ScrollTrigger.update);
gsap.ticker.add((time) => { lenis.raf(time * 1000); });
gsap.ticker.lagSmoothing(0);
```
This syncs Lenis smooth scrolling with GSAP's ScrollTrigger for buttery animations.

---

## File Structure

```
lyrox-site/
├── index.html          # Complete landing page (HTML + CSS + JS)
├── README.md           # This file
└── PROJECT-CONTEXT.md  # Business context and positioning (if present)
```

---

## Deployment

### Vercel (recommended)
```bash
# Install Vercel CLI
npm i -g vercel

# Deploy from project root
cd lyrox-site
vercel

# Set custom domain
vercel domains add lyrox.ai
```

### Any static host
Just serve `index.html`. No build step, no dependencies to install.

---

## Development

Open locally:
```bash
open index.html
# or
python3 -m http.server 8000
# then visit http://localhost:8000
```

### Key CSS patterns used
- **Glassmorphism:** `backdrop-filter: blur()` + semi-transparent backgrounds + borders
- **Yolkk button:** `border: 2px solid white` + rotating inner gradient circle
- **Sibling fade:** Parent `:hover` dims children, hovered child restores opacity
- **Starfield:** Pure CSS `box-shadow` with `translateX/Y` keyframes

### Key JS patterns
- **GSAP timelines** with ScrollTrigger for scroll-linked animations
- **SplitType** for word/character-level text animations
- **Lenis** for momentum-based smooth scrolling
- **IntersectionObserver** fallback for chat demo trigger
- **requestAnimationFrame** counter animations with cubic ease-out

---

## Contact

- **Website:** [lyrox.ai](https://lyrox.ai)
- **Email:** hello@lyrox.ai
- **Coach inquiries:** coach@lyrox.ai
- **Investor inquiries:** invest@lyrox.ai

---

## License

Proprietary. All rights reserved.
