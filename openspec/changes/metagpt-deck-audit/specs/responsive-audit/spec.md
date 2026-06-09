## ADDED Requirements

### Requirement: All content SHALL be visible at all breakpoints
No content SHALL be cut off, overflow, or hidden at any of the 4 breakpoints (1440px, 980px, 720px, 480px).

#### Scenario: Content visibility at 980px
- **WHEN** the deck is viewed at 980px width
- **THEN** all content SHALL be fully visible without horizontal scrolling

#### Scenario: Content visibility at 480px
- **WHEN** the deck is viewed at 480px width
- **THEN** all content SHALL be fully visible without horizontal scrolling

### Requirement: Card grids SHALL collapse gracefully
Card grids SHALL collapse from multi-column to single-column at appropriate breakpoints.

#### Scenario: Grid collapse at 980px
- **WHEN** the deck is viewed at 980px width
- **THEN** 3-column and 4-column grids SHALL collapse to 2 columns

#### Scenario: Grid collapse at 720px
- **WHEN** the deck is viewed at 720px width
- **THEN** all grids SHALL collapse to single column

### Requirement: Video embeds SHALL maintain aspect ratio
YouTube iframes SHALL maintain 16:9 aspect ratio at all breakpoints.

#### Scenario: Video aspect ratio
- **WHEN** video embeds are viewed at any breakpoint
- **THEN** they SHALL maintain 16:9 aspect ratio without distortion

### Requirement: Navigation SHALL be accessible on mobile
Navigation buttons and dots SHALL be accessible and usable on mobile devices.

#### Scenario: Mobile navigation
- **WHEN** the deck is viewed at 480px width
- **THEN** navigation buttons SHALL be tappable and dots SHALL be clickable

### Requirement: Text SHALL not overflow containers
Text content SHALL not overflow its container at any breakpoint.

#### Scenario: Text overflow check
- **WHEN** text content is analyzed at each breakpoint
- **THEN** no text SHALL overflow its container
