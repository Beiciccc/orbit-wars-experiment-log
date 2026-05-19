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
- using fully visible opponent fleets for defense and target inference is now the clearest discussion-backed direction
- better target inference from fleet origin metadata
- simpler production-aware expansion scoring
- threat maps that avoid over-defending safe planets
- mission-style rescue and recapture logic

Directly copying public entries is not enough by itself. The next useful step is subsystem-level ablation: isolate one idea, test it against replay-derived cases, then submit only if the change improves those cases without hurting common openings.

## 2026-05-17 Public Review

The newest public-code refresh produced no direct-use candidate. One new multi-policy notebook was useful as a simple design reference, but it was not submission-shaped as published and used several physics shortcuts that make direct transfer risky.

Another recently rerun public reference had clean parsing and fleet-intent ideas, but local mixed-anchor checks were weak. It remains useful only as donor material for movement parsing, emergency reinforcement, and rough fleet intent.

The practical direction is unchanged: build a small validation set from public replays, then test one subsystem at a time. The highest-value subsystem remains visible-fleet threat timing: infer likely targets, reserve only when arrival timing requires it, and avoid making four-player openings too passive.

## 2026-05-18 Public Review

The public-code refresh was partially blocked by API rate limiting, so no verified new Kaggle notebook was promoted for direct use. Discussion updates reinforced the same engineering themes: runtime uncertainty, environment parity, fast local rollout infrastructure, present-value target scoring, and replay-driven loss review.

An external public reference with broader strategy claims compiled locally, but a small mixed-anchor check was weak and slow. It remains donor material only, mainly for parsing, influence scoring, and target-timing ideas.

The immediate improvement priority is final-window selection discipline: preserve a stable distinct result when it is close to a volatile leader, instead of using both final slots on the same high-variance reference.

## 2026-05-19 Public Review

The newest public-code refresh surfaced validator and top-k selection ideas, a PPO-style reference, and several robust rule references. Local anchor checks did not provide enough evidence for a direct submission from these sources.

The useful takeaways are implementation-level rather than package-level: better timeout hygiene, stronger validation before final selection, and threat-timing ideas from visible movement. The next practical step is to convert these into a small replay-derived validation set before spending more public leaderboard slots.

## Next Priority

Build a small replay-mining dataset and use it to answer three questions:

- Which openings consistently survive strong four-player maps?
- Which defensive mistakes cause the largest public losses?
- Which pathing choices create sun or boundary losses after the recent collision changes?

The next implementation review should focus on whether visible opponent fleets can be converted into a reliable threat map without causing over-defense in four-player games.

## 2026-05-13 Public Review

The newest high-interest public reference combined search with a learned value estimate. The main takeaway was not to submit this type of reference unless all required local assets are packaged and checked against the competition runtime.

Public discussion still points toward visible opponent movement as the most actionable improvement path. The next useful implementation work is to convert that information into threat timing, likely targets, and defensive reserves without making the bot too passive.

## 2026-05-14 Public Review

No new same-day high-score public reference was found. A recent high-score reference from the public code section was reviewed and tried once, but the public result did not transfer.

The useful research direction remains subsystem work: visible movement threat timing, better defense reserves, and replay-derived validation. Direct reruns are not closing the gap to the top 10.

## 2026-05-15 Public Review

The newest public references added two useful research paths: value-search packaging and exposed-target logic. The value-search package was validated with its required value data file, but the public result still landed below the starting score. The exposed-target reference also did not transfer.

The main lesson is operational: preserve the best same-day score in the final active window. Mechanism-level work remains more promising than direct public-code reruns, especially visible fleet threat timing, target travel-time scoring, and robust per-game state reset handling.

## 2026-05-16 Public Review

Several new public references appeared, but none had enough evidence for direct submission. The most defensible public candidate was reviewed as a donor/reference only after local checks failed to show a clear advantage.

The useful direction remains targeted mechanism work rather than direct public-code reruns: visible fleet threat maps, travel-time target scoring, and stricter final-window preservation rules.
