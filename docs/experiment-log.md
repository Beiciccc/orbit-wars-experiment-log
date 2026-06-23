# Experiment Log

## 2026-06-23 Live Update

The day started from a public leaderboard score of 1083.5 and rank 694. The rank-100 threshold was 1253.9, and the rank-500 threshold was 1113.9.

Fresh public review found no new official daily episode data beyond 2026-06-21 and no 2026-06-23 public-code run at refresh time. New discussion clarified that the deadline was not extended and lost attempts would not be refunded. One fresh weights-based package passed import and replay-state runtime checks, so it was used as the first probe. It returned the floor score and will not be repeated.

| Iteration | Public score | Result |
| --- | ---: | --- |
| 1 | 575.2 | Fresh weights probe did not transfer. |
| 2 | 844.9 | Recovery anchor drifted upward but stayed below the start line. |
| 3 | 706.2 | Recovery-family diversity sample stayed weak. |
| 4 | 600.0 | Final-window recovery initially returned the floor score. |

Current lessons:

- Runtime safety and replay-state checks are necessary but still not sufficient for live transfer.
- After a floor-score fresh probe and two weak recovery entries, the remaining two entries should be treated only as final-window recovery.
- The last two active entries remain the main closeout risk, so later entries must be selected for recovery rather than exploration.

## 2026-06-22 Live Update

Five entries were used after a fresh public-code, discussion, and official episode-data review. The latest exported leaderboard snapshot showed a public score of 978.0 and rank 1224. The rank-100 threshold was 1250.9, and the rank-500 threshold was 1117.8.

The day started from an 1100+ visible row near the rank-500 band. Fresh public-code probes from the prior day had transferred poorly, and new 2026-06-22 public discussion reported long pending queues, stale pairing concerns, and entries with few follow-up games. Because no new reference had stronger same-account evidence, all five entries used the established final-window anchor. The repeats did not preserve the starting line, and the last two entries controlled the exported row.

| Iteration | Public score | Result |
| --- | ---: | --- |
| 1 | 907.3 | Completed final-window anchor repeat. |
| 2 | 890.3 | Completed final-window anchor repeat. |
| 3 | 799.9 | Completed final-window anchor repeat. |
| 4 | 978.0 | Completed final-window anchor repeat. |
| 5 | 896.2 | Completed final-window anchor repeat. |

Current lessons:

- In the final window, same-account live evidence is stronger than public package labels.
- Recent public-code references remain useful for review, but they need stronger replay-derived outcome evidence before replacing the active anchor.
- Queue delays and delayed scoring require waiting for each official completion before using the next entry.
- Repeating a prior anchor can still erase a strong visible row when the latest two entries are both weak; preservation needs a stricter stop rule when early repeats fall below the starting line.

## 2026-06-21 Export

Five entries were used after a final-week public-code, discussion, and official episode-data review. The exported leaderboard snapshot showed a public score of 982.8 and rank 1263. The rank-100 threshold was 1265.3, and the rank-500 threshold was 1134.2.

The day started near 1080.6 and rank 795 after delayed score drift from the prior day. The latest official daily episode data was downloaded and used for replay-state screening. One new public reference looked best in that offline screen, but it did not transfer publicly. The final two entries returned to the established anchor family; they initially completed at the floor value, then drifted upward before the exported recheck.

| Iteration | Public score | Result |
| --- | ---: | --- |
| 1 | 744.5 | New four-player-oriented public-code probe did not transfer. |
| 2 | 799.0 | New frontier-style public-code probe stayed below the useful range. |
| 3 | 712.8 | Updated dynamic-control probe stayed below the useful range. |
| 4 | 982.8 | Final-window anchor drifted upward after a floor-value completion. |
| 5 | 964.8 | Final-window companion drifted upward after a floor-value completion. |

Lessons:

- Official replay-state screening is useful as a rejection filter, but coarse action matching is still not enough to predict leaderboard transfer.
- Public package labels and clean packaging remain weak evidence without same-account live evidence.
- When the first three entries are below 900, the last two entries should be treated as latest-window anchors, not expected improvement attempts, even if delayed scoring later improves them.

## 2026-06-20 Export

Five entries were used after a fresh public-code and public-data review. The final exported leaderboard snapshot showed a public score of 802.5 and rank 1675. The rank-100 threshold was 1261.8, and the rank-500 threshold was 1148.5.

