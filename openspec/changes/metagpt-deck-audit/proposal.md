## Why

The portfolio deck (`eric-zheng-deck-v5.html`) was upgraded from 11 to 13 slides in a single session with rapid content additions. Before using this deck for job applications (Founding 500, HyperAgent, LinkedIn), it needs a systematic audit to catch code quality issues, UX inconsistencies, accessibility gaps, and content errors that were introduced during the expansion. Similar to the MetaGPT product validation done for AI Film Studio (24 fixes), this audit ensures the deck is production-ready.

## What Changes

- Fix HTML semantic issues (missing lang attribute, heading hierarchy, alt text equivalents)
- Fix CSS inconsistencies (unused classes, duplicate selectors, missing responsive rules)
- Fix JavaScript edge cases (navigation state, dot count, keyboard handling)
- Fix content issues (broken links, inconsistent terminology, missing data)
- Improve accessibility (ARIA labels, focus management, screen reader support)
- Improve performance (font loading, CSS efficiency, iframe lazy loading)
- Improve responsive design (edge cases at breakpoints, overflow handling)
- Improve print styles (page breaks, color contrast, hidden elements)

## Capabilities

### New Capabilities
- `html-semantic-audit`: HTML structure, semantics, heading hierarchy, meta tags
- `css-quality-audit`: CSS consistency, unused rules, duplicate selectors, specificity
- `js-navigation-audit`: JavaScript navigation logic, state management, edge cases
- `content-consistency-audit`: Content accuracy, broken links, terminology consistency
- `accessibility-audit`: ARIA labels, focus management, keyboard navigation, screen reader
- `responsive-audit`: Breakpoint behavior, overflow, touch targets, mobile UX
- `print-style-audit`: Print media queries, page breaks, color contrast for print
- `performance-audit`: Font loading, CSS efficiency, iframe handling, animation performance

### Modified Capabilities
<!-- None — this is a new audit, not modifying existing specs -->

## Impact

- **File**: `ai_EZ_DECK/eric-zheng-deck-v5.html` (single file, all changes here)
- **Dependencies**: None (pure HTML/CSS/JS, no build step)
- **Risk**: Low — all changes are within one file, easily reversible via git
- **Testing**: Manual browser testing at 4 breakpoints + print preview
