## MODIFIED Requirements

### Requirement: Navigation supports 13 slides
The navigation system SHALL support 13 slides instead of 11.

#### Scenario: Slide count variable is updated
- **WHEN** the JavaScript initializes
- **THEN** the variable `t` is set to `13`

#### Scenario: Progress indicator shows correct total
- **WHEN** user navigates any slide
- **THEN** the progress indicator displays "XX / 13" format

#### Scenario: Dot pagination creates 13 dots
- **WHEN** the page loads
- **THEN** 13 navigation dots are created in the `.dots` container

#### Scenario: Slide indices are updated
- **WHEN** the HTML is rendered
- **THEN** all slide-index elements display "01 / 13" through "13 / 13"
