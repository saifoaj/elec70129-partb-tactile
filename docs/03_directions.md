# Choosing our direction

**We must pick one direction (A to G) and send one paragraph by Sun 29 Nov, 23:59.** The paragraph names the direction, the paper(s), the dataset and the stakeholder ([template](../admin/DIRECTION.md)). It is for feedback only and not marked, but direction G (our own idea) must be approved at this point.

## The directions in plain terms

| | Direction | What it means | Read first | Suggested data | Example stakeholders (handbook) |
|---|---|---|---|---|---|
| **A** | Material, texture or hardness, with explanations | Classify what is being touched, and show *why* the model decided (for example which image regions mattered) | TactEx; ViTacTip | Touch and Go; ObjectFolder Real; TacVerse grating data | Quality inspection, prosthetic-hand users, fruit picking |
| **B** | Graph learning on tactile markers | Treat the marker dots on the gel as nodes of a graph and use a graph neural network | Tac-VGNN | Marker-based images (TacVerse, TacTip-family sensors) | Robotics researchers, surface inspection |
| **C** | Cross-sensor and self-supervised learning | Make a model trained on one sensor work on another, with few labels, or pre-train without labels | TacVerse; SARL; Sparsh | TacVerse (sensors other than GelSight); Touch-Slide | Warehouses with mixed grippers, sensor makers |
| **D** | Visuo-tactile fusion or cross-modal translation | Combine camera and touch, or translate one into the other (for example with a GAN) | Multi-modality sensor (GANs); SARL | Touch and Go; ObjectFolder Real | Robots working in poor lighting |
| **E** | Generative tactile data | Use diffusion or GANs to create extra training images when real data is scarce | MultiDiffSense | A small real dataset plus generated images | Start-ups with little labelled data |
| **F** | Slip and grasp-outcome detection | From touch over several frames, predict whether a grasp will hold or an object will slip | The Feeling of Success; ViTacTip | Feeling of Success; YCB-Slide | Warehouse operators, assistive robotics |
| **G** | Our own idea | Any advanced setting, built on any reading-list paper | Any reading-list paper | Agreed with the module team | Our choice, for example medical robotics |

## Initial assessment (for discussion, not a decision)

The constraint that matters most: **Part A is due Sun 13 Dec**, so most of us have about one focused week for Part B (14 to 20 Dec), plus some time before 7 Dec.

| | Build difficulty in our time | Taught in lectures? | Data notes | Starting points for novelty (ideas only) |
|---|---|---|---|---|
| **A** | Low to medium: essentially a CNN classifier, the same skill as Part A | Yes: CNNs (17 Nov) and ResNet (24 Nov) | Touch and Go: about 13.9k touches, 20 material categories, CC BY 4.0 | Explanations a human inspector can check; recognising materials never seen in training; ranking hardness rather than classifying it |
| **B** | High: needs marker detection plus a new library (PyTorch Geometric) | GNNs only as advanced or guest material | Marker-based TacVerse sensors | Graph versus CNN when markers are missing or the layout changes |
| **C** | Medium to high; simplest form is train on sensor X, fine-tune on sensor Y | Transfer learning, partly; self-supervised, no | TacVerse is the TA's own dataset (useful at the progress check) | How many labels does a new sensor need to match within-sensor accuracy? (a label-efficiency curve) |
| **D** | Medium for fusion; high for GAN translation | Fusion, partly; GANs late or not at all | Touch and Go has paired video and touch | Fusion that still works when the camera is dark or blocked |
| **E** | High: compute-heavy, hard to evaluate | Late or not at all | Ask the TA how this fits the rule against AI-generated data | Does generated data help most when real data is tiny? (accuracy versus number of real images, with and without generated ones) |
| **F** | Medium: CNN on several frames (stacked or differenced) | CNNs, yes; sequence models from 1 Dec | Feeling of Success: 9,269 grasps on 106 objects, but about **110 GB** in total (CC BY-NC-ND 4.0), so a subset is essential; YCB-Slide is an alternative | Predict failure early enough for the robot to regrasp; touch-only versus vision-only versus both |
| **G** | Depends | Depends | Must be agreed by 29 Nov | Depends |

## The four-question test

Score each shortlisted direction 1 (weak) to 3 (strong). Fill this in during the meeting.

| Direction | 1. A real, named stakeholder with a clear "why touch" | 2. Data we can download and subset this week | 3. A proof of concept we can build with a CNN-level model in about a week | 4. A novelty angle beyond the paper and the obvious approach | Team interest | Total |
|---|---|---|---|---|---|---|
| | | | | | | |
| | | | | | | |
| | | | | | | |

## After we choose

1. Data lead: confirm the download size, licence and a subset plan within 48 hours (issue).
2. Research lead: read the main paper properly and write 5 lines on what it does and what we add (issue).
3. Coordinator: fill in [the direction paragraph](../admin/DIRECTION.md) and [the charter](../admin/CHARTER.md), collect signatures, upload by 29 Nov.
4. Everyone: update the status table in the [README](../README.md).
