# Production Pipeline

This document explains the actual build method in operational terms.

## 1. Create The Brief

Start with the business process, not the tool.

Good inputs:

- who does the work today
- what steps are manual
- what data must be checked
- what errors happen
- what the new product changes
- what outcome leaders care about

## 2. Generate The Script

The first script should be plain language. Avoid trying to make it cinematic too early.

Recommended structure:

```text
Opening line
Current process
Pain points
New workflow
Step 1
Step 2
Step 3
Impact
Closing line
```

## 3. Build Timestamp Plan

Once the script is stable, divide it into scenes. Scene changes should happen when the meaning changes, not randomly.

Example:

- current process starts when manual work is introduced
- product proof starts when the workflow steps are described
- KPI screen starts when the result is described

## 4. Build HyperFrames Composition

The video was built as an HTML composition:

- `index.html` as source of truth
- CSS variables for visual system
- GSAP timeline for animation
- audio element for voiceover
- subtitle array for captions
- screenshot assets for product scenes

## 5. Add Voiceover

Voiceover can come from:

- a human-recorded MP3
- a text-to-speech tool
- an AI voice workflow

The important requirement is consistency with the final script. If one line changes in the script, subtitle timings and scene timings may need to be adjusted.

## 6. Transcription And Timing Review

After voiceover is available:

1. Use FFprobe to confirm audio duration.
2. Use FFmpeg silence detection to identify phrase gaps.
3. Use a Whisper-style transcription flow to produce a rough transcript with timings.
4. Convert transcript phrases into subtitle cues.
5. Manually adjust cue boundaries where the scene changes.

This is more reliable than guessing timings by reading the script.

## 7. Subtitle Method

Subtitles were treated as timed UI elements:

- each subtitle has `start`, `end`, and `text`
- text appears in a dark translucent strip
- long lines are split before they overflow
- subtitle changes are aligned to narration, not only scene cuts

## 8. QA Method

QA was done at frame level:

- extract still frames at important timestamps
- check if focus boxes align to UI
- check if subtitles match the audio moment
- check if confidential labels or logos are visible
- check if final screen is readable

## 9. Final Outputs

Recommended outputs:

- full MP4
- 4-5 short clips
- README with method
- prompt pack
- anonymization guide
- timestamp plan
- case study

