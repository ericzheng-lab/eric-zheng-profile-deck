## ADDED Requirements

### Requirement: Slide 03 displays YouTube video embeds
Slide 03 (AI Videos) SHALL replace the 4 placeholder `.vbox` elements with YouTube iframe embeds for 5 demo videos.

#### Scenario: All 5 videos are embedded
- **WHEN** user navigates to slide 03
- **THEN** 5 YouTube iframe embeds are visible, each in a 16:9 aspect ratio container

#### Scenario: YouTube embed URLs are correct
- **WHEN** the iframes load
- **THEN** they reference the following YouTube embed URLs:
  - Portfolio Reel: `https://www.youtube.com/embed/b4I2AGmFgWk`
  - HOME XSMARTHOME (live-action): `https://www.youtube.com/embed/f5BNhoHL2Uk`
  - HOME XSMARTHOME MANGA (anime): `https://www.youtube.com/embed/7AGx2OsC6Yw`
  - AI Film Studio Workflow: `https://www.youtube.com/embed/QpTX-hcNw4A`
  - Prompt Builder Demo: `https://www.youtube.com/embed/3aw-AqPE5M4`

#### Scenario: Videos use lazy loading
- **WHEN** the iframes are rendered
- **THEN** they have `loading="lazy"` attribute to prevent simultaneous loading of all 5 videos

#### Scenario: Video layout adapts to screen size
- **WHEN** viewport is at 980px or narrower
- **THEN** the video grid collapses to 2 columns

#### Scenario: Video layout on mobile
- **WHEN** viewport is at 720px or narrower
- **THEN** the video grid collapses to 1 column
