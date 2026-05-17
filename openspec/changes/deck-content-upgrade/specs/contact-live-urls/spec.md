## ADDED Requirements

### Requirement: Contact slide shows 4 live product URLs
The Contact slide (slide 13) SHALL display 4 live product URLs in addition to existing contact info.

#### Scenario: Live URLs are visible
- **WHEN** user navigates to the Contact slide
- **THEN** the following URLs are listed:
  - ai.drsfilms.com
  - video-canvas.pages.dev
  - videoagent-studio.vercel.app
  - ericzheng-lab.github.io/prompt-builder

#### Scenario: URLs use existing contact-list styling
- **WHEN** the URLs are rendered
- **THEN** they follow the existing `.contact-list` grid layout with label + value pairs