The day started from 1125.1 and rank 641 after delayed score drift from the prior day. A newly published high-title public reference was rebuilt with its published utility dependency and tested once, then the remaining entries used established reference families and final-window guards. None recovered the starting line.

| Iteration | Public score | Result |
| --- | ---: | --- |
| 1 | 645.8 | Fresh high-title public-code exploration did not transfer. |
| 2 | 820.5 | Established reference family stayed below the starting line. |
| 3 | 832.3 | Recent public-row family stayed below the starting line. |
| 4 | 802.5 | Final-window guard became the exported contributor. |
| 5 | 739.4 | Final companion stayed weak. |

Lessons:

- Public title claims and exact dependency packaging are still not enough evidence for leaderboard transfer.
- Established reference families can recover from very low values, but not enough to protect an 1100+ start line.
- The next useful step is replay-state validation from the latest official public episode data before using more live entries on public-code probes.

## 2026-06-19 Export

Five entries were used after a fresh public-code and public-data review. The final exported leaderboard snapshot showed a public score of 753.9 and rank 1899. The rank-100 threshold was 1268.9, and the rank-500 threshold was 1157.0.

The day started from 1205.7 and rank 202 after the prior day's score drift. Because the starting window was already strong, all five entries used the same previously successful package as a preservation attempt. The repeats did not preserve the window, and the latest-two closeout row fell sharply.

| Iteration | Public score | Result |
| --- | ---: | --- |
| 1 | 910.0 | Same-package repeat did not reach the start line. |
| 2 | 826.3 | Same-package repeat stayed weak. |
| 3 | 827.2 | Same-package repeat stayed weak. |
| 4 | 753.9 | Exported contributor after latest-window replacement. |
| 5 | 701.3 | Final companion stayed weak. |

Lessons:

- A package that transferred once can still fail on exact repeat.
- Latest-window management matters: later weak entries can erase an earlier better repeat.
- The next useful step is offline replay-state validation before spending more live entries from a strong starting rank.

## 2026-06-18 Export

Five entries were used after a fresh public-code, discussion, and public-data review. The final exported leaderboard snapshot showed a public score of 810.3 and rank 1625. The rank-100 threshold was 1284.0, and the rank-500 threshold was 1167.5.

The day started from 1044.6 and rank 1128. Public-code archives and recent public rows were reviewed, cleaned, and locally checked, but none transferred. The best same-day entry settled at 810.3.

| Iteration | Public score | Result |
| --- | ---: | --- |
| 1 | 676.7 | Baseline time-matched probe stayed weak. |
| 2 | 724.8 | Embedded public archive did not transfer. |
| 3 | 725.4 | Clean rebuilt archive did not transfer. |
| 4 | 810.3 | Best same-day entry but still below the start line. |
| 5 | 737.3 | Public-row probe did not transfer. |

Lessons:

- Embedded archive labels and same-day public context are still not enough evidence for leaderboard transfer.
- Cleaning package structure prevents avoidable submission issues but does not predict score.
- The next useful step remains replay-state validation from recent public episode data before spending more entries on direct public-code probes.

## 2026-06-17 Export

Five entries were used after a fresh public-code, discussion, and public-data review. The final exported leaderboard snapshot showed a public score of 942.2 and rank 1322. The rank-100 threshold was 1282.1, and the rank-500 threshold was 1171.2.

The day started from 1024.8 and rank 1198. A fresh public-code candidate won the small local four-player screening, but it did not transfer publicly. A rebuild with the refreshed public utility data also stayed weak. The remaining entries returned to the known recovery family, which also failed to recover the starting line.

| Iteration | Public score | Result |
| --- | ---: | --- |
| 1 | 779.8 | Fresh public-code exploration did not transfer. |
| 2 | 797.6 | Rebuilt public-code exploration stayed weak. |
| 3 | 781.5 | Recovery entry stayed below the starting line. |
| 4 | 942.2 | Best same-day entry and exported contributor. |
| 5 | 843.8 | Final companion stayed weak. |

Lessons:

- Public-code recency, clean packaging, and small local match panels are still not enough to predict public transfer.
- Refreshing the shared public utility data fixed a real reproducibility issue but did not produce leaderboard transfer.
- The next useful step is replay-state validation from recent public episode data before using more entries on direct public-code probes.

## 2026-06-16 Export

Five entries were used after a fresh public-code and public-data review. The final exported leaderboard snapshot showed a public score of 1051.1 and rank 1101. The rank-100 threshold was 1279.7, and the rank-500 threshold was 1171.7.

