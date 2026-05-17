## 1. Hero Page Fix

- [x] 1.1 Add "ERIC ZHENG" name element to slide 01 hero section (above `.s1-name`)
- [x] 1.2 Style the name with `.s1-eyebrow` typography (Barlow Condensed, uppercase, 12px, 0.3em letter-spacing)
- [x] 1.3 Adjust `.s1-name` margin-top to accommodate the new name element

## 2. Slide Navigation Update

- [x] 2.1 Update JS variable `t` from 11 to 13
- [x] 2.2 Update all slide-index elements from "XX / 11" to "XX / 13" format
- [x] 2.3 Verify dot pagination creates 13 dots on page load

## 3. YouTube Video Embeds (Slide 03)

- [x] 3.1 Replace 4 placeholder `.vbox` elements with 5 YouTube iframe embeds
- [x] 3.2 Add CSS for iframe containers: `position: relative; padding-top: 56.25%; iframe position: absolute; inset: 0`
- [x] 3.3 Add `loading="lazy"` and `allowfullscreen` attributes to all iframes
- [x] 3.4 Update slide 03 grid to accommodate 5 videos (2-row layout)
- [x] 3.5 Add responsive breakpoints for video grid (2-col at 980px, 1-col at 720px)

## 4. OpenClaw Agent Architecture (Slide 04)

- [x] 4.1 Replace 3 `.card` elements with 8 agent cards in `.agent-grid` layout
- [x] 4.2 Add agent data: General, Engineer, Creator, Advisor, Wiseman, Debugger, Video-Creator, Marketer
- [x] 4.3 Add cron schedule section below agent grid (Daily Brief 08:30, Inbox Triage 09:00/14:00/21:00, Weekly Retro)
- [x] 4.4 Add responsive breakpoints for 8-agent grid (2-col at 980px, 1-col at 720px)

## 5. Budget Studio Slide (New Slide 07)

- [x] 5.1 Insert new slide section after AI Film Studio with slide-index "07 / 13"
- [x] 5.2 Add slide-cat "BUDGET STUDIO" and h2 title "AI-native production budgeting"
- [x] 5.3 Add description paragraph about the tool
- [x] 5.4 Add card grid with 6 feature cards: Contingency/Fringe, Cash Flow, Budget Versioning, Excel/PDF Export, Dark/Light Theme, Supabase Auth
- [x] 5.5 Add tech stack badges: React 18, Vite, Tailwind CSS, Supabase

## 6. Product Matrix Slide (New Slide 08)

- [x] 6.1 Insert new slide section after Budget Studio with slide-index "08 / 13"
- [x] 6.2 Add slide-cat "PRODUCTS" and h2 title "7 products, one studio"
- [x] 6.3 Add card grid with 7 product cards: OpenClaw, AI Film Studio, Prompt Builder, Budget Studio, AI Canvas Studio, VideoAgent Studio, OpenVideoAgent
- [x] 6.4 Each card shows: product name, one-line description, status badge, live URL

## 7. AI Film Studio Details (Slide 06)

- [x] 7.1 Add 5-View System section below existing gate cards (Dashboard, Canvas, Documents, Library, Review)
- [x] 7.2 Add Supabase integration mention in description
- [x] 7.3 Add gate validation logic description (validation, exploration ≠ master, no generation without approval)

## 8. Prompt Builder URL (Slide 05)

- [x] 8.1 Add live URL "ericzheng-lab.github.io/prompt-builder" to Prompt Builder slide

## 9. Tool Stack Expansion (Slide 09)

- [x] 9.1 Expand from 4 cards to 6 cards organized by category
- [x] 9.2 Add categories: AI Orchestration (Claude Code, OpenClaw, ChatGPT), Video (Runway, Seedance, Higgsfield, Hyperframes), Image (GPT-Image-2, Flux 2 Max, Midjourney, Nano Banana), Audio (ElevenLabs, Suno, MiMo TTS), Frameworks (Next.js 16, React 18, Vite, Tailwind), Data (Supabase, Zustand, ReactFlow)
- [x] 9.3 Add usage frequency context for key tools

## 10. Contact Live URLs (Slide 13)

- [x] 10.1 Add 4 live product URLs to contact list: ai.drsfilms.com, video-canvas.pages.dev, videoagent-studio.vercel.app, prompt-builder
- [x] 10.2 Use existing `.contact-list` styling with label + value pairs

## 11. Slide Renumbering

- [x] 11.1 Renumber existing slides 07-11 to 09-13
- [x] 11.2 Update all slide-index elements to match new numbering
- [x] 11.3 Update slide-cat labels if needed

## 12. Responsive & Print Verification

- [x] 12.1 Test all new slides at 1440px, 980px, 720px, 480px viewports
- [x] 12.2 Verify YouTube embeds render correctly at all breakpoints
- [x] 12.3 Verify 8-agent grid collapses properly on narrow screens
- [x] 12.4 Verify print styles work with 13 slides (page breaks)
- [x] 12.5 Verify navigation (Prev/Next, keyboard, dots) works with 13 slides
