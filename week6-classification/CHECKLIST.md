# Week 6 — Spot the Hits (Classification)

**Hand in by end of Week 6:** Part 5 done, confusion matrix explained.

## Group tasks
- [ ] Confirm as a group that `popularity` is **not** in the classification inputs — run the
      `assert` in the notebook and watch it pass (this is a −10 automatic deduction if missed)
- [ ] Agree on the hit threshold definition (currently top 25% within-genre) and whether that's
      the right bar for this genre, or whether it should change
- [ ] Walk through the confusion matrix together — agree on what a false negative and false
      positive actually cost the business, in plain terms
- [ ] Notebook still runs top to bottom with no errors after Part 5
- [ ] Save a checkpoint copy of the notebook into this folder

## Member tasks (each person individually)
- [ ] Can explain, without notes, what accuracy near 1.00 would signal and why (leakage)
- [ ] Can read the confusion matrix and state, in one sentence, what the model gets wrong
- [ ] Understands why precision and recall matter more here than accuracy alone (with an
      imbalanced hit rate, accuracy alone can be misleading)

## Common failure modes to check for
- [ ] Accuracy is suspiciously close to 1.00 — re-check `X_cls` doesn't include `popularity`
- [ ] Confusion matrix is shown but not actually explained in words anywhere
- [ ] Recommendation sentence ignores the false-negative/false-positive trade-off entirely
