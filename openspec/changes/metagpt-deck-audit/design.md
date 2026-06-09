## Context

The portfolio deck is a single-file HTML application (`eric-zheng-deck-v5.html`, ~900 lines) that was rapidly expanded from 11 to 13 slides in one session. It uses:
- Pure HTML/CSS/JS (no build step, no framework)
- CSS custom properties for theming
- CSS Grid for card layouts
- JavaScript for slide navigation (goTo/go/dots/keyboard)
- YouTube iframe embeds (5 videos)
- Google Fonts (Space Grotesk, Barlow Condensed, Space Mono)
- Responsive design (4 breakpoints)
- Print styles

The rapid expansion introduced potential issues across HTML semantics, CSS consistency, JavaScript edge cases, content accuracy, accessibility, responsive behavior, and print compatibility.

## Goals / Non-Goals

**Goals:**
- Identify and fix all HTML semantic issues (lang attribute, heading hierarchy, meta tags)
- Identify and fix CSS inconsistencies (unused classes, duplicate selectors, missing rules)
- Identify and fix JavaScript edge cases (navigation state, dot count, keyboard handling)
- Identify and fix content issues (broken links, inconsistent terminology, missing data)
- Identify and fix accessibility gaps (ARIA labels, focus management, keyboard navigation)
- Identify and fix responsive edge cases (overflow, touch targets, mobile UX)
- Identify and fix print style issues (page breaks, color contrast, hidden elements)
- Ensure the deck is production-ready for job applications

**Non-Goals:**
- Adding new features or slides
- Changing the visual design or theme
- Adding external dependencies or frameworks
- Changing the file structure (stays single HTML file)
- Performance optimization beyond basic fixes

## Decisions

**Decision 1: Audit approach — systematic per-category**
- Rationale: Each audit category (HTML, CSS, JS, content, a11y, responsive, print) has different tools and techniques. Systematic per-category ensures nothing is missed.
- Alternative: Random spot-checking — rejected because it's unreliable and misses cross-cutting issues.

**Decision 2: Fix in place, no new files**
- Rationale: The deck is a single HTML file. All fixes go into `eric-zheng-deck-v5.html`. No new CSS files, no new JS files, no build step changes.
- Alternative: Extract CSS/JS into separate files — rejected because it changes the deployment model (single file → multiple files).

**Decision 3: Manual testing over automated**
- Rationale: The deck is a visual presentation tool. Automated linters can catch syntax issues but not visual/UX problems. Manual browser testing at each breakpoint is essential.
- Alternative: Automated testing only — rejected because it can't catch visual regressions or UX issues.

**Decision 4: Git commit after each category**
- Rationale: Each audit category produces independent fixes. Committing after each category creates clean rollback points and makes it easy to revert specific changes if needed.
- Alternative: Single commit at the end — rejected because it makes rollback harder if a fix introduces new issues.

## Risks / Trade-offs

- **Risk**: Fixing one thing breaks another → **Mitigation**: Test after each category, git commit for rollback
- **Risk**: Over-optimization (spending time on non-issues) → **Mitigation**: Focus on real problems, not theoretical ones
- **Risk**: Accessibility fixes change visual appearance → **Mitigation**: Use invisible ARIA attributes and semantic HTML, minimize visual changes
- **Risk**: Responsive fixes break desktop layout → **Mitigation**: Test at all 4 breakpoints after each change
