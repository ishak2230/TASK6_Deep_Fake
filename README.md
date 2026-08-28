# Task 6 — Constructing and Evaluating Synthetic Media

> **SYNTHETIC MEDIA DISCLOSURE:**  
> The audio and video artifacts in this repository are AI-generated and were created for an academic research experiment on synthetic media. They should not be interpreted as authentic recordings of real events or people.

## Project Overview

This project explores the creation and evaluation of synthetic media by transforming a written sports-data narrative into AI-generated audio and video.

The source material was adapted from my Task 5 analysis of the 2025 Syracuse Women's Lacrosse season. The script summarizes verified team statistics and provides a data-based coaching recommendation.

The experiment used two synthetic-media approaches:

1. AI-generated speech using ElevenLabs.
2. A synthetic talking-avatar video using D-ID and the improved ElevenLabs audio.

The goal was not only to create convincing synthetic media, but also to identify failure modes, compare different generation approaches, and evaluate whether an automated detection system could recognize the resulting media as AI-generated.

## Source Material

The source narrative is available in:

`SOURCE_SCRIPT.md`

The script was adapted from the final coaching advisory analysis produced during Task 5 using the 2025 Syracuse Women's Lacrosse game and player datasets.

## Approach 1 — Synthetic Speech

The first approach used ElevenLabs Text to Speech.

### Attempt 1

The initial generation used the Roger voice with settings kept close to their initial/default configuration.

The result was understandable and fairly natural, but several synthetic characteristics were noticeable:

- An unnatural pause occurred after "Syracuse" in the opening sentence.
- The voice sounded somewhat robotic.
- Emotional expression was limited.
- Most other pauses and pacing were natural.

### Attempt 2

For the second attempt, I adjusted the voice settings by increasing the speaking speed slightly, reducing stability, and increasing style exaggeration.

These changes produced a noticeable improvement. The pacing and pauses sounded more natural, the voice had more energy, and the robotic quality from the first attempt was no longer noticeable to me.

This demonstrated that generation settings can significantly affect the perceived realism of synthetic speech even when the script, model, and selected voice remain the same.

## Approach 2 — Synthetic Avatar Video

The second approach used D-ID to add a synthetic visual component to the improved ElevenLabs audio.

I used the stock Arthur V4 avatar with the Professional style and a lacrosse-related background. The improved audio from Approach 1 was uploaded as the speech source.

The lip-sync was highly convincing and closely matched the spoken audio.

However, adding the visual component introduced new synthetic characteristics. The avatar displayed minimal facial expression, no noticeable hand gestures, and limited body movement.

The video therefore demonstrated that adding another synthetic modality does not necessarily make an artifact more realistic. The highly natural audio made the limited visual behavior of the avatar more noticeable.

## Detection Test

I tested a 20-second excerpt of the improved ElevenLabs audio using Hive's AI-generated audio detector.

Hive classified the sample as likely to contain AI-generated content with:

**99.1% confidence for AI-Generated Speech**

The original recording was approximately 1 minute and 18 seconds long, but the detector interface accepted audio clips of no more than 30 seconds. Therefore, I created a 20-second excerpt without otherwise modifying the audio.

The result was particularly interesting because the improved audio sounded highly natural during my own listening evaluation. Despite this perceived realism, the detector identified the sample as synthetic with very high confidence.

Full details are available in `DETECTION_RESULTS.md`.


## Key Learnings

This experiment demonstrated that synthetic-media quality is strongly affected by generation settings and by the number of modalities involved.

The first ElevenLabs generation was understandable but contained noticeable synthetic cues, particularly a robotic tone, limited emotion, and an unnatural pause. Adjusting the generation settings substantially improved the perceived naturalness of the voice.

The D-ID experiment showed a different type of limitation. Although the lip-sync was convincing, the lack of expressive facial behavior, hand gestures, and body movement made the avatar appear less natural.

One of the most important findings was that human perception and automated detection did not necessarily produce the same assessment. The improved ElevenLabs recording sounded convincing to me, yet Hive identified a 20-second sample as AI-generated speech with 99.1% confidence.

Overall, the project showed that synthetic media can become highly convincing in individual dimensions such as voice quality or lip synchronization while still containing detectable artifacts in other dimensions. It also demonstrated the importance of transparent labeling, provenance checks, and critical evaluation when working with synthetic media.

## Ethics and Disclosure

This project was conducted for research and educational purposes.

No attempt was made to impersonate a real named person. The video used a stock avatar supplied by the synthetic-media platform, and all generated artifacts are explicitly identified as AI-generated.

The synthetic-media artifacts should not be presented or distributed as authentic recordings.