The day started from 1062.1 and rank 1068. One clean public-code candidate was tested first after local screening, then the remaining entries returned to the previously validated recovery family. The run did not recover the starting line.

| Iteration | Public score | Result |
| --- | ---: | --- |
| 1 | 839.9 | Clean public-code exploration did not transfer. |
| 2 | 823.5 | Recovery entry stayed below the starting line. |
| 3 | 802.5 | Recovery entry stayed weak. |
| 4 | 1051.1 | Final-window recovery became the exported contributor. |
| 5 | 958.6 | Final companion stayed below the contributor. |

Lessons:

- Clean packaging and a small local panel are not enough for public transfer.
- Local four-player screening remains useful for blocking tilted candidates, but not for proving leaderboard upside.
- The next useful step is replay-state validation from recent public episode data before using more entries on direct public-code probes.

## 2026-06-15 Export

Five entries were used after a fresh public-code and public-data review. The final exported leaderboard snapshot showed a public score of 990.2 and rank 1148. The rank-100 threshold was 1290.2, and the rank-500 threshold was 1168.0.

The day started from 1145.5 and rank 604. Three fresh public-code candidates were tested after package cleanup and runtime checks, but none transferred to the visible leaderboard range suggested by their authors' current public rows. The final two entries returned to the previously validated family, but both landed below the starting window.

| Iteration | Public score | Result |
| --- | ---: | --- |
| 1 | 910.6 | Fresh public-code exploration did not transfer. |
| 2 | 755.3 | Fresh public-code exploration did not transfer. |
| 3 | 802.0 | Fresh public-code exploration did not transfer. |
| 4 | 990.2 | Recovery entry became the exported contributor but stayed below the start line. |
| 5 | 859.3 | Final companion stayed weak. |

Lessons:

- A high current public row from an author is not enough evidence that the downloadable notebook matches the submitted artifact.
- Local full-game panels remain useful for runtime screening, but not for predicting public transfer.
- The next useful step is replay-state validation from recent public episode data before using more entries on direct public-code probes.

## 2026-06-14 Export

Five entries were used after a fresh public-code and public-data review. The final exported leaderboard snapshot showed a public score of 1098.9 and rank 891. The rank-100 threshold was 1287.0, and the rank-500 threshold was 1165.1.

The day started from 1115.6 and rank 805. One fresh public-code entry was tested first, then recovery entries returned to the Flowdiff family. The run did not recover the starting line.

| Iteration | Public score | Result |
| --- | ---: | --- |
| 1 | 830.6 | Fresh public-code exploration did not transfer. |
| 2 | 810.6 | Flowdiff recovery stayed weak. |
| 3 | 1098.9 | Best same-day entry and exported contributor. |
| 4 | n/a | Submission recorded an error and produced no score. |
| 5 | 935.7 | Final recovery stayed below the contributor. |

Lessons:

- A small local edge is still not enough evidence for a fresh public-code entry above a 1100+ starting line.
- Flowdiff can still produce useful late drift, but the exported result remains volatile.
- Submission errors need immediate follow-up because they can consume quota.

## 2026-06-13 Export

Five entries were used after a fresh public-code and public-data review. The final exported leaderboard snapshot showed a public score of 1031.2 and rank 1013. The rank-100 threshold was 1289.7, and the rank-250 threshold was 1205.8.

The day started from 1056.4 and rank 979. No fresh public-code reference had reproducible evidence above the starting line, so all five entries used the known Flowdiff repeat family. The run did not recover the starting line.

| Iteration | Public score | Result |
| --- | ---: | --- |
| 1 | 805.7 | Stability repeat stayed below the starting line. |
| 2 | 849.7 | Stability repeat improved only modestly. |
| 3 | 780.2 | Stability repeat remained weak. |
| 4 | 999.1 | Same-family repeat stayed below the starting line after the final recheck. |
| 5 | 1031.2 | Exported contributor after late score drift. |

Lessons:

- Repeating the same Flowdiff family is still highly variable and did not protect a low 1050 line.
- The latest active window remained unstable across close-out checks.
- Future entries need replay-state validation from recent public episode data before more direct public-code probing.

## 2026-06-12 Export

Five entries were used after a fresh public-code review. The final exported leaderboard snapshot showed a public score of 1054.0 and rank 969. The rank-100 threshold was 1282.0, and the rank-250 threshold was 1202.1.

