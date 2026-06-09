## ADDED Requirements

### Requirement: Print styles SHALL hide navigation
The navigation bar SHALL be hidden in print mode.

#### Scenario: Navigation hidden in print
- **WHEN** the deck is printed
- **THEN** the navigation bar SHALL not appear

### Requirement: Print styles SHALL show all slides
All 13 slides SHALL be visible in print mode, each on its own page.

#### Scenario: All slides in print
- **WHEN** the deck is printed
- **THEN** all 13 slides SHALL be visible, each with a page break after

### Requirement: Print styles SHALL have sufficient contrast
Text in print mode SHALL have sufficient contrast for readability.

#### Scenario: Print contrast
- **WHEN** the deck is printed
- **THEN** all text SHALL have sufficient contrast against the white background

### Requirement: Print styles SHALL hide decorative elements
Grain textures, background lines, and other decorative elements SHALL be hidden in print.

#### Scenario: Decorative elements hidden
- **WHEN** the deck is printed
- **THEN** grain textures and background lines SHALL not appear

### Requirement: Print styles SHALL handle video embeds
Video embeds SHALL be replaced with placeholder text or hidden in print.

#### Scenario: Video embeds in print
- **WHEN** the deck is printed
- **THEN** video embeds SHALL not appear as broken elements
