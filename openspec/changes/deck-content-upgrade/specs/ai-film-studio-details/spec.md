## MODIFIED Requirements

### Requirement: AI Film Studio slide shows production pipeline
Slide 06 (AI Film Studio) SHALL display the gated production pipeline with G0-G7 stages.

#### Scenario: Gate pipeline is displayed
- **WHEN** user navigates to slide 06
- **THEN** 4 gate cards are visible showing G0-G2, G3-G4, G5-G6, G7

#### Scenario: 5-View System is displayed
- **WHEN** user views slide 06
- **THEN** a section shows the 5 views: Dashboard, Canvas, Documents, Library, Review

#### Scenario: Supabase integration is mentioned
- **WHEN** user views slide 06
- **THEN** Supabase is listed as the data persistence layer

## ADDED Requirements

### Requirement: AI Film Studio shows gate validation logic
- **WHEN** user views the AI Film Studio slide
- **THEN** a description mentions that each gate has validation, exploration ≠ master, and no generation without approval