The day started from 1132.6 and rank 714. One fresh public-code entry was tested first, then exact Flowdiff repeats were used for final-window recovery. Neither path recovered the starting line.

| Iteration | Public score | Result |
| --- | ---: | --- |
| 1 | 850.2 | Fresh public-code exploration did not transfer. |
| 2 | 932.0 | Flowdiff repeat stayed below the starting line. |
| 3 | 820.2 | Flowdiff repeat stayed weak. |
| 4 | 940.5 | Final-window repeat did not recover. |
| 5 | 1054.0 | Final-window repeat became the exported contributor. |

Lessons:

- Local 4P win rate again failed as a submit gate.
- Exact Flowdiff did not produce a high-tail draw today.
- Future entries need replay-state validation from recent public episode data before more public-code probing.

## 2026-06-11 Export

Five entries were used after the next submission window opened. The final exported leaderboard snapshot showed a public score of 1124.9 and rank 747. The rank-100 threshold was 1275.5, and the rank-250 threshold was 1204.9.

The day started from 1151.6 and rank 614. One fresh public-code entry was tested first, then exact Flowdiff repeats were used for final-window recovery. The strongest transient delayed score was 1234.0, but the exported row settled lower.

| Iteration | Public score | Result |
| --- | ---: | --- |
| 1 | 810.4 | Fresh public-code exploration did not transfer. |
| 2 | 639.7 | Flowdiff repeat stayed weak. |
| 3 | 696.5 | Flowdiff repeat stayed weak. |
| 4 | 1124.9 | Final-window repeat became the exported contributor. |
| 5 | 1092.6 | Final-window companion stayed below the contributor. |

Lessons:

- Strong local 2P/4P validation still did not predict public transfer.
- Exact Flowdiff remains volatile and can show high transient peaks, but exported stability is the only usable signal.
- The next improvement step needs replay-state validation from recent public episode data before more direct public-code probes.

## 2026-06-10 Export

Five entries were used in a preservation attempt from a strong visible line. The final exported leaderboard snapshot showed a public score of 1096.2 and rank 753. The rank-100 threshold was 1267.2, and the rank-250 threshold was 1208.9.

The day started from 1198.7 and rank 305. One local Flowdiff variant was tested first, then four exact Flowdiff repeats were used for final-window recovery. The highest transient delayed score was 1183.3, but the exported row settled lower.

| Iteration | Public score | Result |
| --- | ---: | --- |
| 1 | 788.4 | Local conservative variant did not transfer. |
| 2 | 855.4 | Flowdiff repeat remained below the starting line. |
| 3 | 911.8 | Flowdiff repeat recovered only partially. |
| 4 | 1013.2 | Final-window repeat stayed below the active line. |
| 5 | 1096.2 | Final-window repeat became the exported contributor. |

Lessons:

- Local near-variant self-play is not enough evidence for a slot from a 1190+ visible line.
- Exact Flowdiff still has delayed-score upside but did not reproduce the prior top-100 tail today.
- The next improvement step needs replay-state validation from fresh public episode data.

## 2026-06-09 Export

Five entries were used in a top-100 recovery attempt. The final exported leaderboard snapshot showed a public score of 1272.4 and rank 95. The rank-100 threshold was 1269.8, and the rank-50 threshold was 1351.1.

The day started from a visible line at 1144.5. Two high-title Producer Hybrid entries did not transfer, then exact Flowdiff preservation recovered the final window after extended delayed scoring.

| Iteration | Public score | Result |
| --- | ---: | --- |
| 1 | 803.6 | Producer Hybrid reference did not transfer. |
| 2 | 731.2 | Producer Hybrid rebuild was weaker. |
| 3 | 600.0 | First Flowdiff repeat did not recover. |
| 4 | 1272.4 | Final-window repeat became the exported contributor. |
| 5 | 1147.4 | Final-window companion stayed below the contributor. |

Lessons:

- High-title public references need same-day evidence before taking more than one slot.
- Exact Flowdiff preservation remains volatile but can still reach the top-100 band.
- The exported row must be checked after delayed scoring; intermediate score spikes can reverse.

## 2026-06-08 Export

Five entries were used in a recovery attempt. The final exported leaderboard snapshot showed a public score of 1154.4 and rank 596. The rank-250 threshold was 1214.9, and the rank-100 threshold was 1268.6.

