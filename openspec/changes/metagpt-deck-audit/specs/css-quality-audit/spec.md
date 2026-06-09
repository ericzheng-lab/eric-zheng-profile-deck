## ADDED Requirements

### Requirement: CSS SHALL not have unused classes
All CSS classes defined in the stylesheet SHALL be used in the HTML.

#### Scenario: Unused class detection
- **WHEN** the CSS is analyzed for unused classes
- **THEN** all defined classes SHALL have at least one corresponding element in the HTML

### Requirement: CSS SHALL not have duplicate selectors
Each CSS selector SHALL appear only once in the stylesheet.

#### Scenario: Duplicate selector check
- **WHEN** the CSS is analyzed for duplicate selectors
- **THEN** no selector SHALL appear more than once (excluding media query variations)

### Requirement: CSS custom properties SHALL be consistent
All CSS custom properties SHALL be defined in `:root` and used consistently throughout.

#### Scenario: Custom property consistency
- **WHEN** the CSS custom properties are analyzed
- **THEN** all custom properties SHALL be defined in `:root` and all usages SHALL reference existing properties

### Requirement: Responsive breakpoints SHALL cover all new components
All new components (video-grid, agent-grid, cron-section, view-system) SHALL have responsive rules at each breakpoint.

#### Scenario: Responsive coverage
- **WHEN** the responsive breakpoints are analyzed
- **THEN** all new components SHALL have rules at 980px, 720px, and 480px breakpoints

### Requirement: CSS SHALL not have !important declarations unless necessary
The `!important` declaration SHALL only be used when absolutely necessary (e.g., print styles, override requirements).

#### Scenario: !important usage check
- **WHEN** the CSS is analyzed for !important declarations
- **THEN** each !important SHALL have a clear justification (print styles or override)
