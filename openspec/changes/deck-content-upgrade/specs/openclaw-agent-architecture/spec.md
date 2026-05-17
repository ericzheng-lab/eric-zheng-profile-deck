## ADDED Requirements

### Requirement: OpenClaw slide displays 8 agent roles
Slide 04 (OpenClaw) SHALL display 8 specific agent roles in a grid layout, replacing the current 3 generic cards.

#### Scenario: All 8 agents are displayed
- **WHEN** user navigates to slide 04
- **THEN** 8 agent cards are visible: General, Engineer, Creator, Advisor, Wiseman, Debugger, Video-Creator, Marketer

#### Scenario: Each agent card shows role name and description
- **WHEN** an agent card is rendered
- **THEN** it displays the agent name (e.g., "GENERAL") and a one-line role description

### Requirement: OpenClaw slide shows cron schedule
The OpenClaw slide SHALL display the automated schedule details.

#### Scenario: Cron schedule is visible
- **WHEN** user views slide 04
- **THEN** a schedule section shows: Daily Brief 08:30, Inbox Triage 09:00/14:00/21:00, Weekly Retrospective Fridays

### Requirement: Agent grid is responsive
- **WHEN** viewport is 980px or narrower
- **THEN** the 8-agent grid collapses to 2 columns (4 rows)

#### Scenario: Mobile agent layout
- **WHEN** viewport is 720px or narrower
- **THEN** the 8-agent grid collapses to 1 column
