## ADDED Requirements

### Requirement: Interactive elements SHALL have ARIA labels
All interactive elements (buttons, links, iframes) SHALL have appropriate ARIA labels.

#### Scenario: Button ARIA labels
- **WHEN** the navigation buttons are analyzed
- **THEN** each button SHALL have an `aria-label` attribute describing its function

### Requirement: iframes SHALL have accessible names
All YouTube iframes SHALL have `title` attributes describing their content.

#### Scenario: Iframe titles
- **WHEN** the YouTube iframes are analyzed
- **THEN** each iframe SHALL have a `title` attribute with descriptive text

### Requirement: Color contrast SHALL meet WCAG AA
Text and interactive elements SHALL have sufficient color contrast (4.5:1 for normal text, 3:1 for large text).

#### Scenario: Color contrast check
- **WHEN** color contrast is analyzed
- **THEN** all text elements SHALL meet WCAG AA contrast requirements

### Requirement: Focus states SHALL be visible
All interactive elements SHALL have visible focus states for keyboard navigation.

#### Scenario: Focus visibility
- **WHEN** user tabs through interactive elements
- **THEN** each element SHALL have a visible focus indicator

### Requirement: Touch targets SHALL be minimum 44x44px
All interactive elements SHALL have minimum touch target size of 44x44px on mobile.

#### Scenario: Touch target size
- **WHEN** interactive elements are analyzed on mobile viewport
- **THEN** each element SHALL have minimum 44x44px touch target
