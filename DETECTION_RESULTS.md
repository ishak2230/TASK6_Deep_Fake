# Detection and Provenance Results

## Hive AI-Generated Audio Detection

**Detector:** Hive Models — AI Generated Audio  
**Artifact Tested:** `approach_1_attempt_2_AI_GENERATED.mp3`  
**Test Clip Length:** 20 seconds  
**Original Artifact Length:** Approximately 1 minute 18 seconds

### Method

I tested the improved synthetic audio from Approach 1 using Hive's AI-generated audio detector. The original ElevenLabs recording was approximately 1 minute and 18 seconds long, but the detector required an audio file of 30 seconds or less.

To meet this limitation, I created a 20-second excerpt from the original recording. The audio was only trimmed for length and was not otherwise modified or enhanced.

### Result

Hive reported that the input was **likely to contain AI-generated content**.

**AI-Generated Speech Confidence: 99.1%**

The detector therefore correctly identified the ElevenLabs-generated speech as synthetic with very high confidence.

### Evaluation

This result was interesting because the second ElevenLabs attempt sounded highly natural during my own listening evaluation. After adjusting the speed, stability, and style settings, I did not notice the same robotic quality that was present in the first attempt.

Despite this improvement in perceived naturalness, Hive still identified the audio as AI-generated with 99.1% confidence.

This suggests that synthetic speech can sound convincing to a human listener while still containing characteristics that an automated detection system recognizes as AI-generated. It also demonstrates that perceived realism alone is not a reliable method for determining whether audio is authentic.

### Detector Limitation

The detector could not process the complete 1-minute-and-18-second artifact through the interface I used because audio uploads were limited to 30 seconds or less. Therefore, the 99.1% result applies specifically to the tested 20-second excerpt and should not automatically be interpreted as a confidence score for every part of the full recording.
