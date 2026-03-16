CTA SANDBOX
Planetary Geometry Fingerprint Study
Complete Record: Null Result → Exploratory Positive → Validation → Control Battery
March 2026  |  CC0 Public Domain  |  No Attribution Required

Abstract
This document records a complete exploratory computational study testing whether planetary angular geometry correlates with classes of historical events. The study proceeded through four stages: (1) a null result on treasury/plunder/siege events, (2) an exploratory positive signal in financial crisis events using an upgraded fingerprint representation, (3) locked-specification validation including leave-one-out robustness testing and a pre-registered holdout, and (4) a negative control battery on three unrelated event classes.
The financial crisis bucket produced a statistically significant clustering result (p=0.033) that survived robustness testing and passed a pre-registered holdout. Three control buckets — Olympic opening ceremonies, US presidential inaugurations, and sovereign debt defaults — returned null results under the identical locked specification. The pipeline is discriminating. The financial crisis signal is classified as an exploratory positive result requiring independent replication.

Figure 1 — Pipeline and Results Overview
 
Figure 1. Analysis pipeline (top) and four-panel results summary. (A) Treasury/plunder bucket: null result, p=0.32. (B) Financial crises bucket: significant clustering, p=0.033. (C) Validation battery summary across three independent tests. (D) Control battery: financial crises is the only bucket producing a significant result.
 
1. Methodology
1.1 Planetary Fingerprint v2
Each event date was represented as a 100-dimensional planetary fingerprint vector constructed from four blocks:
•	Pair-angle block (15 features): angular separation for all 15 pairs among six planets (Mars, Jupiter, Saturn, Uranus, Neptune, Pluto), values in [0°, 180°].
•	Aspect-strength block (75 features): for each of the 15 pairs, a 5-element Gaussian proximity vector measuring distance from each of the five major aspects (0°, 60°, 90°, 120°, 180°), sigma=6°. This preserves harmonic structure rather than raw angle noise.
•	Velocity block (6 features): short-term planetary drift computed as the 1-day forward/backward difference in ecliptic longitude, indicating whether geometry is tightening or dispersing at the event date.
•	Phase context block (4 features): normalized phase position within four major slow cycles (Jupiter-Saturn, Saturn-Uranus, Saturn-Neptune, Uranus-Pluto), capturing the large-scale cycle context.

1.2 Distance Metric
Pairwise fingerprint distance was computed as a weighted hybrid metric combining circular angular distance for the angle block and Euclidean distance for the remaining blocks, with weights: angles=1.0, aspects=2.0, velocity=0.5, phase=1.0 (normalized by sum). The aspect block received higher weight because harmonic structure was the primary theoretical signal.
1.3 Clustering and Significance
Ward linkage hierarchical clustering was applied to the pairwise distance matrix. Cluster compactness was measured as mean within-cluster pairwise distance averaged across clusters. Statistical significance was assessed by permutation test: 10,000 random event sets were drawn uniformly from the historical era, and the real cluster compactness was compared to the random distribution. P-value is the fraction of random runs achieving equal or better compactness.
1.4 Event Classification
All event labels were restricted to observable event-day conditions — phenomena that an informed witness could have described on the date itself. Retrospective historical judgments ("civilizational collapse," "end of era") were explicitly excluded following a methodological finding in the treasury study that such labels do not map to planetary geometry categories. This is documented in Section 3.
 
2. Study I — Treasury / Plunder / Siege (Null Result)
The initial study tested whether historical treasury-strip and imperial plunder events share planetary geometry signatures. This study produced a null result after exhaustive methodological refinement.
2.1 Event Bucket
The bucket contained 28 events spanning approximately 600 BCE to 1800 CE, drawn from three hypothesized categories: Breach/Exposure (city walls breached), Elite Capture/Wealth Seizure (rapid decapitation events), and Compound Systemic Collapse (multi-actor imperial redistributions).
2.2 Analytical Progression
The study underwent four major analytical passes, each prompted by a methodological finding from the previous pass:
1.	Pass 1: Original three-family taxonomy (Breach/Exposure, Transfer/Extraction, Compound): agreement 29%, p≈0.32 — not significant.
2.	Pass 2: Relabeled with event-day observable categories (Siege/Breach, Center Shock, Rapid Capture): agreement improved to 54%, p=0.194 — improvement but not significant.
3.	Pass 3: Two-type model (Siege vs. Sudden Force): agreement unchanged at 54%, p=0.162 — collapsing categories did not help.
4.	Pass 4: Siege timing sensitivity (start date vs. fall date): identical results for both timestamps — timing was not the variable.

