# Uncertainty Visualization

**Summary**: Uncertainty visualization communicates an AI system's confidence or prediction uncertainty to users through graphical displays; effects on trust are temporally dynamic, domain-dependent, and can paradoxically increase overreliance when cognitive load is high.

**Sources**: Jansen et al._Longitudinal effects of visualizing uncertainty of situation detection.pdf; Jansen et al._Visualizing imperfect situation detection and prediction.pdf; Bhaskara et al._Effect of automation tranparency in the management of multiple unmanned vehicles.pdf; Tatasciore et al._Do concurrent task demands impact the benefit of automation transparency.pdf; Tatasciore & Loft_Can increased automation transparency mitigate the effects of time pressure on automation use_.pdf

**Research questions addressed**: RQ1, RQ2

**Last updated**: 2026-04-18

---

## Definition

Uncertainty visualization refers to graphical or numerical displays that communicate how confident an AI system is in its output. Common formats include:
- **Confidence percentages or scores** displayed alongside predictions
- **Semantic segmentation overlays** showing object detection certainty in autonomous systems
- **Pedestrian intention prediction icons** in autonomous vehicle contexts
- **Probability distributions** or error bars
- **Reliability indicators** in automation panels

This construct overlaps with [[process-transparency]] (showing how the system processes information) and [[explainability]] (justifying specific decisions), but focuses specifically on the representation of system *uncertainty* rather than *reasoning*.

## Key Findings

### Temporal Dynamics

- Longitudinal exposure (3 days, 6 sessions) to uncertainty visualizations in autonomous vehicles significantly increases perceived safety (p < 0.001) and trust over time, but effects are not immediate — they develop through familiarity (domain: autonomous vehicles; Jansen et al., 2025).
- Inconsistencies in pedestrian detection and prediction produce mixed user reactions; visualization stability is as important as information richness (domain: autonomous vehicles; Jansen et al., 2025).
- Mental workload remained stable over the 3-day longitudinal study despite added visualization complexity — suggesting users adapt to uncertainty displays without cognitive overload (domain: autonomous vehicles; Jansen et al., 2025).

### Non-linear Effects with Automation Transparency Levels

The Situational Awareness Transparency (SAT) model distinguishes three levels:
- **Level 1** (what the automation perceives)
- **Level 2** (what the automation will do based on current understanding)
- **Level 3** (what the automation projects will happen)

In unmanned vehicle management tasks:
- Level 1+2 transparency significantly improved reliance accuracy compared to no transparency
- Level 1+2+3 (adding projected outcomes) *degraded* reliance accuracy, inducing automation bias — a clear non-linear effect (domain: defense/unmanned vehicles; Bhaskara et al., 2021)

### Cognitive Load Moderates Uncertainty Visualization Benefits

- High transparency improved accuracy and trust under single-task conditions, but under concurrent cognitive demands induced automation bias rather than accurate discrimination (domain: unmanned vehicles; Tatasciore et al., 2023).
- Time pressure (12s vs. 25s windows) independently degraded performance, and high transparency did not buffer this effect — additive degradation without interaction (domain: unmanned vehicles; Tatasciore & Loft, 2024).

## Design Implications

Uncertainty displays must account for:
1. **Information load**: More uncertainty information is not always better — there is an optimal level
2. **Temporal adaptation**: Users need time to integrate uncertainty visualizations into their mental models
3. **Cognitive context**: Benefits of uncertainty displays disappear or reverse under high load

## Related pages

- [[explainability]]
- [[process-transparency]]
- [[algorithmic-transparency]]
- [[trust-calibration]]
- [[appropriate-reliance]]
- [[domain-context]]
- [[rq2-relationships]]

## References

Bhaskara, A., Skinner, M., & Loft, S. (2021). Effect of automation transparency in the management of multiple unmanned vehicles. *Human Factors*, 63(2), 173–189 [details TBD].

Jansen, R., Heesen, F., Diermeyer, F., & Bengler, K. (2025). Longitudinal effects of visualizing uncertainty of situation detection in automated driving on trust, perceived safety, and mental workload. *Transportation Research Part F* [details TBD].

Tatasciore, M., & Loft, S. (2024). Can increased automation transparency mitigate the effects of time pressure on automation use? *Applied Ergonomics*, 114, 104142.

Tatasciore, M., Bowden, V., & Loft, S. (2023). Do concurrent task demands impact the benefit of automation transparency? *Applied Ergonomics*, 110, 104022.
