# Experiment Log

## 2026-05-20 Export

Five submissions were used. The final exported leaderboard snapshot showed a public score of 910.7 and rank 448. The top 10 threshold was 1442.7.

| Iteration | Public score | Result |
| --- | ---: | --- |
| 1 | 752.3 | Best same-day individual result, still below the starting score. |
| 2 | 659.0 | Distinct recovery probe did not transfer. |
| 3 | 633.1 | Recovery rerun remained weak. |
| 4 | 836.9 | Final-window support result after delayed drift. |
| 5 | 910.7 | Final exported contributor and best same-day result. |

Lessons:

- A poor first-three sequence can still recover through a volatile reference, but final reporting needs a later fresh snapshot because scores can move substantially after the normal stabilization window.
- The final active result improved after delayed drift, so the immediate post-complete score alone would have understated the loop outcome.
- Public updates today were more useful for replay mining and validation infrastructure than direct submissions.

## 2026-05-19 Export

Five submissions were used. The final exported leaderboard snapshot showed a public score of 741.3 and rank 1126. The top 10 threshold was 1431.6.

| Iteration | Public score | Result |
| --- | ---: | --- |
| 1 | 872.8 | Best individual same-day result, but outside the final exported active result. |
| 2 | 642.5 | Distinct stability probe did not transfer strongly today. |
| 3 | 818.8 | Preservation rerun recovered into the useful range. |
| 4 | 601.3 | Final-window preservation attempt underperformed. |
| 5 | 741.3 | Final exported result, below the best same-day score. |

Lessons:

- Same-reference reruns can move by hundreds of points after completion, so final-window decisions need an extra stabilization gate.
- Do not spend both final slots on one volatile reference unless a final-window run has already stabilized above the preservation threshold.
- Recent public code was useful as reference material, but not as a direct submission candidate today.

## 2026-05-18 Export

Five submissions were used. The final exported leaderboard snapshot showed a public score of 793.3 and rank 869. The top 10 threshold was 1423.7.

| Iteration | Public score | Result |
| --- | ---: | --- |
| 1 | 843.5 | Best individual result of the day, but outside the final active window. |
| 2 | 805.2 | Best distinct reference result and the more stable active-window candidate. |
| 3 | 657.0 | Recovery rerun underperformed. |
| 4 | 716.3 | Final-window recovery remained below the distinct reference. |
| 5 | 793.3 | Final active contributor, below the best same-day results. |

Lessons:

- When a distinct candidate is above 800 and close to a volatile leader, preserve one final slot for that distinct candidate.
- Repeating the same high-variance reference in both final slots can erase the best same-day score.
- Public discussion and code refresh did not produce a direct-use candidate; replay-derived validation and better final-window selection remain the highest-value work.

## 2026-05-17 Export

Five submissions were used. The final exported leaderboard snapshot showed a public score of 835.1 and rank 688. The top 10 threshold was 1435.9.

| Iteration | Public score | Result |
| --- | ---: | --- |
| 1 | 939.5 | Best individual result of the day, from a known reference rerun. |
| 2 | 599.5 | Distinct hybrid reference did not transfer today. |
| 3 | 772.5 | Value-search reference improved after delayed scoring, but stayed below the preservation threshold. |
| 4 | 775.9 | First preservation rerun underperformed. |
| 5 | 835.1 | Final active contributor, below the strongest same-day result. |

Lessons:

- Same-reference reruns remain useful but very volatile; the best individual result did not reproduce in the final active slot.
- Public-code freshness was not enough for direct use today. New material was better treated as donor/reference material.
- Final-slot protection should still preserve the same-day leader, but high-variance reruns need longer stabilization before spending both final slots.

## 2026-05-16 Export

Five submissions were used. The final exported leaderboard snapshot showed a public score of 751.0 and rank 1031. The top 10 threshold was 1417.9.

| Iteration | Public score | Result |
| --- | ---: | --- |
| 1 | 758.0 | Known recovery reference started below the prior score line. |
| 2 | 795.7 | Distinct recovery reference became the early leader. |
| 3 | 847.1 | Best same-day individual result, but not preserved in the final active window. |
| 4 | 751.0 | Final-window preservation attempt underperformed. |
| 5 | 716.7 | Final active contributor, below the best same-day result. |

Lessons:

- The final active window must preserve the current same-day score leader, not the historically safest family.
- Once a candidate crosses the preservation threshold, wait for one more poll before spending the next slot.
- Public-code freshness alone was not useful today; local checks and same-day public score remain stronger signals.

## 2026-05-15 Export

Five submissions were used. The final exported leaderboard snapshot showed a public score of 825.6 and rank 705. The top 10 threshold was 1420.9.

| Iteration | Public score | Result |
| --- | ---: | --- |
| 1 | 584.1 | New exposed-planet public reference did not transfer. |
| 2 | 863.3 | Best individual result of the day, but not preserved in the final active window. |
| 3 | 679.3 | Recovery attempt underperformed. |
| 4 | 780.3 | Final-window recovery remained below the start line. |
| 5 | 825.6 | Final active contributor, below the prior exported score. |

Lessons:

- A validated multi-file value package can still underperform; packaging correctness is only a gate, not evidence of leaderboard transfer.
- If an exploratory entry is the best same-day score, it should be preserved in the final active window unless a later recovery attempt clearly beats it.
- Historical rerun peaks are not enough for final-slot decisions; final slots need same-day evidence.

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
