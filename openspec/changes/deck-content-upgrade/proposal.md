## Why

The portfolio deck (`eric-zheng-deck-v5.html`) is missing critical content from two authoritative sources: the Founding 500 submission form and the SYSTEM_BRAIN knowledge base. The hero page doesn't even display Eric Zheng's name — a fundamental oversight for a personal portfolio. Additionally, 4 of 7 products are completely absent from the deck, YouTube demo videos aren't embedded, and the OpenClaw agent architecture is underspecified. This deck is Eric's primary visual asset for job applications, client pitches, and the HyperAgent program — it needs to reflect the full scope of what's been built.

## What Changes

- **Critical fix**: Add "ERIC ZHENG" prominently to the hero page (slide 01)
- **Slide 03 AI Videos**: Replace 4 placeholder video boxes with YouTube embed links (5 videos total)
- **Slide 04 OpenClaw**: Upgrade from 3 generic cards to 8 specific agent roles + cron schedule details
- **Slide 05 Prompt Builder**: Add live URL (ericzheng-lab.github.io/prompt-builder)
- **Slide 06 AI Film Studio**: Add 5-View System, Supabase integration, gate validation logic
- **Slide 07 Tool Stack**: Expand with full stack (14+ tools with usage frequency)
- **Slide 11 Contact**: Add 4 live product URLs
- **NEW Slide 08**: Budget Studio — AI-native production budgeting tool (React 18 + Vite + Supabase)
- **NEW Slide 09**: Product Matrix — showing all 7 products with status and URLs
- Renumber existing slides 08-11 to 10-13 (total 13 pages)
- Update navigation JS to handle 13 slides instead of 11

## Capabilities

### New Capabilities
- `hero-name-display`: Adding Eric Zheng's name prominently to the hero page
- `youtube-video-embeds`: Embedding YouTube videos in slide 03 with responsive aspect ratios
- `openclaw-agent-architecture`: Detailed 8-agent role breakdown with cron schedules
- `budget-studio-slide`: New slide showcasing Budget Studio product
- `product-matrix-slide`: New slide showing all 7 products in a unified view
- `contact-live-urls`: Adding live product URLs to contact page

### Modified Capabilities
- `ai-film-studio-details`: Expanding AI Film Studio slide with 5-View System and Supabase
- `tool-stack-expansion`: Expanding tool stack with full technology inventory
- `slide-navigation`: Updating JS to support 13 slides instead of 11

## Impact

- Single file modified: `ai_EZ_DECK/eric-zheng-deck-v5.html`
- HTML: 2 new slide sections, modifications to 6 existing slides, hero page fix
- CSS: Responsive adjustments for YouTube embeds (16:9 aspect ratio), new card layouts for Budget Studio and Product Matrix
- JS: Slide count `t` changes from 11 to 13, progress indicator update
- External dependencies: YouTube iframe embeds (no API keys needed)
- No breaking changes to navigation, print styles, or micro-interactions
