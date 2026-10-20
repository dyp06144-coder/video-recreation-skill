
# Video Recreation Skill

A modular AI skill for analyzing, recreating, editing, and creatively transforming reference videos.

The skill focuses on understanding what makes a reference video work, identifying which relationships should be preserved, and rebuilding those relationships for new characters, products, environments, actions, voices, or creative goals.

## Features

- Reference video analysis
- Faithful recreation
- Partial replacement and editing
- Creative transformation
- Character and object replacement
- Product replacement
- Scene transformation
- Action and timing adaptation
- Script and event timing
- Video generation prompt direction
- Voice identity and accent replacement
- Preservation of key visual, narrative, motion, and audio relationships

## Structure

```text
video-recreation-skill/
│
├── SKILL.md
└── references/
    ├── 01-reference-analysis.md
    ├── 02-brief-treatment.md
    ├── 03-reference-transformation.md
    ├── 04-script-timing.md
    ├── 05-video-prompt-direction.md
    └── 06-voice-replacement.md
```

## Main Skill

`SKILL.md`

The main skill acts as the entry point. It determines the user's goal, identifies what should be preserved or replaced, and routes the task to the relevant reference modules.

## Reference Modules

### 01 — Reference Analysis

Analyzes the content, structure, audiovisual language, timing, and attention mechanisms of the reference video.

### 02 — Brief & Treatment

Defines the user's target, preservation requirements, replacement scope, and creative direction for the new version.

### 03 — Reference Transformation

Transforms characters, products, environments, actions, content, or style while preserving the important relationships from the reference.

### 04 — Script & Timing

Handles dialogue, narration, action, music, visual events, timing relationships, and duration adaptation.

### 05 — Video Prompt Direction

Converts the analysis and creative plan into generation-ready or editing-ready video prompts.

### 06 — Voice Replacement

A conditional module activated when the user explicitly requests a new voice identity, timbre, gender presentation, accent, or voice reference.

It enforces consistent target voice identity across all speaking scenes and prevents fallback to the original speaker voice.

## Typical Workflow

```text
User Request
      ↓
SKILL.md
      ↓
Reference Analysis
      ↓
Brief & Treatment
      ↓
Reference Transformation
      ↓
Script / Timing
      ↓
Video Prompt Direction
      ↓
Optional Voice Replacement
```

Not every task requires every module. The main skill selects and reuses only the modules necessary for the current request.

## Example Use Cases

- Recreate a commercial using a different product
- Replace the main character while preserving camera language
- Recreate a viral short-form video's attention mechanism
- Replace the environment while preserving action and pacing
- Adapt a reference video into a new creative concept
- Replace a male speaker with a consistent female voice
- Preserve choreography or motion timing while changing characters
- Generate an executable prompt from a reference video

## License

Specify the license for this repository here.
