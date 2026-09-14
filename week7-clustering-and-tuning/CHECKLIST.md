# Week 7 — Find Moods, Then Tune

**Hand in by end of Week 7:** Parts 6 and 7 done, moods named.

## Group tasks
- [ ] Confirm features were scaled *before* K-Means (check the mean ≈ 0 / std ≈ 1 sanity print)
- [ ] Agree as a group on `k`, using the elbow/silhouette plot as evidence — write down why,
      don't just take the default silently
- [ ] Agree on a playlist-ready name for every single cluster — no "Cluster 0" left in the
      final notebook
- [ ] Review the Grid Search before/after together and agree on how to describe the result
      honestly, especially if the improvement is small
- [ ] Notebook still runs top to bottom with no errors after Parts 6–7
- [ ] Save a checkpoint copy of the notebook into this folder

## Member tasks (each person individually)
- [ ] Can explain why K-Means needs scaled inputs and what "every track in one cluster" means
      as a failure sign
- [ ] Named at least one cluster and can justify the name from its profile table (which
      features are high/low for that cluster)
- [ ] Can explain what Grid Search is actually searching over, in plain language

## Common failure modes to check for
- [ ] Every track landed in one cluster — scaling step was skipped, go back and fix
- [ ] Cluster names are generic ("upbeat", "calm") rather than something distinctive to this genre
- [ ] Tuning result is reported as an improvement when the R² change is negligible
