# Week 3 — Clean the Data

**Hand in by end of Week 3:** Part 2 done in the notebook, cleaning log filled in.

## Group tasks
- [ ] Agree as a group on how duplicates are being defined (exact row vs same track+artist
      re-release) before anyone writes the reason in the log
- [ ] Agree on the policy for missing values (drop vs impute) and make sure it's applied
      consistently, not per-person
- [ ] Review the final cleaned row count together — does the drop in rows make sense, or did
      cleaning remove an unreasonable chunk of the genre?
- [ ] Notebook still runs top to bottom with no errors after Part 2
- [ ] Save a checkpoint copy of the notebook into this folder

## Member tasks (each person individually)
- [ ] Independently verified at least one of the counts in the cleaning log against the
      notebook's actual output (not just copied a teammate's numbers)
- [ ] Filled in at least one row of the cleaning log table with a real reason, in your own words
- [ ] Can explain why we drop `tempo == 0` / `duration_ms == 0` rather than treating them as
      real quiet/short tracks

## Common failure modes to check for
- [ ] Cleaning log has numbers but no reasons (reasons are what's graded, not just the counts)
- [ ] Rows were dropped for a reason that isn't actually written down anywhere
- [ ] `Input contains NaN` still appears in a later section — cleaning is incomplete, come back here
