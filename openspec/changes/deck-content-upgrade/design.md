## Context

The portfolio deck is a single-file HTML slide deck (`eric-zheng-deck-v5.html`, ~730 lines) with horizontal translateX navigation. It currently has 11 slides, dark prestige cinematic theme, Space Grotesk headings, Barlow Condensed body, and existing hover micro-interactions, responsive breakpoints, and print styles.

Two authoritative content sources exist outside the deck:
1. **Founding 500 submission form** — contains YouTube demo URLs, product descriptions, agent architecture details
2. **SYSTEM_BRAIN** (`_00_SYSTEM_BRAIN/`) — contains Budget Studio, AI Canvas Studio, VideoAgent Studio, OpenVideoAgent details, OpenClaw 8-agent specs, AI Film Studio 5-View architecture

The deck is missing: Eric Zheng's name on the hero page, 4 of 7 products, YouTube video embeds, and detailed agent/product architecture.

## Goals / Non-Goals

**Goals:**
- Fix the critical hero page name omission
- Embed 5 YouTube demo videos in slide 03
- Expand OpenClaw from 3 cards to 8 agent roles with cron schedules
- Add 2 new slides (Budget Studio, Product Matrix) — total 13 pages
- Expand AI Film Studio with 5-View System and Supabase details
- Expand Tool Stack with full 14+ tool inventory
- Add live product URLs to Contact page
- Preserve all existing design system, interactions, and navigation

**Non-Goals:**
- Redesigning the visual theme (already unified dark prestige)
- Changing font choices (Space Grotesk + Barlow Condensed confirmed)
- Adding new CSS frameworks or JS libraries
- Modifying the navigation mechanism (translateX sliding)
- Adding authentication, API calls, or backend logic

## Decisions

### D1: YouTube embed strategy — iframe with lazy loading
**Decision**: Use `<iframe>` with `loading="lazy"` and `allowfullscreen` for YouTube videos.
**Why**: YouTube iframes are the standard embed method, no API key needed, lazy loading prevents 5 simultaneous video loads from killing page performance.
**Alternative considered**: Click-to-play overlay (keep placeholder, open modal on click) — rejected because the user wants immediate visual impact in the deck.
**Implementation**: Each video gets a `.vbox` container with `position:relative; padding-top:56.25%` (16:9) and iframe absolutely positioned inside.

### D2: Slide count change — 11 → 13, JS variable update
**Decision**: Change `t=11` to `t=13` in the JS, add 2 new slide sections, renumber existing slide indices.
**Why**: Minimal JS change, existing navigation logic works for any slide count.
**Risk**: All `01 / 11` through `11 / 11` strings in HTML need updating to `01 / 13` through `13 / 13`.

### D3: New slide placement — Budget Studio after AI Film Studio, Product Matrix after Tool Stack
**Decision**: Insert Budget Studio as slide 07 (after AI Film Studio), Product Matrix as slide 08 (after Tool Stack). Existing slides 08-11 become 10-13.
**Rationale**: Budget Studio is an AI product (fits with AI section), Product Matrix is a summary (fits before Film/Commercial section).

### D4: OpenClaw 8-agent layout — 2×4 grid instead of 3-column
**Decision**: Replace 3 `.card` with 8 smaller cards in a `.card-grid-4` (2 rows of 4).
**Why**: 8 agents need more compact presentation. Each card shows agent name + one-line role.
**Alternative**: Keep 3 columns with 3 rows — too tall for a single slide. 2×4 is more balanced.

### D5: YouTube embed CSS — aspect-ratio on .vbox
**Decision**: Add `aspect-ratio: 16/9` to `.vbox` when it contains an iframe, and use `position: absolute; inset: 0` for the iframe.
**Why**: Existing `.vbox` already has `aspect-ratio: 16/9`, so iframes naturally fit. Just need to make the iframe fill the container.

## Risks / Trade-offs

- **[Performance] YouTube iframes on slide 03** → Mitigated by `loading="lazy"`, videos only load when slide is near viewport
- **[Slide renumbering]** → All hardcoded `XX / 11` strings must be updated; JS progress indicator uses `t` variable so it auto-updates
- **[Content density]** → Some slides (OpenClaw with 8 cards, AI Film Studio with 5-View + gates) may feel crowded → Mitigated by using smaller card sizes and `clamp()` font sizing
- **[Mobile responsive]** → 8-agent grid needs to collapse to 2-column or 1-column on narrow screens → Add to existing `@media (max-width: 980px)` and `@media (max-width: 720px)` breakpoints
