## MODIFIED Requirements

### Requirement: Tool Stack slide shows technology inventory
Slide 09 (Tool Stack) SHALL display the full technology stack used across all products.

#### Scenario: Tool categories are displayed
- **WHEN** user navigates to slide 09
- **THEN** tools are organized by category: AI Orchestration, Video Generation, Image Generation, Audio, Production Frameworks

#### Scenario: Full tool list is shown
- **WHEN** user views the Tool Stack slide
- **THEN** the following tools are listed: Claude Code (daily 4-8h), OpenClaw, ChatGPT, GPT-Image-2, Flux 2 Max, Midjourney, Nano Banana, Runway, Seedance, Higgsfield, Hyperframes, ElevenLabs, Suno, MiMo TTS

#### Scenario: Usage frequency is indicated
- **WHEN** a tool card is rendered
- **THEN** it shows the tool name and a brief usage context (e.g., "Claude Code — daily execution, 4-8h")
