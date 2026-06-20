# Voiceover And Caption Pipeline

This template explains how to move from script to synced subtitles.

## Inputs

- final script
- voiceover MP3 or WAV
- expected scene plan

## Step 1: Confirm Duration

Use FFprobe:

```powershell
ffprobe -v error -show_entries format=duration -of default=nw=1:nk=1 voiceover.mp3
```

## Step 2: Detect Silence

Use FFmpeg silence detection:

```powershell
ffmpeg -i voiceover.mp3 -af silencedetect=noise=-35dB:d=0.25 -f null -
```

This helps identify where sentences and phrases naturally break.

## Step 3: Transcribe

Use a Whisper-style transcription flow to produce rough text and timings.

Output should ideally include:

- transcript text
- segment start time
- segment end time
- confidence or review notes, if available

## Step 4: Build Subtitle Cues

Convert transcript segments into cue objects:

```js
const captions = [
  { start: 0.15, end: 2.9, text: "Opening subtitle line." },
  { start: 2.9, end: 5.8, text: "Second subtitle line." }
];
```

## Step 5: Manual Alignment

Manually adjust cues where:

- a scene changes
- a key UI highlight appears
- a sentence is too long
- a subtitle overlaps important UI

## Step 6: QA

Watch the rendered video and check:

- subtitle wording
- subtitle timing
- line length
- contrast
- placement
- sync with scene transitions

