# Reading list and datasets

**Every direction must build on at least one of these papers and cite it on screen.** Letters show which directions each paper serves. The list is from the module handbook.

## Part B papers

| Dirs | Paper | Link |
|---|---|---|
| A | F. Verstraete, L. Wei, W. Fan, D. Zhang, "TactEx: an explainable multimodal robotic interaction framework for human-like touch and hardness estimation," IEEE ICRA, 2026 | Search the title (ICRA 2026) |
| A, F | W. Fan et al., "ViTacTip: design and verification of a novel biomimetic physical vision-tactile fusion sensor," 2024 | [arXiv:2402.00199](https://arxiv.org/abs/2402.00199) |
| B | W. Fan, M. Yang, Y. Xing, N. F. Lepora, D. Zhang, "Tac-VGNN: a Voronoi graph neural network for pose-based tactile servoing," 2023 | [arXiv:2303.02708](https://arxiv.org/abs/2303.02708) |
| C | L. Wei et al., "TacVerse: a multisensor dataset and benchmark for cross-sensor vision-based tactile perception," Advanced Robotics Research, 2026 | [doi:10.1002/adrr.70169](https://doi.org/10.1002/adrr.70169) |
| C, D | G. Khurana, L. Wei, D. Zhang, "SARL: spatially-aware self-supervised representation learning for visuo-tactile perception," IEEE ICRA, 2026 | Search the title (ICRA 2026) |
| C | C. Higuera et al., "Sparsh: self-supervised touch representations for vision-based tactile sensing," 2024 | [arXiv:2410.24090](https://arxiv.org/abs/2410.24090) |
| D | D. Zhang et al., "Design and benchmarking of a multi-modality sensor for robotic manipulation with GAN-based cross-modality interpretation," 2025 | [arXiv:2501.02303](https://arxiv.org/abs/2501.02303) |
| E | S. Bhouri, L. Wei, J.-Q. Zheng, D. Zhang, "MultiDiffSense: diffusion-based multi-modal visuo-tactile image generation," IEEE ICRA, 2026 | [arXiv:2602.19348](https://arxiv.org/abs/2602.19348) |
| F | R. Calandra et al., "The feeling of success: does touch sensing help predict grasp outcomes?," 2017 | [arXiv:1710.05512](https://arxiv.org/abs/1710.05512) |
| any | W. Fan, H. Li, D. Zhang, "MagicTac: a novel high-resolution 3D multi-layer grid-based tactile sensor," 2024 | [arXiv:2402.01366](https://arxiv.org/abs/2402.01366) |
| any | W. Fan, H. Li, D. Zhang, "CrystalTac: vision-based tactile sensor family fabricated via rapid monolithic manufacturing," Cyborg and Bionic Systems, 2025 | Search the title |

Background for everyone: W. Yuan, S. Dong, E. H. Adelson, "GelSight: high-resolution robot tactile sensors for estimating geometry and force," Sensors, 17(12), 2762, 2017.

## Datasets we may use

These are large. A documented subset is fine. Check each licence and cite the dataset.

| Dataset | Sensor | What it contains | Licence and size notes | Link |
|---|---|---|---|---|
| TacVerse | Seven vision-based tactile sensors | Shape classification, grating classification and force regression | **Do not use the GelSight subsets** in Part B | [LannWei/Tactile_Database](https://github.com/LannWei/Tactile_Database) |
| Touch and Go | GelSight plus RGB video | Human-collected touches of objects in natural scenes; material labels on touch-onset frames (20 categories) | CC BY 4.0 | [touch-and-go.github.io](https://touch-and-go.github.io) |
| ObjectFolder Real | Gel-based tactile video | 100 household objects; tactile, visual and audio data at 30 to 50 contact points per object | Downloads come in batches of 10 objects | [download page](https://objectfolder.stanford.edu/objectfolder-real-download) |
| The Feeling of Success | GelSight on each gripper finger, plus camera | 9,269 robot grasps on 106 objects, with outcomes; HDF5 files | CC BY-NC-ND 4.0; about **110 GB** in total, so download a subset of files | [project page](https://sites.google.com/view/the-feeling-of-success), [archive (TU Dresden)](https://doi.org/10.25532/OPARA-700) |
| YCB-Slide | DIGIT | Sliding touches over YCB objects, with sensor poses and object meshes | Best for object recognition; localisation is advanced | [rpl-cmu/YCB-Slide](https://github.com/rpl-cmu/YCB-Slide) |
| Touch-Slide | DIGIT | About 180k unlabelled frames from 9 objects | Self-supervised pre-training only; CC BY-NC 4.0 | [Hugging Face](https://huggingface.co/datasets/facebook/touch-slide) |

Pretrained tactile encoders such as Sparsh are allowed as an advanced option, as long as we train and evaluate the model ourselves.

Dataset facts were checked on 27 Nov 2026; the data lead re-checks size and licence before downloading.
