# Week 5 — Predict Popularity (Regression)

**Hand in by end of Week 5:** Part 4 done, two models compared.

## Group tasks
- [ ] Confirm as a group that both models are scored on the **test** set, not training data
      (this is a −7 automatic deduction if missed — check it twice)
- [ ] Agree on the one-sentence recommendation ("This means the streaming service should…")
      together, so it reflects the actual R²/RMSE, not a generic line
- [ ] Sanity-check: if R² > 0.9, stop and find the leak before moving on
- [ ] Notebook still runs top to bottom with no errors after Part 4
- [ ] Save a checkpoint copy of the notebook into this folder

## Member tasks (each person individually)
- [ ] Can explain what RMSE means in real units (popularity points) without looking it up
- [ ] Can explain why R² between 0.05–0.20 here is a normal, honest result and not a failure
- [ ] Looked at the Linear Regression coefficients and can name the strongest one and its
      real-world direction (e.g. "higher X is associated with slightly lower popularity")
- [ ] Can explain the difference between what Linear Regression and Random Forest are doing,
      in plain language

## Common failure modes to check for
- [ ] R² looks suspiciously high — check the train/test split wasn't accidentally skipped
- [ ] The recommendation sentence doesn't actually follow from the R² value reported above it
