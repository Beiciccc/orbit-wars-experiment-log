# Experiment Log

## 2026-05-08 Export

The public leaderboard snapshot showed a score of 864.5 and rank 392 for the tracked team. The top 10 threshold was 1451.7.

The most important observation from the latest cycle is that direct public-code reruns and same-entry reruns remain highly volatile. A candidate can move by more than 100 public points after completion as more games are evaluated. The latest two active submissions also control the visible team score, so final slots need to preserve the best current-day result instead of spending the last slot on an unproven idea.

## 2026-05-07

Five submissions were used.

| Iteration | Public score | Result |
| --- | ---: | --- |
| 1 | 814.6 | Best exploratory entry of the day, still below the prior score line. |
| 2 | 808.3 | Stable enough to keep as a reference, but volatile across reruns. |
| 3 | 596.3 | Failed to transfer. |
| 4 | 715.8 | Failed to recover the prior score line. |
| 5 | 864.5 | Final active recovery; became the exported score. |

Lessons:

- Keep the strongest current-day score in one of the final two active slots.
- Treat public-code titles and local smoke tests as weak evidence.
- Use public replay data to build targeted regression cases before spending more quota.

## 2026-05-06

Five submissions were used. The best score observed that day was 894.7 from a high-base rerun, while the final active line ended near 880.6 after stabilization.

Lessons:

- The most reliable candidates were still heuristic strategy variants, not direct public-code copies.
- Local 2-player tests helped filter bad candidates but did not predict public score reliably.
- Four-player outcomes and opening failures dominated public volatility.

## 2026-05-05

Five submissions were used. The best observed score was 950.4, the strongest exported result in this log window.

Lessons:

- Same-code reruns can be useful for active recovery, but only when at least one later slot remains.
- The final slot should not be used for a risky experiment unless another active high score is already protected.

## 2026-05-04 And Earlier

Earlier iterations established the main operating pattern:

- public submissions can drift materially after initial completion
- four-player games are the main source of score variance
- direct public-code submissions rarely close the gap to the top 10
- replay analysis is more valuable than adding more broad local matches

The next improvement direction is to mine high-quality public replay datasets, extract early-game and defense patterns, and validate changes against replay-derived cases before public submission.
