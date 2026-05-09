# Public Research Notes

## High-Value Public Data

Kaggle staff shared top-percentile daily replay datasets for Orbit Wars. These datasets are the most useful public source for understanding strong openings, defense timing, and late-game ship movement patterns.

Near-term work should prioritize:

- parsing the top replay datasets
- summarizing first-80-turn expansion routes
- collecting failure cases involving defense, over-expansion, and sun or out-of-bounds losses
- turning those cases into a repeatable validation set

## Rule And Environment Notes

Recent public discussion indicates that sweep and collision handling changed around early May 2026. Some competitors reported new sun or out-of-bounds losses that did not reproduce in older local environments.

This means route legality should be validated against fresh public replays before tuning around edge paths.

## Public Code Review

The most useful public-code ideas seen in the latest review were:

- two-strategy combine entries can transfer well, but are volatile across reruns
- better target inference from fleet origin metadata
- simpler production-aware expansion scoring
- threat maps that avoid over-defending safe planets
- mission-style rescue and recapture logic

Directly copying public entries is not enough by itself. The next useful step is subsystem-level ablation: isolate one idea, test it against replay-derived cases, then submit only if the change improves those cases without hurting common openings.

## Next Priority

Build a small replay-mining dataset and use it to answer three questions:

- Which openings consistently survive strong four-player maps?
- Which defensive mistakes cause the largest public losses?
- Which pathing choices create sun or boundary losses after the recent collision changes?
