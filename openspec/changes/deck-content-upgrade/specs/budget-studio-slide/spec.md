## ADDED Requirements

### Requirement: New Budget Studio slide
A new slide (slide 07) SHALL be added after AI Film Studio, showcasing the Budget Studio product.

#### Scenario: Budget Studio slide exists
- **WHEN** user navigates to the deck
- **THEN** slide 07 displays Budget Studio content with slide-index "07 / 13"

#### Scenario: Budget Studio slide shows product info
- **WHEN** user views the Budget Studio slide
- **THEN** it displays:
  - Title: "Budget Studio"
  - Subtitle: "AI-native production budgeting"
  - Description: Production budgeting tool for film and commercial projects
  - Tech stack: React 18, Vite, Tailwind CSS, Supabase
  - Key features in card format: Contingency/Fringe calc, Cash Flow integration, Budget Versioning, Excel/PDF Export, Dark/Light Theme, Supabase Auth

### Requirement: Budget Studio slide uses existing card layout
- **WHEN** the Budget Studio slide is rendered
- **THEN** it uses the existing `.card-grid-2` or `.card-grid-3` layout with `.card`, `.card-cat`, `.card-name`, `.card-body` classes
