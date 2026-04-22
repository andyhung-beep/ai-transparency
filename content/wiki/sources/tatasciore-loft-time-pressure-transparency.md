# Can Increased Automation Transparency Mitigate the Effects of Time Pressure on Automation Use?

**Source file**: [Original article](../../raw/Tatasciore, M., & Loft, S. (2024). Can increased automation transparency mitigate the effects of time pressure on automation use_.pdf)

**Summary**: An experimental study using an uninhabited vehicle (UV) management task that found high automation transparency improved accuracy and trust but did not buffer against the negative effects of high time pressure on automation use accuracy or perceived workload.

**Sources**: Tatasciore, M., & Loft, S. (2024). Can increased automation transparency mitigate the effects of time pressure on automation use_.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Tatasciore and Loft (2024, *Applied Ergonomics*, 114, 104142) investigated whether increased automation transparency could offset the degrading effects of time pressure on human–automation teaming performance. The study used a within-subjects design (N=64 undergraduate participants) in a simulated defence task involving uninhabited vehicle (UV) management, where participants had to accept or reject automated recommendations from an "Recommender" system operating at 80% reliability.

The study crossed two factors within-subjects: automation transparency (low vs. high) and time pressure (low = 25s per decision, high = 12s per decision). The SAT (Situation-Awareness Agent-Based Transparency) model (Chen et al., 2014) guided the transparency design:
- **Low transparency**: Table display showing the Recommender's capability weightings (broadly SAT Level 1).
- **High transparency**: Additional bar graphs showing how the Recommender calculated each UV's capability scores, including environmental factor impacts (broadly SAT Levels 1+2+3).

This paper is a direct follow-up to Tatasciore et al. (2023; see [[tatasciore-concurrent-tasks-transparency]]), which examined concurrent task demands rather than time pressure as the stressor. Both studies used near-identical UV tasks and methods, enabling direct comparison of two different cognitive load manipulation strategies.

---

## Key Findings

- **Time pressure reduced accuracy of automation use**: Hit rates (0.90 low vs. 0.87 high TP, p<.001), correct rejection rates (0.81 low vs. 0.71 high TP, p<.001), and sensitivity d' (2.30 low vs. 1.81 high TP, p<.001, η²=.44) were all significantly poorer under high time pressure. [Domain: defence/unmanned vehicle control simulation]
- **High time pressure increased perceived workload** (4.17 low vs. 4.53 high, p<.001, η²=.31). [Domain: defence/unmanned vehicle control simulation]
- **High transparency improved accuracy of automation use**: Sensitivity d' was significantly better with high (M=2.19) vs. low (M=1.93) transparency (p=.02, η²=.09). [Domain: defence/unmanned vehicle control simulation]
- **High transparency increased automation bias**: Participants were more biased toward agreeing with the Recommender under high (c=−0.40) compared to low (c=−0.21) transparency (p<.001, η²=.32), indicating a risk of over-reliance. [Domain: defence/unmanned vehicle control simulation]
- **High transparency did not mitigate time pressure effects**: No significant interaction between transparency and time pressure on sensitivity, correct rejection rates, or workload. With both low and high transparency, accuracy dropped equally under high time pressure. [Domain: defence/unmanned vehicle control simulation]
- **High transparency increased perceived trust** (2.79 vs. 2.42, p<.001, d=0.45) and **usability** (62.77 vs. 57.50, p=.03, d=0.32). [Domain: defence/unmanned vehicle control simulation]
- **High transparency had no effect on perceived workload** (no main effect, F<1 for transparency main effect). [Domain: defence/unmanned vehicle control simulation]
- Authors interpret the null interaction as evidence that time pressure reduces the quality of information processing regardless of how much transparency information is available — users cannot efficiently use high-transparency information when cognitively constrained by time. This converges with Tatasciore et al. (2023)'s finding that concurrent task demands similarly did not interact with transparency.

---

## Transparency Constructs

The paper operationalizes **[[process-transparency]]** — specifically, the SAT model's multi-level transparency framework covering the automation's goals (Level 1), its reasoning process (Level 2), and projected outcomes plus uncertainty (Level 3). High transparency provides detailed, visual, interactive information about how the Recommender calculated its recommendation, making the system's internal process legible to the operator. This is an operationalization closer to [[traceability]] (showing calculation steps with environmental factors) than to natural language or post-hoc explanation approaches.

The paper also implicitly addresses **[[uncertainty-visualization]]** at SAT Level 3, though the current study's high transparency display focused more on calculation transparency than uncertainty quantification per se.

---

## Trust Constructs

- **[[cognitive-trust]]**: Measured using a 6-item questionnaire adapted from Merritt (2011), capturing perceived dependability and competence of the Recommender. Higher with high transparency.
- **[[behavioural-trust]]** / **[[appropriate-reliance]]**: The primary outcome is operational — accuracy of automation use (hit rate, correct rejection rate, sensitivity d') and bias (criterion c). High transparency increased both correct use and automation bias (inappropriate over-reliance), illustrating [[trust-calibration]] challenges.
- **[[algorithm-aversion]]**: Not directly observed; participants accepted automated advice at relatively high rates, and transparency increased rather than decreased reliance.

---

## Relevance to Research Questions

**RQ1**: Contributes an operationalization of [[process-transparency]] derived from the SAT model within a human-automation teaming context (defence/UV domain). Trust is measured both subjectively (Merritt 2011 scale) and behaviorally (signal detection outcomes). This is a tightly controlled, behaviorally grounded operationalization complementing subjective-measure studies.

**RQ2**: Central contribution. The study finds a **main effect of transparency on accuracy** (positive) and **no interaction with time pressure** (null moderation). This is an important conditional null finding: transparency helps in normal conditions but does not rescue performance under time pressure. Additionally, the finding that high transparency increases both accuracy and automation bias simultaneously illustrates a non-monotonic or dual-directional effect. The pattern replicates the concurrent-task null interaction from Tatasciore et al. (2023). Relevant to [[rq2-relationships]] on boundary conditions and conditional effects.

**RQ3**: Limited direct relevance. All participants were undergraduate novices; the authors explicitly note this as a limitation and call for replication with expert UV operators. The effect of operator expertise on transparency benefits is an open question. Relevant to [[user-expertise]] as a gap.

---

## Related pages

- [[process-transparency]]
- [[traceability]]
- [[appropriate-reliance]]
- [[trust-calibration]]
- [[behavioural-trust]]
- [[tatasciore-concurrent-tasks-transparency]]
- [[rq2-relationships]]
