## ADDED Requirements

### Requirement: All URLs SHALL be valid and accessible
All URLs in the deck SHALL be valid and point to accessible resources.

#### Scenario: URL validation
- **WHEN** all URLs in the deck are checked
- **THEN** each URL SHALL return a 200 status code or be a valid embed URL

### Requirement: Content SHALL be consistent across slides
Terminology and product names SHALL be consistent across all slides.

#### Scenario: Terminology consistency
- **WHEN** content is analyzed for terminology
- **THEN** product names (OpenClaw, AI Film Studio, etc.) SHALL be spelled consistently

### Requirement: Slide indices SHALL match slide comments
Slide index numbers in the HTML SHALL match the slide comment numbers.

#### Scenario: Index-comment alignment
- **WHEN** slide indices and comments are compared
- **THEN** each slide's index SHALL match its comment number

### Requirement: All product URLs SHALL be correct
Live product URLs mentioned in the deck SHALL point to the correct deployed versions.

#### Scenario: Product URL verification
- **WHEN** product URLs are checked
- **THEN** each URL SHALL point to the correct deployed product

### Requirement: Content SHALL not have placeholder text
The deck SHALL not contain any placeholder text (e.g., "Lorem ipsum", "TODO", "TBD").

#### Scenario: Placeholder text check
- **WHEN** the deck content is analyzed
- **THEN** no placeholder text SHALL be found
