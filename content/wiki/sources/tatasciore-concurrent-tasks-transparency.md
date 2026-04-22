# Do Concurrent Task Demands Impact the Benefit of Automation Transparency?

**Source file**: [Original article](../../raw/Tatasciore et al._Do concurrent task demands impact the benefit of automation transparency.pdf)

**Summary**: A mixed-design experiment using an uninhabited vehicle (UV) management task that found high automation transparency improved accuracy of automation use both with and without concurrent task demands, but with concurrent tasks it also led to higher trust, faster decisions, and increased automation bias — suggesting over-reliance on highly transparent systems under divided attention conditions.

**Sources**: Tatasciore et al._Do concurrent task demands impact the benefit of automation transparency.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Tatasciore, Bowden, and Loft (2023, *Applied Ergonomics*, 110, 104022) examined whether the established benefits of increased automation transparency persist when operators must simultaneously complete a non-automated concurrent task. The study used a mixed between-within design: N=212 undergraduate participants randomly assigned to low, medium, or high transparency (between-subjects), completing a UV mission task with and without a concurrent image analysis task (within-subjects).

The UV task required participants to select the optimal unmanned vehicle to complete a mission based on vehicle capabilities, mission-specific capability weightings, and environmental factors. The automated "Recommender" was 80% reliable. Transparency levels were:
- **Low transparency**: Table showing how the Recommender weighted each capability.
- **Medium transparency**: Table plus bar graphs showing calculated UV scores after environmental factors.
- **High transparency**: As medium, plus detailed bar graphs showing how scores were calculated step-by-step, including individual environmental factor contributions.

The concurrent task was an image-analysis task requiring participants to detect changes (appearance, disappearance, movement) of icons on an aerial map — emulating real-world multi-task UV operator workloads.

The paper is the predecessor to Tatasciore and Loft (2024; see [[tatasciore-loft-time-pressure-transparency]]), which used a near-identical task to examine time pressure instead of concurrent demands.

---

## Key Findings

- **Concurrent tasks degraded automation use accuracy**: Sensitivity d' was significantly lower with the concurrent task present (M=1.84) vs. absent (M=2.02, p=.002, η²=.05). Correct rejection rates also declined (0.67 present vs. 0.71 absent, p=.02). [Domain: defence/unmanned vehicle control simulation]
- **Concurrent tasks slowed decision times** and **increased perceived workload** substantially (workload: M=5.24 present vs. 4.26 absent, p<.001, η²=.39). [Domain: defence/unmanned vehicle control simulation]
- **High transparency improved accuracy vs. low transparency** both with and without concurrent demands — the effect size was nearly identical in both conditions (d≈0.42–0.71), and no interaction between transparency and concurrent task was found for this comparison. [Domain: defence/unmanned vehicle control simulation]
- **High vs. medium transparency under concurrent task demands** showed a more complex pattern: high transparency led to higher trust ratings (p=.004, d=0.49), faster decisions (p=.01, d=0.46), and greater automation bias (c: −0.56 high vs. −0.38 medium, p=.01, d=0.45), but not better accuracy than medium. This suggests operators provided high transparency adopted a strategy of greater reliance on the automation under dual-task conditions, reducing cognitive effort spent on verification. [Domain: defence/unmanned vehicle control simulation]
- **High transparency under concurrent tasks led to fewer false alarms** on the image analysis task vs. medium transparency (p=.002, d=0.55), indicating participants allocated more attention to the image analysis task when high transparency was available — possibly treating the Recommender as a reliable substitute for active verification. [Domain: defence/unmanned vehicle control simulation]
- **No interaction between transparency and concurrent task on overall sensitivity** (F<1), indicating high transparency did not mitigate the performance cost of concurrent task demands. [Domain: defence/unmanned vehicle control simulation]
- **Trust and usability**: Trust was higher with high than medium transparency when the concurrent task was present (p=.004), but not absent. No significant effect of transparency on usability. [Domain: defence/unmanned vehicle control simulation]
- Authors conclude this is the first study demonstrating high transparency can improve accuracy of automation use under dual-task conditions (vs. low transparency), but that under high concurrent demands, operators may shift to a reliance strategy — reducing verification effort and increasing automation bias — which is potentially dangerous with lower-reliability automation. [Domain: defence/unmanned vehicle control simulation]

---

## Transparency Constructs

This paper operationalizes a three-level **[[process-transparency]]** framework grounded in the SAT model (Chen et al., 2014):
- Low: Goal/intent level (why the automation was created, capability weightings).
- Medium: Reasoning level (which UV is rated better/worse, calculated scores).
- High: Projection/outcome level (step-by-step calculation, environmental factor contributions, uncertainty about scores).

The high-transparency condition implements **[[traceability]]** by visually exposing calculation steps — environmental hazard symbols, score adjustments, and final composite scores — in a graphical bar-chart display. This operationalization allows operators to detect specific errors made by the Recommender (missed factors, miscalculated impacts), enabling active verification rather than passive acceptance.

---

## Trust Constructs

- **[[cognitive-trust]]**: Measured via 6-item Merritt (2011) questionnaire (α=0.87–0.92). Trust was higher with high than medium transparency specifically under concurrent task conditions.
- **[[behavioural-trust]]** / **[[appropriate-reliance]]**: The primary behavioral measure is accuracy of automation use (d', hit rate, correct rejection rate). The concurrent-task findings reveal a shift toward **inappropriate reliance** under high transparency + high workload: higher bias (c), faster decisions, and lower correct rejection rates vs. medium transparency.
- **[[algorithm-aversion]]**: Not observed in this study; over-reliance rather than under-reliance was the concern.
- **[[trust-calibration]]**: Central concern. High transparency increased trust and improved accuracy in single-task contexts but led to miscalibrated over-reliance (higher bias, higher automation misuse risk) under concurrent task demands.

---

## Relevance to Research Questions

**RQ1**: Contributes precise operationalizations of both transparency (three-level SAT-based process transparency) and trust (self-reported cognitive trust + behavioral reliance indices) in a defence/automated decision support domain. The dual operationalization — subjective trust ratings alongside signal detection performance measures — is methodologically rigorous and domain-relevant.

**RQ2**: Key finding is a **conditional null**: high transparency does not moderate the negative effects of concurrent task demands on overall accuracy. However, the comparison with medium transparency under concurrent tasks reveals a nuanced positive relationship that transitions into over-reliance: high transparency raises both accuracy (vs. low) and automation bias (vs. medium). This non-linear pattern — where adding transparency initially helps but may produce automation bias under cognitive load — is a significant contribution to [[rq2-relationships]], particularly regarding boundary conditions of the transparency–trust–reliance relationship.

**RQ3**: All participants were undergraduate novices. Authors note the limitation and call for expert replication. The study does not examine how operator expertise or role moderates transparency effects, but the novice-only design is an acknowledged gap relevant to [[user-expertise]] and [[rq3-user-roles]].

---

## Related pages

- [[process-transparency]]
- [[traceability]]
- [[trust-calibration]]
- [[appropriate-reliance]]
- [[behavioural-trust]]
- [[tatasciore-loft-time-pressure-transparency]]
- [[rq2-relationships]]
