# cershe-valence-arousal-data-analysis

# Cershe: Emotional-State Training Stories

This notebook reads the training stories for Cershe's emotional-state module and plots how her **valence** and **arousal** change, step by step, as events happen and time passes.

It is part of [Milestone 1: A Coherent Emotional State](https://cershe.ai/log/milestone-1-coherent-emotional-state) on the [Cershe Log](https://cershe.ai/log). The idea of elapsed time behind these stories is described in [Log 003: Time Heals](https://cershe.ai/log/time-heals).

## What is in the data

Each story (a **sequence**) follows Cershe through a series of **steps**. Every step records:

| Field | Meaning |
| --- | --- |
| Elapsed minutes | Time since the previous step |
| Event type | `news`, `conversation`, `memory_recall`, `reminder` or `time_only` |
| Event | What happened |
| Core value related | 1 if the event touches one of her core values, 0 if not |
| Core value | Which values it touches (optional) |
| Unresolved / Resolves | Whether the event opens or closes an ongoing concern (optional) |
| Target valence | How pleasant or unpleasant she feels, from −1.00 to 1.00 |
| Target arousal | How calm or activated she is, from 0.00 to 1.00 |
| Annotation note | Why the values were chosen |

Her resting state, when nothing is affecting her, is valence 0.10 and arousal 0.20.

**Cershe's core values:** against animal cruelty · kindness · preserving the earth · against global warming · against money hoarding · against misogyny · free to live · against patriarchy.

## How to use this notebook

1. Upload `stories-draft-001.txt` when the notebook asks for it.
2. Run the cells in order, from top to bottom.
3. To look at a different story, change the story number in the cell that picks it (`blocks[0]` is the first story) and run the cells below it again.

## What the graphs show

- **Valence and arousal at each step.** A sudden jump marks the moment an event changes how she feels. The slow slopes in between show the feeling fading with time.
- **Event type under each step**, so you can see which events cause the spikes.
- **Core-value steps marked**, to show whether events that touch her values move her more.

## Notes

- Valence and arousal were labelled by Anyta Ali. They are one person's judgement, intended as training targets, not measurements.
- The events are invented, fictitious scenarios. Any resemblance to actual events is coincidental.
- All rights reserved.

Questions, or interested in being a tester? Write to anyta.ali@cershe.ai.
