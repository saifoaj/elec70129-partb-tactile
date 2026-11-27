# Risk register

Reviewed at each weekly meeting. Likelihood and impact: low, medium or high.

| Risk | Likelihood | Impact | Mitigation | Owner |
|---|---|---|---|---|
| Dataset too large or slow to download (Feeling of Success is about 110 GB in total) | Medium | High | Pick a documented subset in the first 48 hours; test one file end to end before downloading more | Data lead |
| Part A week (7 to 13 Dec) stalls Part B | High | High | Baseline running by Sun 6 Dec; only storyboard and scripts that week | Coordinator |
| Data leakage: frames of one object or trial in both train and test | Medium | High | Split by object/trial/session with a grouping column; the notebook asserts no overlap | Data lead |
| Choosing settings on the test set by accident | Low | High | Validation set for every choice; test evaluated once, at the end | Modelling lead |
| Colab disconnects and loses a training run | High | Medium | Save checkpoints to Google Drive every epoch; small subsets and image sizes | Modelling lead |
| Licence forbids our use (for example non-commercial or no-derivatives terms) | Low | Medium | Data lead reads the licence before downloading and notes it in the README | Data lead |
| Video runs over 5:00 | Medium | High | Storyboard with timings; target 4:40; full run-through by Sat 19 Dec | Video producer |
| A member becomes unavailable | Medium | Medium | Backup for each role; charter process; escalate to the TA by Mon 7 Dec if unresolved | Coordinator |
| Novelty too thin ("a standard CNN on a standard dataset") | Medium | High | Research lead writes the "what we add" argument by the progress check and tests it on the TA | Research lead |
