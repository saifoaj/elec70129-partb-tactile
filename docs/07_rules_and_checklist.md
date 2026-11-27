# Rules that protect our marks, and the final checklist

## Integrity

- [ ] **Part A is individual.** Nobody shares Part A code, weights, results or report text with the group, and none of it enters this repo.
- [ ] **Part B is shared work.** Every member is responsible for the whole submission.
- [ ] **Cite everything we did not create:** papers, datasets, pretrained weights, adapted code, figures, music.
- [ ] **Never fabricate or adjust results.** Never select models or settings on the test set.

## Data

- [ ] No Part A dataset, and no GelSight subsets of TacVerse.
- [ ] Own data only if agreed with the module team by 29 Nov; anything involving people needs ethical approval first.
- [ ] Split by object, session, trial or sensor, never by single frame; normalise with training statistics only.
- [ ] Raw data never goes into the repo or the submission. Licences checked and cited.

## AI use

- [ ] Allowed and declared: brainstorming, explanations, debugging, code we understand and test, grammar of our own text, video editing.
- [ ] Never: AI voices or avatars presenting; generating or changing data, results or references.
- [ ] Four-line declaration in the contributions form: tools; what for; which parts; how we checked. Required even if we used none.

## Final checklist (Sun 20 Dec)

**Proof of concept**
- [ ] Advanced task on one documented dataset (not the Part A data)
- [ ] Leakage-free split documented
- [ ] Model we trained ourselves, compared with a reference point
- [ ] Test results: accuracy, macro F1, confusion matrix (or RMSE, MAE, predicted versus true)
- [ ] At least one failure case shown and explained
- [ ] Demo clip of the model on test data

**Video**
- [ ] At most 5:00 including the opening and closing cards (target 4:30 to 4:50)
- [ ] Every member presents in their own voice, 45 to 70 seconds each, named on screen
- [ ] Reading-list paper(s) named and cited on screen
- [ ] Results and demo shown
- [ ] Captions burned in or a corrected `.srt`
- [ ] MP4 (H.264, AAC), 1920x1080 preferred, under 1 GB
- [ ] Watched together before upload: timing, sound, captions, spelling

**Files**
- [ ] `GroupXX_TactileDL_Video.mp4` (+ `.srt`)
- [ ] `GroupXX_TactileDL_Code.zip`: notebook, README, weights, `TRAIN = False` loads them, no raw data
- [ ] `GroupXX_TactileDL_Contributions.pdf`: who did what, shares adding to 100%, AI-use declaration
- [ ] Coordinator uploaded; Canvas confirmation saved
- [ ] Email to the TA, copying every member: group number, title, direction, paper(s), members, Colab link

**After**
- [ ] All six peer assessments submitted by Wed 23 Dec, 23:59