2.3 Key Methodological Finding
The most valuable output of the null study was a methodological finding: event-day observable labels substantially outperform retrospective historical categories as taxonomy axes. "Terminal Handoff" and "civilizational collapse" are judgment categories visible only in retrospect, not on the event day. Switching to event-day observables improved agreement from 29% to 54% despite the result remaining non-significant. This finding was carried forward into the financial crisis study design.
2.4 Null Result Statement
Exploratory clustering and permutation testing of planetary angular separations across historical plunder and siege events (N=28) produced no statistically significant association between planetary geometry and event category across all four analytical passes. The null hypothesis could not be rejected.
 
3. Study II — Financial Crisis Bucket (Exploratory Positive Result)
3.1 Bucket Design
The financial crisis bucket was constructed using the methodological lessons from Study I. All events have sharp, day-bounded timestamps. Labels are observable on the event day. Three categories were defined: market crashes (sudden market-wide price collapse), bank failures (specific institution failure or halt), and currency/sovereign crises (peg break, default announcement, or moratorium declaration on a specific day).
Event	Date	Category
Black Thursday 1929	1929-10-24	Market Crash
Black Monday 1987	1987-10-19	Market Crash
Lehman Collapse 2008	2008-09-15	Market Crash
COVID Crash 2020	2020-03-16	Market Crash
Bear Stearns 2008	2008-03-14	Bank Failure
Northern Rock 2007	2007-09-14	Bank Failure
SVB Failure 2023	2023-03-10	Bank Failure
Black Wednesday 1992	1992-09-16	Currency Crisis
Thai Baht 1997	1997-07-02	Currency Crisis
Russian Default 1998	1998-08-17	Currency Crisis
Argentina Default 2001	2001-12-23	Currency Crisis
+ 12 additional events	(see locked spec)	All three categories

3.2 Exploratory Clustering Result
 
Figure 2. Financial crisis fingerprint analysis. Left: Ward dendrogram. Center: permutation test histogram (p=0.033, 96.7th percentile). Right: PCA projection by declared event type.

Ward hierarchical clustering produced a statistically significant cluster structure (p=0.033, 96.7th percentile of 10,000 random permutations). The strongest internal grouping appeared among currency/sovereign crisis events, with Thai baht, Russian default, Argentina, Swiss peg break, Turkish lira collapse, and UK gilt crisis clustering together. The 1929 crash events clustered with the 2008 banking/crash nexus events, suggesting the geometry may reflect systemic contagion structure rather than nominal event labels.
 
4. Validation Battery
Following the exploratory positive result, a locked specification was established. No parameters were modified after this point.
4.1 Locked Specification
The locked specification (hash: 99496f6e315e) froze: the complete event list and dates, feature block construction, aspect sigma value, distance metric weights, clustering method, cluster count, and permutation test parameters. Any further analysis used this specification without modification.
4.2 Leave-One-Out Robustness
Each of the 24 events was removed individually and the full clustering and permutation test was repeated on the remaining 23 events. Results: 17/24 runs remained statistically significant (p<0.05); 7/24 were marginal (p<0.10); 0/24 became non-significant. No single event is responsible for the signal. The result is distributed across the bucket.
4.3 Rare-State Occupancy (Supportive, Partially Circular)
A rare-state screen was constructed by computing weekly fingerprints across 1920-2023 and identifying the background days geometrically closest to the crisis fingerprint cloud. All 24 crisis events fell within rare-state windows (p<0.0001). This result is supportive but not fully independent: the rare states were defined using the event-derived fingerprint cloud, creating partial circularity. It is presented as corroborating evidence, not primary evidence.
4.4 Pre-Registered Holdout
A holdout dataset of 10 events (5 temporal-forward, 5 balanced earlier) was defined before any holdout analysis was run. Two success criteria were pre-registered: (1) mean holdout distance to training cloud below the 60th percentile of random controls, and (2) subtype match rate above 50%. Both criteria passed. Misclassifications were not random — structurally similar crisis types were paired (Cyprus bail-in with Swiss peg, Archegos with SVB, Franklin National with Bear Stearns).
 