The day started from a strong visible line at 1160.5. Two public-code exploration entries were weak, then exact Flowdiff preservation partially recovered after extended delayed scoring, but the exported row still finished below the starting line.

| Iteration | Public score | Result |
| --- | ---: | --- |
| 1 | 796.7 | High-title rollout reference did not transfer. |
| 2 | 695.6 | Refreshed Flowdiff variant underperformed the older exact package. |
| 3 | 600.0 | Recovery repeat did not recover. |
| 4 | 1119.3 | Final-window repeat recovered partially. |
| 5 | 1154.4 | Final-window repeat became the exported contributor, below the starting line. |

Lessons:

- From a 1150+ visible line, direct public title probes need same-day evidence before taking more than one slot.
- Exact Flowdiff preservation remains the strongest current family.
- Delayed scoring must be polled for a long window, but a transient peak should not be treated as stable until the exported row is rechecked.

## 2026-06-07 Export

Five entries were used in an aggressive improvement search. The final exported leaderboard snapshot showed a public score of 1049.7 and rank 619. The rank-100 threshold was 1266.0.

The day started from a visible line just above 1000. A refreshed Flowdiff public reference became the best same-day signal, and the final repeat improved the exported row after extended delayed scoring.

| Iteration | Public score | Result |
| --- | ---: | --- |
| 1 | 1024.3 | Refreshed Flowdiff reference became the best same-day signal. |
| 2 | 978.9 | ProducerLite reference recovered to the high-900 range. |
| 3 | 695.8 | High-title public fork did not transfer. |
| 4 | 979.2 | Recovery reference provided a weaker final companion. |
| 5 | 1049.7 | Flowdiff repeat became the exported contributor after delayed scoring. |

Lessons:

- When an early entry beats the starting visible line, preserve that exact run immediately; do not rely on a later repeat reproducing it.
- Refreshed Flowdiff is a useful current reference, but not yet a top-100 path.
- The next improvement path is replay-derived tuning from the latest public episode data, not another high-title fork.

## 2026-06-06 Export

Five entries were used in a top-100 attempt. The final exported leaderboard snapshot showed a public score of 944.2 and rank 815. The rank-100 threshold was 1264.3.

The day started from a stronger active window above 970. Fresh public references and one historical high-title package were tested first, but none reached the starting window. The final-window repeats also underperformed.

| Iteration | Public score | Result |
| --- | ---: | --- |
| 1 | 922.8 | New multi-focus public reference transferred moderately but stayed below the start line. |
| 2 | 925.3 | New Carbon v2 public reference became the best same-day probe, still far from top 100. |
| 3 | 836.1 | Historical high-title package did not reproduce its title range. |
| 4 | 831.0 | Final-window repeat recovered partially after delayed scoring. |
| 5 | 944.2 | Final-window companion became the exported contributor but remained below the start line. |

Lessons:

- A top-100 attempt needs fresh same-day evidence above 1100 or a replay-derived validation result; public title claims alone are not enough.
- The current final-window repeat family is too volatile to protect a 970+ starting window.
- If fresh probes stay below the weaker active score, adjacent direct reruns should stay research-only.

## 2026-06-05 Export

Five entries were used. The final exported leaderboard snapshot showed a public score of 1016.7 and rank 647. The top 10 threshold was 1542.9.

The day started from a strong active window above 1000. One newly published high-title reference was tested first, then the remaining entries returned to the known high-variance family after the new reference did not reproduce the claimed range.

| Iteration | Public score | Result |
| --- | ---: | --- |
| 1 | 872.2 | New high-title public reference did not reproduce its published range. |
| 2 | 919.6 | Same-family recovery reached the best non-final-window result. |
| 3 | 736.1 | Recovery repeat stayed weak. |
| 4 | 1016.7 | Final-window entry became the exported contributor after delayed scoring. |
| 5 | 750.8 | Final companion recovered partially but stayed weaker. |

Lessons:

- Public title claims above 1200 are useful discovery signals but are not reproducibility evidence.
- A high active window above 1000 should not be displaced without a fresh result already above the weaker active score.
- Same-family reruns remain capable of late recovery, but final-window companion variance is still the main failure mode.

## 2026-06-04 Export

Five entries were used. The final exported leaderboard snapshot showed a public score of 885.1 and rank 843. The top 10 threshold was 1525.8.

The day started from a strong active window near the 1000-point band, but repeated same-family reruns did not reproduce that band in the final exported snapshot.

