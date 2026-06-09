## ADDED Requirements

### Requirement: Fonts SHALL load efficiently
Google Fonts SHALL use `display=swap` and preload hints for optimal loading.

#### Scenario: Font loading
- **WHEN** the page loads
- **THEN** fonts SHALL use `display=swap` and preload hints SHALL be present

### Requirement: iframes SHALL use lazy loading
All YouTube iframes SHALL use `loading="lazy"` attribute.

#### Scenario: Iframe lazy loading
- **WHEN** the YouTube iframes are analyzed
- **THEN** each iframe SHALL have `loading="lazy"` attribute

### Requirement: CSS SHALL not have redundant rules
CSS rules SHALL not duplicate functionality that could be achieved with fewer rules.

#### Scenario: CSS efficiency
- **WHEN** the CSS is analyzed for redundancy
- **THEN** no redundant rules SHALL be found

### Requirement: Animations SHALL respect reduced motion preferences
Animations SHALL be disabled when `prefers-reduced-motion: reduce` is set.

#### Scenario: Reduced motion support
- **WHEN** the user has reduced motion preference enabled
- **THEN** all animations SHALL be disabled or minimized

### Requirement: Images and backgrounds SHALL be optimized
Background images (SVG grain texture) SHALL be optimized for size.

#### Scenario: Background optimization
- **WHEN** the SVG grain texture is analyzed
- **THEN** it SHALL be optimized for minimal file size
