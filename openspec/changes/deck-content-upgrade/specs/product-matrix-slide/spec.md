## ADDED Requirements

### Requirement: New Product Matrix slide
A new slide (slide 08) SHALL be added after Tool Stack, showing all 7 products in a unified view.

#### Scenario: Product Matrix slide exists
- **WHEN** user navigates to the deck
- **THEN** slide 08 displays Product Matrix content with slide-index "08 / 13"

#### Scenario: Product Matrix shows all 7 products
- **WHEN** user views the Product Matrix slide
- **THEN** it displays cards for: OpenClaw, AI Film Studio, Prompt Builder, Budget Studio, AI Canvas Studio, VideoAgent Studio, OpenVideoAgent

#### Scenario: Each product card shows key details
- **WHEN** a product card is rendered
- **THEN** it displays: product name, one-line description, status (shipped/in-progress/open-source), and live URL if available

#### Scenario: Product Matrix uses grid layout
- **WHEN** the slide is rendered on desktop
- **THEN** products are displayed in a 3-column or 4-column grid