| Iteration | Public score | Result |
| --- | ---: | --- |
| 1 | 812.1 | Same-family preservation run recovered from a low initial value but stayed below the starting line. |
| 2 | 816.9 | Second preservation run stabilized in the same range. |
| 3 | 844.3 | Best same-day individual result, still below the prior active window. |
| 4 | 885.1 | Final-window entry became the exported contributor after delayed scoring. |
| 5 | 835.7 | Final companion improved after delayed scoring but remained weaker. |

Lessons:

- A 1000+ active window should not be displaced without fresh same-day evidence above the weaker active score.
- Same-family reruns can still drift upward from low initial values, but the current observed band is too wide to treat as reliable high-score preservation.
- New public references need direct runnable form and stronger same-day evidence before taking quota against a high active window.

## 2026-05-31 Export

Five entries were used. The final exported leaderboard snapshot showed a public score of 815.2 and rank 1035. The top 10 threshold was 1520.9.

| Iteration | Public score | Result |
| --- | ---: | --- |
| 1 | 710.6 | New public-code reference did not transfer. |
| 2 | 822.8 | New public-code reference showed moderate transfer but was displaced from the final active window. |
| 3 | 899.1 | Verified baseline became the best same-day result but was displaced. |
| 4 | 758.0 | Final-window recovery repeat did not reproduce the prior run. |
| 5 | 815.2 | Final companion recovered partially but remained below the start line. |

Lessons:

- A same-day result near 900 must be preserved in the latest active window unless a later result is already higher.
- Public-code title claims did not transfer reliably; they need stronger validation before final-window use.
- Final-window choices should preserve the current-day leader before attempting another family rerun.

## 2026-05-29 Recovery Export

Three additional accepted entries were used after the earlier five-entry loop. The final exported leaderboard snapshot showed a public score of 976.7 and rank 296. The top 10 threshold was 1547.7.

| Iteration | Public score | Result |
| --- | ---: | --- |
| 1 | 827.4 | Same-family recovery probe restored a moderate floor. |
| 2 | 976.7 | Final-window recovery became the exported contributor. |
| 3 | 916.2 | Final companion stayed useful and kept the active window in the same validated family. |

Lessons:

- When the strongest same-day family has already shown a clear lead, repeating it in the active window can recover a failed final state.
- Family diversity is less important than preserving a demonstrated current-day scorer when the companion family has weak same-day evidence.
- Fresh leaderboard exports are necessary after recovery runs because public scores continue to drift after completion.

## 2026-05-29 Export

Five entries were used. The final exported leaderboard snapshot showed a public score of 758.2 and rank 1239. The top 10 threshold was 1536.8.

| Iteration | Public score | Result |
| --- | ---: | --- |
| 1 | 893.1 | Verified public baseline was the best same-day individual result but was displaced from the final active window. |
| 2 | 714.3 | Historical high-reference entry stayed below the preservation threshold. |
| 3 | 774.1 | Second verified-baseline run recovered modestly but was also displaced. |
| 4 | 758.2 | Final-window preservation entry briefly drifted higher, then settled as the exported contributor. |
| 5 | 641.7 | Final companion reference did not provide protection after delayed scoring. |

Lessons:

- The strongest same-day result must remain in the final active window when later results are materially weaker.
- A temporary late score spike is not enough for final protection unless it holds across repeated fresh checks.
- Historical strength alone should not justify a final companion entry without same-day evidence above the damage-control threshold.

## 2026-05-27 Export

Five submissions were used. The final exported leaderboard snapshot showed a public score of 953.8 and rank 370. The top 10 threshold was 1508.2.

| Iteration | Public score | Result |
| --- | ---: | --- |
| 1 | 768.6 | Historical high-reference entry recovered modestly after delayed scoring. |
| 2 | 857.3 | Verified public baseline recovered but was outside the final active window. |
| 3 | 750.7 | Second high-reference run recovered modestly. |
| 4 | 953.8 | Final-window companion recovered strongly and became the exported contributor. |
| 5 | 859.9 | Required historical best reference recovered after delayed scoring. |

Lessons:

- A pre-committed final entry makes the fourth slot decisive; it should be the strongest distinct family with recent drift evidence.
- Low initial completions still require extended polling. The fourth entry moved from 600.0 to 953.8 in the latest exported snapshot.
- New public references remained validation-only after bounded screening.

## 2026-05-26 Export

