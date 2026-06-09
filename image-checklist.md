# V7 Image Checklist

All images needed for `eric-zheng-deck-v7.html`. Replace placeholder `<div>` elements with actual `<img>` tags.

---

## 1. Hero Portrait (Slide 01)

**File:** `images/hero-portrait.jpg`
**Dimensions:** 380 × 520px (or 2x: 760 × 1040px)
**Style:** Professional headshot or cinematic portrait, warm tones to match gold accent
**Location:** Right side of hero, behind text

**Options:**
- [ ] Professional headshot (film producer aesthetic)
- [ ] Cinematic portrait with warm lighting
- [ ] AI-generated portrait (Midjourney/Flux prompt below)

**AI Prompt (if needed):**
```
Cinematic portrait of an Asian male film producer, 35-40 years old, wearing dark minimalist clothing, warm amber lighting, shallow depth of field, dark background with subtle gold tones, professional headshot style, editorial photography --ar 3:4 --style raw
```

**CSS class:** `.hero-image`
**HTML comment:** `<!-- IMAGE: hero-portrait.jpg -->`

---

## 2. Film Poster (Slide 10)

**File:** `images/film-poster.jpg`
**Dimensions:** 240 × 360px (or 2x: 480 × 720px)
**Style:** Official movie poster or festival still from "Brief History of A Family"
**Location:** Right side of film info, below badges

**Options:**
- [ ] Official movie poster (if available)
- [ ] Festival still from the film
- [ ] Press kit photo
- [ ] AI-generated placeholder (prompt below)

**AI Prompt (if needed):**
```
Film poster for "Brief History of A Family", Chinese family drama, Sundance Film Festival official selection, minimalist design, dark background, gold typography, cinematic composition, award-winning indie film aesthetic --ar 2:3 --style raw
```

**CSS class:** `.film-poster`
**HTML comment:** `<!-- IMAGE: film-poster.jpg -->`

---

## 3. AI Film Studio Screenshot (Slide 06)

**File:** `images/ai-film-studio-screenshot.png`
**Dimensions:** 16:10 aspect ratio (e.g., 1280 × 800px)
**Style:** Dark theme, gate pipeline dashboard showing G0-G7 gates
**Location:** Below 5-View System badges

**Options:**
- [ ] Actual app screenshot (run `npm run dev` and capture)
- [ ] Figma mockup
- [ ] AI-generated UI mockup (prompt below)

**AI Prompt (if needed):**
```
Dark theme dashboard UI for film production software, showing 9 pipeline gates (G0-G7), gold accent color on dark charcoal background, modern web application interface, clean minimalist design, professional SaaS product screenshot --ar 16:10 --style raw
```

**CSS class:** `.product-screenshot`
**HTML comment:** `<!-- IMAGE: ai-film-studio-screenshot.png -->`

---

## 4. Budget Studio Screenshot (Slide 07)

**File:** `images/budget-studio-screenshot.png`
**Dimensions:** 16:10 aspect ratio (e.g., 1280 × 800px)
**Style:** Dark theme, budget interface with contingency/fringe calculation
**Location:** Below tech badges

**Options:**
- [ ] Actual app screenshot (run `npm run dev` in V2/ and capture)
- [ ] Figma mockup
- [ ] AI-generated UI mockup (prompt below)

**AI Prompt (if needed):**
```
Dark theme budget spreadsheet interface for film production, showing contingency and fringe calculations, gold accent numbers on dark background, modern web application, clean data table design, professional financial tool screenshot --ar 16:10 --style raw
```

**CSS class:** `.product-screenshot`
**HTML comment:** `<!-- IMAGE: budget-studio-screenshot.png -->`

---

## 5. Tool Logos (Slide 09)

**Directory:** `images/logos/`
**Dimensions:** 80 × 80px each (square, PNG with transparency)
**Style:** White or light gray logos on transparent background
**Location:** Tool logo grid (12 logos)

**Required logos:**
- [ ] `claude.png` — Anthropic Claude
- [ ] `runway.png` — Runway ML
- [ ] `midjourney.png` — Midjourney
- [ ] `elevenlabs.png` — ElevenLabs
- [ ] `supabase.png` — Supabase
- [ ] `nextjs.png` — Next.js
- [ ] `flux.png` — Flux (Black Forest Labs)
- [ ] `suno.png` — Suno AI
- [ ] `vite.png` — Vite
- [ ] `react.png` — React
- [ ] `tailwind.png` — Tailwind CSS
- [ ] `zustand.png` — Zustand

**Source:** Download from [Simple Icons](https://simpleicons.org/) or official brand kits

**CSS class:** `.tool-logo`
**HTML comment:** `<!-- Tool logos — replace placeholders with actual logo PNGs -->`

---

## Image Directory Structure

```
ai_EZ_DECK/
├── images/
│   ├── hero-portrait.jpg
│   ├── film-poster.jpg
│   ├── ai-film-studio-screenshot.png
│   ├── budget-studio-screenshot.png
│   └── logos/
│       ├── claude.png
│       ├── runway.png
│       ├── midjourney.png
│       ├── elevenlabs.png
│       ├── supabase.png
│       ├── nextjs.png
│       ├── flux.png
│       ├── suno.png
│       ├── vite.png
│       ├── react.png
│       ├── tailwind.png
│       └── zustand.png
└── eric-zheng-deck-v7.html
```

---

## HTML Replacement Examples

### Hero Portrait
```html
<!-- Before (placeholder) -->
<div class="hero-image">
<div class="hero-image-placeholder">PORTRAIT<br>PHOTO</div>
</div>

<!-- After (actual image) -->
<div class="hero-image">
<img src="images/hero-portrait.jpg" alt="Eric Zheng — Film Producer & AI Builder">
</div>
```

### Film Poster
```html
<!-- Before (placeholder) -->
<div class="film-poster">
<div class="film-poster-placeholder">MOVIE<br>POSTER</div>
</div>

<!-- After (actual image) -->
<div class="film-poster">
<img src="images/film-poster.jpg" alt="Brief History of A Family — Official Poster">
</div>
```

### Tool Logo
```html
<!-- Before (placeholder) -->
<div class="tool-logo"><div class="tool-logo-placeholder">CLAUDE</div></div>

<!-- After (actual image) -->
<div class="tool-logo"><img src="images/logos/claude.png" alt="Claude"></div>
```

---

## Priority

| Priority | Image | Impact | Effort |
|----------|-------|--------|--------|
| P0 | Hero portrait | High — first impression | Low — use existing photo |
| P0 | Film poster | High — validates film credentials | Low — use existing poster |
| P1 | AI Film Studio screenshot | Medium — shows actual product | Medium — need to run app |
| P1 | Budget Studio screenshot | Medium — shows actual product | Medium — need to run app |
| P2 | Tool logos | Low — already have text labels | Low — download from Simple Icons |
