# Part B on one page

**In one sentence:** pick a touch-sensing problem that a real, named organisation has, pitch a deep learning solution in a video of at most 5:00, and prove the core idea with a small model we train ourselves.

Source: the Simplified Handbook (10 Nov 2026) and the Final Project Handbook on Canvas. If anything here disagrees with Canvas, Canvas wins.

## The brief

- Groups of 4 to 6; we are 6. Worth **40 of the final project's 100 marks** (Part A is the other 60), scaled for each of us by a peer factor (see [marking](02_marking.md)).
- The idea must **build on at least one paper from the reading list** ([reading list](06_reading_list.md)) and say what we add.
- It must go **beyond the Part A tasks** in at least one way:
  - a different kind of model: graph, generative or self-supervised
  - a harder setting: a new sensor, few labels, several frames over time
  - another modality: vision together with touch, or translating one into the other
  - a new tactile property: hardness, material or texture

## Proposed solution versus proof of concept

| | What it is | Must it be built? |
|---|---|---|
| **Proposed solution** | The full system we pitch to the stakeholder | No. We describe it, argue it is feasible and name the risks. |
| **Proof of concept** | A small model showing the core idea works | Yes. It must be real, and the code is checked. |

This is the most useful fact about Part B: we can pitch something ambitious as long as a small, honest experiment supports it.

## Proof of concept: the minimum

1. One advanced task on one dataset. A documented subset is fine (for example 5 to 10 classes and a few thousand frames).
2. A leakage-free split, 60/20/20 or 70/15/15, **by object, session, trial or sensor, never by single frame**. Normalise with training-set statistics only.
3. A model we trained ourselves: a small CNN, a graph network, or a fine-tuned network such as ResNet-18.
4. A reference point: a trivial baseline (majority class, or predicting the mean) or a simpler model. For a cross-sensor project, the within-sensor score.
5. Test-set results. Classification: accuracy, macro F1 and a confusion matrix. Regression: RMSE, MAE and a predicted-versus-true plot.
6. At least one failure case we can show and explain.
7. A short demo clip of the model predicting on test examples (a screen recording is fine).

The code is mandatory but not graded: markers use it to check the proof of concept is real. Colab's free GPU is enough if we resize images (128x128 or 224x224) and work on a subset.

## Data

- **Allowed:** public tactile datasets such as TacVerse (not its GelSight subsets), Touch and Go, ObjectFolder Real, The Feeling of Success, YCB-Slide, Touch-Slide. Details in the [reading list](06_reading_list.md).
- **Not allowed:** the Part A dataset, and the GelSight subsets of TacVerse.
- **Our own data:** optional, and must be agreed with the module team **by 29 Nov**. Anything involving people needs College ethical approval first.
- Check each licence, cite the dataset, and never put raw data in the submission.

## The video

- **5:00 hard limit**, including an opening card (group, title, names) and a closing card (who did what, datasets, credits). Markers stop at 5:00. Aim for 4:30 to 4:50.
- Audience: a robotics engineer, a potential user and a funder.
- **Every member presents** in their own voice, about 45 to 70 seconds each, named on screen. No AI voices, avatars or text-to-speech.
- Name and cite on screen the reading-list paper(s) we build on. Show the result analysis and a demo.
- Captions burned in or as a corrected `.srt`. MP4 (H.264, AAC), 1920x1080 preferred, 1280x720 minimum, under 1 GB.

## What we submit (by Sun 20 Dec, 23:59)

The coordinator uploads to the Part B group assignment on Canvas:

| File | Contents |
|---|---|
| `GroupXX_TactileDL_Video.mp4` (+ `.srt`) | The video. If Canvas rejects it, share from College OneDrive and submit the link before the deadline. |
| `GroupXX_TactileDL_Code.zip` | Notebook, README and weights, with a `TRAIN = False` switch that loads the weights. No raw data. |
| `GroupXX_TactileDL_Contributions.pdf` | Who did what, agreed shares of effort (adding to 100%), and the group's AI-use declaration |

Then the coordinator emails the TA, copying every member, with the group number, title, direction, paper(s), members and the Colab link. Only the coordinator uploads; the last upload counts.

## AI use

| Use | Allowed? |
|---|---|
| Brainstorming, explanations, debugging | Yes, declared |
| Generating code we understand and test | Yes, declared |
| Grammar of our own text; video editing | Yes, declared |
| AI voices or avatars presenting for a member | No |
| Generating or changing data, results or references | Never |

The declaration is four lines: tools; what for; which parts; how we checked. It goes in the contributions form even if we used no AI.