Five submissions were used. The final exported leaderboard snapshot showed a public score of 799.7 and rank 982. The top 10 threshold was 1469.0.

| Iteration | Public score | Result |
| --- | ---: | --- |
| 1 | 793.7 | Verified public baseline recovered after delayed scoring but was displaced from the final active window. |
| 2 | 824.0 | Known high-variance reference recovered after delayed scoring but was displaced later. |
| 3 | 876.7 | Best same-day result, but outside the final active window. |
| 4 | 653.2 | Final-window support entry stayed weak. |
| 5 | 799.7 | Final exported contributor after late drift, still below the best same-day result. |

Lessons:

- Low initial completions can be misleading; two references recovered by more than 200 points after additional polling.
- A same-day result drifting above 800 should be preserved in the final active window instead of being displaced by a historical fallback.
- Public refresh produced useful references and data sources, but no new direct-use candidate beat the validated references in bounded screening.

## 2026-05-25 Export

Five submissions were used. The final exported leaderboard snapshot showed a public score of 895.8 and rank 535. The top 10 threshold was 1485.3.

| Iteration | Public score | Result |
| --- | ---: | --- |
| 1 | 676.2 | Known high-variance reference underperformed. |
| 2 | 598.5 | Damage-control reference failed to establish a floor. |
| 3 | 822.1 | Same high-variance family recovered but was outside the final active window. |
| 4 | 895.8 | Verified public baseline recovered after delayed scoring and became the exported contributor. |
| 5 | 642.7 | Final companion entry stayed weak. |

Lessons:

- A verified public baseline can be the best recovery path when familiar references start weak.
- Do not treat the damage-control family as automatic final protection unless it has already shown a current-day score above the preservation threshold.
- Runtime-stalled public candidates should remain reference material until a bounded validation run completes.

## 2026-05-24 Export

Five submissions were used. The final exported leaderboard snapshot showed a public score of 811.1 and rank 858. The top 10 threshold was 1504.6.

| Iteration | Public score | Result |
| --- | ---: | --- |
| 1 | 624.4 | Known high-variance reference underperformed. |
| 2 | 801.0 | New public-code reference became the best individual same-day result after delayed scoring. |
| 3 | 800.7 | Damage-control reference recovered after delayed scoring but was not preserved in the final active window. |
| 4 | 811.1 | Final-window recovery became the exported contributor after stabilization. |
| 5 | 744.0 | Final companion entry recovered after late drift but stayed below the exported contributor. |

Lessons:

- Preserve a completed same-day score above 800 in the final active window instead of relying on a fresh rerun of the same family.
- Delayed public scoring remains material; multiple entries moved by more than 190 points after initial completion.
- Public-code title claims can identify candidates to test, but final-slot decisions need current active-window evidence.

## 2026-05-23 Export

Five submissions were used. The final exported leaderboard snapshot showed a public score of 841.2 and rank 743. The top 10 threshold was 1499.7.

| Iteration | Public score | Result |
| --- | ---: | --- |
| 1 | 698.6 | Known high-variance reference underperformed. |
| 2 | 685.2 | Same reference remained weak. |
| 3 | 883.5 | Best same-family result, but outside the final active window. |
| 4 | 841.2 | Final-window damage-control entry and exported contributor after late drift. |
| 5 | 708.1 | Final preservation attempt failed. |

Lessons:

- A distinct damage-control entry can be the best final-window protection when repeated high-variance reruns underperform.
- If a damage-control entry drifts above 850, preserve that family in the final slot unless a stronger final-window result is already active.
- New public-code forks need bounded validation before use; slow local screening is itself a runtime-risk signal.

## 2026-05-22 Export

Five submissions were used. The final exported leaderboard snapshot showed a public score of 657.2 and rank 1601. The top 10 threshold was 1494.2.

| Iteration | Public score | Result |
| --- | ---: | --- |
| 1 | 526.0 | Known high-variance reference failed today. |
| 2 | 718.1 | Distinct reference improved after delayed scoring but stayed below the start line. |
| 3 | 807.4 | Best same-day result, but outside the final active window. |
| 4 | 657.2 | Final-window recovery attempt failed after limited late drift. |
| 5 | 619.4 | Final exported companion result, also failed. |

Lessons:

- Once the same high-variance reference has two same-day failures below 650, it should not take both final slots.
- If the best same-day score is only around 800, preserving it can still be better than pursuing a low-probability final-window recovery.
- New public code and discussion updates were useful for validation planning, not direct submission.

