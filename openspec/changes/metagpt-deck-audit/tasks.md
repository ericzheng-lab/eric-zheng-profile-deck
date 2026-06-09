## 1. HTML Semantic Audit

- [x] 1.1 Add `lang="en"` to `<html>` tag
- [x] 1.2 Add `<meta name="description" ...>` tag
- [x] 1.3 Verify heading hierarchy (one h1, sequential h2s)
- [x] 1.4 Add `<section>` or `<article>` wrappers for slides missing semantic elements
- [x] 1.5 Verify all list-like content uses proper `<ul>`/`<ol>` elements

## 2. CSS Quality Audit

- [x] 2.1 Remove unused CSS classes (check each class against HTML usage)
- [x] 2.2 Remove duplicate CSS selectors
- [x] 2.3 Verify all CSS custom properties are defined in `:root`
- [x] 2.4 Add responsive rules for `video-grid` and `agent-grid` at 480px breakpoint
- [x] 2.5 Audit `!important` declarations — justify or remove each one
- [x] 2.6 Fix any CSS specificity issues (high-specificity selectors that could be simplified)

## 3. JavaScript Navigation Audit

- [x] 3.1 Verify `t=13` matches actual slide count
- [x] 3.2 Verify dot pagination creates exactly 13 dots
- [ ] 3.3 Test forward navigation from slide 12 → 13 (last slide)
- [ ] 3.4 Test backward navigation from slide 1 → 1 (boundary)
- [ ] 3.5 Test rapid clicking — no skipped slides or inconsistent state
- [x] 3.6 Verify progress indicator format "XX / 13" with zero-padding

## 4. Content Consistency Audit

- [x] 4.1 Verify all 5 YouTube URLs are valid and accessible
- [ ] 4.2 Verify all 4 live product URLs are correct
- [x] 4.3 Check terminology consistency (OpenClaw, AI Film Studio, etc.)
- [x] 4.4 Verify slide indices match slide comments (01-13)
- [x] 4.5 Scan for placeholder text (Lorem ipsum, TODO, TBD)
- [ ] 4.6 Verify contact information is accurate

## 5. Accessibility Audit

- [x] 5.1 Add `aria-label` to PREV/NEXT buttons
- [x] 5.2 Add `title` attribute to all 5 YouTube iframes
- [ ] 5.3 Check color contrast ratios (WCAG AA: 4.5:1 normal, 3:1 large)
- [ ] 5.4 Add visible focus states for all interactive elements
- [ ] 5.5 Verify touch targets are minimum 44x44px on mobile
- [x] 5.6 Add `role="navigation"` to nav element if missing

## 6. Responsive Audit

- [ ] 6.1 Test all slides at 1440px — no overflow
- [ ] 6.2 Test all slides at 980px — grids collapse to 2-col
- [ ] 6.3 Test all slides at 720px — grids collapse to 1-col
- [ ] 6.4 Test all slides at 480px — no horizontal scroll
- [ ] 6.5 Verify video embeds maintain 16:9 aspect ratio at all breakpoints
- [ ] 6.6 Verify navigation is tappable/clickable at 480px
- [ ] 6.7 Check text overflow at each breakpoint

## 7. Print Style Audit

- [x] 7.1 Verify navigation is hidden in print
- [x] 7.2 Verify all 13 slides appear with page breaks
- [x] 7.3 Verify grain textures and background lines are hidden
- [ ] 7.4 Verify text contrast on white background
- [x] 7.5 Verify video embeds don't appear as broken elements

## 8. Performance Audit

- [x] 8.1 Verify Google Fonts use `display=swap`
- [x] 8.2 Verify all iframes have `loading="lazy"`
- [x] 8.3 Check for redundant CSS rules
- [x] 8.4 Verify `prefers-reduced-motion` support is complete
- [ ] 8.5 Optimize SVG grain texture if oversized

## 9. Final Verification

- [ ] 9.1 Git commit all fixes with descriptive message
- [ ] 9.2 Manual browser test at all 4 breakpoints
- [ ] 9.3 Verify all 13 slides render correctly
- [ ] 9.4 Verify navigation works (Prev/Next, keyboard, dots)
- [ ] 9.5 Verify YouTube embeds load and play
