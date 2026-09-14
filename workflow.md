# Workflow

How this repo is organized, how we work week to week, and who does what.

## Repo layout

```
.
├── music_popularity_capstone.ipynb   ← the ONE notebook. Everyone works in this file.
├── README.md                         ← setup instructions (dataset download, GENRE variable)
├── workflow.md                       ← this file
├── week1-2-setup-and-filtering/
├── week3-cleaning/
├── week4-eda/
├── week5-regression/
├── week6-classification/
├── week7-clustering-and-tuning/
└── week8-report-and-presentation/
```

The notebook itself is never split up — it's one file, worked top to bottom, all eight weeks.
The `weekN-*` folders are **checkpoints**: at the end of each week, save a dated copy of the
current notebook into that week's folder (e.g. `week3-cleaning/capstone_week3_checkpoint.ipynb`)
and commit it there, alongside that week's `CHECKLIST.md`. This is what gives us a paper trail —
if two checkpoints get missed in a row, that's how groups fail this project, so the folders exist
to make "did we actually hand something in this week" visible at a glance.

## Roles (assign in Week 1, revisit if it's not working)

| Role | Responsibility |
|---|---|
| Repo owner | Owns the GitHub repo, merges PRs/branches, keeps `main` runnable |
| Data/cleaning lead | Owns Parts 1–2 (load, filter, clean) |
| EDA lead | Owns Part 3 (charts + interpretations) |
| Modeling lead | Owns Parts 4–5 (regression + classification) |
| Clustering/report lead | Owns Parts 6–7 and drafts the report skeleton |

Roles don't mean "only that person touches that section" — they mean that person is
accountable for it being done and defensible by Friday of that week. Everyone should still
be able to explain every cell; the presentation doesn't let you point at a teammate.

## Weekly cycle

1. **Start of week:** open that week's `CHECKLIST.md`, confirm who's doing what.
2. **Mid-week:** commit early, commit often, in small chunks — not one giant commit the
   night before. A member with no commits cannot receive the group mark, and a single
   last-minute commit reads the same as no commits when it comes to reviewing history.
3. **End of week:** run the whole notebook top to bottom from a fresh kernel. If it errors,
   fix it before you commit — that's an automatic −5 at final submission, don't let it
   accumulate silently.
4. **Checkpoint:** copy the notebook into that week's folder, check off `CHECKLIST.md`,
   push, open a PR if you're using branches, and merge.

## Git basics for this project

```bash
git add .
git commit -m "Week 4: EDA charts + interpretations"
git push
```

If working on branches:
```bash
git checkout -b week5-regression
# ... do the work, commit ...
git push -u origin week5-regression
# open a PR into main, get a teammate to glance at it, merge
```

Either is fine — direct commits to `main` are okay for a small group project as long as
each person's commits are visible under their own name. Pick whichever your group finds
less friction and say so at the bottom of this file.

## Non-negotiables (apply every week, not just Week 8)

- No leakage: `popularity` never enters the classification inputs.
- Regression is always scored on the **test** set.
- Every model section ends with: *"This means the streaming service should…"*
- If an AI assistant helped with a cell, note it in the notebook's usage-note cell at the top.
- Honest numbers over impressive ones — a low R², reported and explained, beats a
  suspiciously high one that turns out to be a train/test leak.

---
**Group's chosen git workflow:** _(fill in: direct-to-main / feature branches)_
