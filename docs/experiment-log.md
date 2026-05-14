# Experiment Log

## 2026-05-14 Export

Five submissions were used. The final exported leaderboard snapshot showed a public score of 851.9 and rank 591. The top 10 threshold was 1399.2.

| Iteration | Public score | Result |
| --- | ---: | --- |
| 1 | 803.2 | Prior strong reference did not recover its earlier right-tail score. |
| 2 | 728.3 | New public high-score reference did not transfer. |
| 3 | 805.0 | Best non-final-window recovery attempt. |
| 4 | 851.9 | Best final active contributor, but below the prior exported score. |
| 5 | 833.1 | Final active contributor, below iteration 4. |

Lessons:

- Same-code reruns are not a complete recovery strategy; high right-tail results can be hard to reproduce.
- When a mid-cycle recovery attempt beats the earlier probes, it should be considered for final-window preservation unless a stronger same-day candidate is available.
- Public high-score references still need replay or broader validation before being trusted as direct submissions.

## 2026-05-13 Export

Five submissions were used. The final exported leaderboard snapshot showed a public score of 927.6 and rank 392. The top 10 threshold was 1430.3.

| Iteration | Public score | Result |
| --- | ---: | --- |
| 1 | ERROR | New learned-value reference failed in the evaluation runtime. |
| 2 | 679.1 | Protective rerun underperformed. |
| 3 | 1066.9 | Best individual result of the day, but not preserved in the final active window. |
| 4 | 793.4 | Final active contributor, but below the prior exported score. |
| 5 | 927.6 | Final-window recovery preserved a usable score, but below the day's best result. |

Lessons:

- A strong same-day result must be preserved inside the final active window; otherwise it does not help the visible score.
- Multi-file learned-value entries need package compatibility checks before public submission.
- The next substantive improvement should focus on visible opponent movement, threat detection, and defense timing rather than more direct public-code reruns.

## 2026-05-12 Export

Five submissions were used. The final exported leaderboard snapshot showed a public score of 915.3 and rank 395. The top 10 threshold was 1441.1.

| Iteration | Public score | Result |
| --- | ---: | --- |
| 1 | 675.2 | Historical high scorer did not recover. |
| 2 | 566.9 | Public high-score reference did not transfer. |
| 3 | 802.5 | Best exploratory result of the day. |
| 4 | 915.3 | Best final active contributor after delayed stabilization. |
| 5 | 842.2 | Final recovery attempt underperformed. |

Lessons:

- Historical peak scores and public high-score labels were weak predictors today.
- The safest late-cycle move was still a known baseline rerun, but rerun variance remained large; the strongest score moved across a wide range before the latest stable check.
- The next improvement path should use visible opponent movement data for threat detection and defense timing, then validate against replay-derived cases before another broad submission cycle.

## 2026-05-09 Export

Five submissions were used. The best individual score observed today was 1031.7, but the final visible score settled at 908.4 because only the latest two active submissions count for the visible team score.

| Iteration | Public score | Result |
| --- | ---: | --- |
| 1 | 918.7 | Strong public result after score drift. |
| 2 | 829.7 | Moderate transfer. |
| 3 | 1031.7 | Best individual result in this log window, not preserved in final active slots. |
| 4 | 908.4 | Final active contributor. |
| 5 | 693.7 | Final-slot recovery attempt underperformed. |

Lessons:

- Wait longer for the first three submissions to stabilize before spending the final two slots.
- If a same-day result crosses 950, preserve that exact candidate in one of the final two slots.
- A historical fallback is not reliable enough for the final slot unless the previous slot already protects the visible score.

## 2026-05-08 Export

The public leaderboard snapshot showed a score of 864.5 and rank 433 for the tracked team. The top 10 threshold was 1451.7.

The most important observation from this cycle was that direct public-code reruns and same-entry reruns remained highly volatile. A candidate can move by more than 100 public points after completion as more games are evaluated.

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

Five submissions were used. The best observed score was 950.4.

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
