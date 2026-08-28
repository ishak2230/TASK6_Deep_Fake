# Process Log

## Approach 1 — Text-to-Speech Audio

### Attempt 1

**Tool:** ElevenLabs Text to Speech  
**Model:** Eleven Multilingual v2  
**Voice:** Roger — Laid-Back, Casual, Resonant  
**Output Format:** MP3 44.1 kHz (128 kbps)  
**Speaker Boost:** Enabled  
**Language Override:** Off  
**Artifact:** `approach_1_attempt_1_AI_GENERATED.mp3`

### Process

For the first attempt, I used ElevenLabs Text to Speech to convert the Task 5 coaching advisory script into synthetic audio. I used the Roger voice and kept the available voice settings close to their default values rather than making significant adjustments. This provided a baseline output that I could evaluate before attempting to improve the synthetic voice.

### Evaluation

The generated audio sounded fairly natural overall, and most of the pauses between sentences and sections were appropriate. However, there was a noticeable unnatural pause after the word "Syracuse" in the first sentence. This made the opening sentence sound less natural than the rest of the recording.

The voice also had a somewhat robotic quality. Although the words were clear and understandable, the delivery did not contain much emotion. It sounded more like a synthetic voice reading a prepared script than a person naturally presenting a sports analysis.

### Observed Failure Modes

- Unnatural pause after "Syracuse" in the opening sentence
- Slightly robotic vocal quality
- Limited emotional expression
- Most other pauses and pacing sounded natural

### Overall Assessment

The first attempt was convincing enough to be easily understood and sounded fairly natural in several places. However, the robotic tone and limited emotional expression were noticeable indicators that the audio was synthetic. The unnatural pause in the opening sentence was another specific artifact that reduced the realism of the recording.


### Attempt 2 — Adjusted Voice Settings

**Tool:** ElevenLabs Text to Speech  
**Model:** Eleven Multilingual v2  
**Voice:** Roger — Laid-Back, Casual, Resonant  
**Output Format:** MP3 44.1 kHz (128 kbps)  
**Language Override:** Off  
**Artifact:** `approach_1_attempt_2_AI_GENERATED.mp3`

### Changes from Attempt 1

After listening to the first attempt, I adjusted several voice settings to address the robotic tone and limited emotional expression.

The main changes were:

- Increased the speaking speed slightly
- Reduced stability to allow more vocal variation
- Increased style exaggeration to add more expression and energy
- Kept the same voice, model, and source material so that the results could be compared with the first attempt

### Evaluation

The second attempt was noticeably better than the first. The speaking pace sounded more natural, and the pauses fit the sentences better. The unnatural pause that was noticeable in the first attempt was no longer a significant problem.

The voice also had more energy and expression. In the first attempt, the delivery sounded somewhat robotic and emotionally flat. After changing the settings, the second version sounded much more like a person naturally presenting the analysis.

I did not notice the same robotic quality that was present in the first attempt. The combination of the faster pace, lower stability, and increased style exaggeration produced a more convincing result.

### Comparison with Attempt 1

| Feature | Attempt 1 | Attempt 2 |
|---|---|---|
| Pacing | Natural overall, but slightly flat | More natural |
| Pauses | Mostly good, with one noticeable unnatural pause | More natural and consistent |
| Emotional expression | Limited | Noticeably improved |
| Energy | Low | More energetic |
| Robotic quality | Noticeable | Not noticeably robotic |
| Overall naturalness | Fairly convincing | Highly convincing |

### Overall Assessment

Attempt 2 was a clear improvement over Attempt 1. Small changes to the generation settings had a noticeable effect on how natural the synthetic voice sounded. In particular, adjusting speed, stability, and style exaggeration improved the pacing and emotional delivery without changing the underlying script.

This experiment showed that the quality of synthetic speech depends not only on the text and selected voice but also on how the generation settings are configured.

## Approach 2 — Synthetic Avatar Video

### Attempt 1

**Tool:** D-ID  
**Avatar:** Arthur (V4)  
**Avatar Style:** Professional  
**Aspect Ratio:** 16:9  
**Audio Source:** Improved ElevenLabs audio from Approach 1  
**Audio Duration:** Approximately 1 minute 18 seconds  
**Artifact:** `approach_2_attempt_2_AI_GENERATED.mp4`

### Process

For the second approach, I used D-ID to turn the improved synthetic audio from ElevenLabs into a talking-avatar video. I selected the stock Arthur V4 avatar with the Professional style and used a lacrosse-related background.

Instead of generating another voice, I uploaded the improved ElevenLabs audio from Approach 1. This allowed me to keep the audio constant and focus on evaluating what changed when a synthetic visual component was added.

### Evaluation

The lip-sync was very convincing. The avatar's mouth movements matched the spoken audio closely, and I did not notice significant synchronization problems.

However, the avatar had very little physical movement. There were no noticeable hand gestures, even though a real person giving this type of analysis might naturally use their hands while speaking.

The facial expressions were also minimal. Although the mouth movement followed the speech accurately, the rest of the face did not show much emotion or variation. This made the presentation feel less natural than the audio alone.

### Observed Failure Modes

- Minimal facial expression
- No visible hand gestures
- Limited body movement
- Strong lip-sync despite limited nonverbal communication

### Overall Assessment

The lip-sync was one of the strongest aspects of the generated video and looked convincing. However, the lack of hand gestures, body movement, and expressive facial behavior made the avatar feel less like a real person giving a presentation.

Interestingly, the ElevenLabs audio by itself sounded highly natural after the settings were adjusted, but adding a visual avatar introduced new indicators of synthetic media. This suggests that adding more modalities does not necessarily make synthetic content more convincing. A realistic voice can actually highlight weaknesses in an avatar when the visual behavior does not match the naturalness and energy of the speech.
