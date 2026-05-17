## ADDED Requirements

### Requirement: Hero page displays Eric Zheng's name
The hero page (slide 01) SHALL display "ERIC ZHENG" prominently above the existing title "Film Producer. AI Builder."

#### Scenario: Name visible on hero page
- **WHEN** user loads the deck and views slide 01
- **THEN** "ERIC ZHENG" is visible in the hero section, positioned above the `.s1-name` heading

#### Scenario: Name uses consistent typography
- **WHEN** the name is rendered
- **THEN** it uses `'Barlow Condensed', sans-serif` with `text-transform: uppercase`, matching the existing `.s1-eyebrow` style for visual consistency

### Requirement: Name does not break existing layout
- **WHEN** the name is added to the hero page
- **THEN** the existing `.s1-name`, `.s1-tagline`, `.s1-meta` elements remain properly positioned without overflow