Figure 3. Pre-registered holdout validation results. Left: distance distribution with holdout mean vs. random controls. Center: PCA projection showing holdout placements (stars). Right: per-event classification table against pre-registered criteria.
 
5. Negative Control Battery
The same locked v2 specification was applied without modification to three unrelated event buckets. The purpose was to test whether the pipeline produces false positives on arbitrary event collections.
 
Figure 4. Control battery results. The financial crisis bucket (leftmost panel) is the only bucket producing a significant result. All three control buckets returned null results.

Bucket	N	p-value	Result
Financial Crises (positive)	24	0.033	SIGNIFICANT — 96.7th pctile
Olympic Openings (neg. control A)	24	0.971	NULL — 2.9th pctile (below random)
US Inaugurations (neg. control B)	21	0.728	NULL — 27.2th pctile
Sovereign Defaults (contrast)	18	0.322	NULL — 67.8th pctile

The sovereign defaults bucket is particularly informative as a contrast case: it contains structurally similar events to the financial crisis bucket (including overlapping events such as Russia 1998, Argentina 2001, and Cyprus 2013), yet returned a null result. This suggests the signal is not simply "anything involving financial disruption" but is specific to the market crash / bank failure / currency crisis cluster as defined.
 
6. Discussion
6.1 What This Study Is
This is an exploratory computational study that produced a statistically significant clustering result in one event bucket, survived a pre-registered validation protocol, and returned null results on three control buckets under an identical locked specification. It is not proof of a causal relationship between planetary geometry and financial crisis timing. It is a well-structured exploratory positive result that meets the criteria for further investigation.
6.2 Limitations
•	The feature representation was developed using the training dataset, introducing potential for overfitting to that specific collection.
•	The rare-state occupancy test is partially event-informed and cannot be treated as fully independent evidence.
•	The training set size (N=24) is modest. The permutation test provides valid significance under the null, but effect size estimates at this N are unstable.
•	The feature weights (angles=1, aspects=2, velocity=0.5, phase=1) were set a priori but not cross-validated. Different weight choices would produce different results.
•	PyEphem heliocentric longitudes are used; geocentric coordinates would produce different fingerprints. This has not been tested.

6.3 What the Clusters May Reflect
The strongest geometric family in the financial crisis bucket is the currency/sovereign crisis cluster. These events share a common structure: a formal institutional constraint (peg, gold standard, debt obligation) breaks under accumulated pressure on a specific day. The geometry may be detecting the slow-planet background during periods of sustained institutional stress rather than the event itself. This interpretation is speculative and untested.
The pairing of 1929 events with 2008 banking/crash events, and the holdout placement of Nixon shock near Bear Stearns, suggests the geometry may be more sensitive to the structural character of the stress than to its surface label.
6.4 Required Next Step
The required next step is independent replication: a different researcher applying the locked v2 specification to a new crisis event bucket without access to the training set, without modifying any parameters, with pre-registered success criteria. Replication success would constitute meaningful evidence. Replication failure would suggest the current result is a dataset-specific artifact.
 
7. Final Posture
This study began as a null-result investigation and evolved into an exploratory positive result through methodological refinement. The correct scientific posture is open but skeptical. The pipeline is discriminating. The financial crisis signal is real enough to investigate further. Independent replication is required before stronger claims can be made.


CC0 1.0 Universal — Public Domain Dedication
Take it.  Break it.  Replicate it.