## 2026-05-21 Export

Five submissions were used. The final exported leaderboard snapshot showed a public score of 963.6 and rank 275. The top 10 threshold was 1456.1.

| Iteration | Public score | Result |
| --- | ---: | --- |
| 1 | 936.1 | Strong early same-day result, later exceeded by the final entry. |
| 2 | 644.6 | Distinct public-code reference did not transfer. |
| 3 | 693.1 | Second distinct reference remained weak. |
| 4 | 879.9 | Final-window support result after delayed drift. |
| 5 | 963.6 | Final exported contributor and best same-day result. |

Lessons:

- Repeating the strongest same-day reference recovered only after a late score refresh.
- The final two entries drifted upward by more than 250 points after initial completion, so delayed scoring remains material.
- Recent public material was more useful for replay mining and validation than direct submission.

## 2026-05-20 Export

Five submissions were used. The final exported leaderboard snapshot showed a public score of 942.7 and rank 341. The top 10 threshold was 1442.7.

| Iteration | Public score | Result |
| --- | ---: | --- |
| 1 | 752.3 | Best same-day individual result, still below the starting score. |
| 2 | 659.0 | Distinct recovery probe did not transfer. |
| 3 | 633.1 | Recovery rerun remained weak. |
| 4 | 875.4 | Final-window support result after delayed drift. |
| 5 | 942.7 | Final exported contributor and best same-day result. |

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

## 2026-06-03 Export

Five submissions were used. The exported leaderboard snapshot shows a visible score of 869.1 and rank 891. The top 10 threshold was 1551.8.

The day started from a much stronger visible line of 1046.6. New public references were reviewed locally, but none had enough evidence to justify a public probe against that starting score, so all five submissions used the same known recovery family.

| Iteration | Public score | Result |
| --- | ---: | --- |
| 1 | 829.3 | Same-family repeat, below the starting line. |
| 2 | 813.8 | Same-family repeat, below the starting line. |
| 3 | 823.6 | Same-family repeat, below the starting line. |
| 4 | 869.1 | Final visible contributor. |
| 5 | 833.3 | Final companion result. |

Lessons:

- Exact same-family repeats can fail to preserve a 1000+ visible score.
- The known recovery family remains volatile and should be treated as an 800-1050 range, not a safe high-score lock.
- Public replay analysis is now more important than additional broad local gates.

## 2026-06-02 Export

Five submissions were used. The exported leaderboard snapshot shows a visible score of 958.8 and rank 547. The top 10 threshold was 1510.5.

The day started from a stronger visible line of 1048.2, so the five-submission cycle carried meaningful downside risk. One recent public reference was tested first, then the remaining submissions returned to the known recovery family.

| Iteration | Public score | Result |
| --- | ---: | --- |
| 1 | 791.9 | Recent public reference; local validation did not transfer enough. |
| 2 | 924.7 | Known recovery family, delayed upward movement. |
| 3 | 870.5 | Same recovery family, moderate result. |
| 4 | 958.8 | Final visible score after delayed movement. |
| 5 | 814.2 | Final companion result, below the visible contributor. |

Lessons:

- A high starting visible score should allow only one exploratory submission before recovery repeats.
- The exact known file was stronger evidence than a same-title refreshed public variant.
- Final-window scores can still move very late; the visible contributor rose from an initial low score to 958.8.

## 2026-06-01 Export

Five submissions were used. The exported leaderboard snapshot shows a visible score of 904.1 and rank 693. The top 10 threshold was 1506.1.

The day started from a stronger visible line near 1049.5 after delayed score movement from the previous cycle. The new cycle did not preserve that line, but it identified one repeatable public reference family that recovered from low first scores into the 900 range.

| Iteration | Public score | Result |
| --- | ---: | --- |
| 1 | 888.2 | Started low, then rose materially after delayed scoring. |
| 2 | 640.7 | Did not reproduce the prior high score. |
| 3 | 825.3 | Moderate recovery, below the prior visible line. |
| 4 | 904.1 | Best final-window result and exported visible score. |
| 5 | 809.2 | Started low, then partially recovered. |

Lessons:

- Initial completed scores were not reliable enough for final decisions; several entries moved by more than 100 points afterward.
- The final two submissions should be chosen from current-day evidence once a visible line is already above 1000.
- Public-reference labels and short local tests remain weak predictors; delayed public-score behavior is a separate signal that must be tracked.

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
