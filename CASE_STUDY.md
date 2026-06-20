# Case Study: AI-Assisted Product Launch Video For An Email Order Intake Platform

## 1. Business Context

Many business teams still process orders, requests, approvals, or documents through email. The process often requires a person to open the email chain, inspect attachments, identify entities, map those entities to master data, check quantities, and prepare an output file for a downstream system.

This case study uses a generic email order intake platform as the example.

## 2. Problem Statement

The manual process had several communication challenges:

- the workflow was easy to understand operationally, but difficult to explain quickly
- the value of AI needed to be shown in business language, not only technical language
- screenshots alone were not enough to communicate the before-and-after impact
- the product needed a short launch video that could be shared with leaders, users, and transformation stakeholders

## 3. Goal

Create a 90-second motion graphics video that explains:

- the current manual burden
- the AI-assisted three-step workflow
- the role of document extraction and master-data matching
- the final business impact

## 4. Solution Approach

The video was built through a structured production pipeline:

1. Convert business context into a launch-video brief.
2. Create a concise voiceover script.
3. Break the script into timestamped scenes.
4. Design a motion system matching the product UI.
5. Use product screenshots as the credibility layer.
6. Build animations in HyperFrames.
7. Add voiceover and subtitles.
8. Use transcript/timing review to sync captions and screen changes.
9. Render and inspect frames for visual quality.
10. Export final video and shorter snippets.

## 5. Why HyperFrames

HyperFrames was useful because the video could be built like a web page:

- HTML for layout
- CSS for visual style
- GSAP for deterministic animation
- media assets for screenshots and voiceover
- CLI render workflow for repeatable exports

This made it easier to revise scenes based on business feedback.

## 6. AI Contribution

AI was used as a production partner across multiple stages:

- converting raw business context into a structured script
- making the story more concise and executive-friendly
- translating process pain points into visual scenes
- generating timestamped storyboard logic
- editing HyperFrames composition code
- aligning subtitles to audio
- identifying scenes where screenshot focus boxes needed adjustment
- preparing public documentation and reusable prompts

The value came from iterative direction, not a single one-shot prompt.

## 7. Technical Pipeline

```text
Input brief
  -> script draft
  -> storyboard
  -> timestamp plan
  -> HyperFrames HTML composition
  -> voiceover MP3
  -> FFmpeg audio inspection
  -> Whisper-style transcript/timing pass
  -> subtitle cue map
  -> render
  -> frame-level QA
  -> snippets
```

## 8. Output

The final output was a short SaaS/product-style launch video with:

- animated opening
- current-process burden scene
- three-step workflow reveal
- product screenshot scenes
- focus rectangles and UI highlights
- synced subtitles
- KPI close
- short social snippets

## 9. Lessons Learned

- Business clarity matters more than visual complexity.
- The script should lead the visuals, not the other way around.
- Product screenshots make the story credible.
- Timestamp-level feedback is essential for good video sync.
- Subtitles need manual review even after transcript automation.
- Public examples should always use anonymized data.

