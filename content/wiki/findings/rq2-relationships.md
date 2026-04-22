# RQ2: Patterns of the Transparency–Trust Relationship

**Summary**: This page synthesizes the reported effect patterns between AI transparency and user trust across 86 sources, documenting linear, non-linear, conditional, and null relationships, and identifying the boundary conditions that explain this variability.

**Sources**: All 86 source documents.

**Research questions addressed**: RQ2

**Last updated**: 2026-04-18

---

## Overview

Research Question 2 asks: *What patterns of relationships between transparency and trust have been reported, including non-linear or conditional effects?*

The dominant finding across the corpus is that simple positive linear relationships between transparency and trust are the exception rather than the rule. Conditional, non-linear, and null effects are equally or more common. This section organizes findings by effect pattern type.

---

## 1. Positive Linear Effects

The simplest pattern — more transparency produces more trust — is supported in some studies, but typically with important qualifications.

| Source | Domain | Transparency type | Trust outcome | Notes |
|---|---|---|---|---|
| Alarcon et al. | General/lab | Calibrated confidence | Behavioural reliance | Conditional on task difficulty |
| Jaziri & Sassi (2025) | Autonomous systems / clinical | Explainability-by-design | Self-reported trust (+19%) | Embedded XAI, optimised design |
| Angerschmid et al. (2022) | Healthcare | Feature importance, example-based | Trust in fairness | Conditional on actual fairness level |
| Shin (2021) | News recommendations | Causability → explainability | Algorithmic trust | Mediated via FAT perceptions |
| Jansen et al. longitudinal | Autonomous vehicles | Uncertainty visualization | Perceived safety, trust | Effect builds over 3 days |
| Weitz (2021) | General/lab | NL explanation via agent | Trust in system | Linear with agent human-likeness |
| van Zetten et al. (2022) | Finance | Local SHAP explanations | Self-reported trust | Field study; warns of over-trust risk |
| Vered et al. (2020) | Defense | Demand-driven transparency | Perceived trust | Presentation mode critical |

**Qualification**: Even in studies reporting positive linear effects, effect sizes are often modest, and the findings are typically domain-specific and constrained to particular explanation formats.

---

## 2. Conditional / Interaction Effects

The most commonly documented pattern: transparency effects on trust depend on a third variable. Effect direction or magnitude changes as a function of the moderator.

### 2a. Conditioned on AI Performance / Accuracy

- Transparency effects are larger when AI expectations are violated (positive or negative disconfirmation) than when AI performs as expected; in expectation-confirmed conditions, low transparency outperforms high transparency (domain: e-commerce; Sun et al., 2026).
- Transparency amplifies trust when AI is correct but accelerates trust erosion when AI errs — a transparency paradox (domain: healthcare; Yu et al., 2025).
- XAI methods work differently on correct vs. incorrect AI trials: counterfactual explanations reduce overreliance on wrong recommendations while feature-importance explanations reinforce it (domain: healthcare; Lee & Chew, 2023).

### 2b. Conditioned on Explanation Content / Actionability

- Actionable sensitivity explanations improve trust and fairness perceptions; non-actionable explanations *backfire* (trust *lower* than no explanation baseline) (domain: e-commerce; Mourali et al., 2025).
- Benefit-focused explanations outperform algorithmic rationale explanations for cognitive trust in recommender systems (domain: workplace teams; Musick et al., 2024).
- Real transparency (genuine information about system) reduces uncertainty and increases trust; placebic transparency (performative disclosure) increases use intention heuristically without reducing uncertainty (domain: general; Liu, 2021).

### 2c. Conditioned on Explanation Timing

- Explanations provided before an AI action increase trust and preference; after-action explanations are no better than no explanation (domain: autonomous vehicles; Du et al., 2019).

### 2d. Conditioned on Task Context / Cognitive Demands

- High transparency improves reliance accuracy under single-task conditions but induces automation bias (overreliance) under concurrent cognitive load (domain: unmanned vehicles; Tatasciore et al., 2023).
- Time pressure independently degrades performance; high transparency does not buffer this effect — additive degradation without protective interaction (domain: unmanned vehicles; Tatasciore & Loft, 2024).

### 2e. Conditioned on Decision Outcome Valence

- Explanation effects on consumer trust are significant for negative outcomes (rejected applications) but attenuated or absent for positive outcomes (domain: e-commerce; Mourali et al., 2025).

### 2f. Conditioned on Task Objectivity

- Explanations reduce algorithm aversion most for decisions based on verifiable objective criteria (domain: HR; Fleiß et al., 2024).

---

## 3. Non-Linear / Inverted-U Effects

A critical subset of findings shows that the transparency–trust relationship peaks at an intermediate level, with very high transparency producing worse outcomes than moderate transparency.

| Source | Domain | Pattern | Notes |
|---|---|---|---|
| Rezaeian et al. (2025) | Healthcare | 4-level: no-explanation > most-detailed in accuracy & trust | Enhanced localization degraded performance |
| Bhaskara et al. | Unmanned vehicles | Level 1+2 optimal; Level 3 harmful | Level 3 induced automation bias |
| Tatasciore et al. (concurrent) | Unmanned vehicles | High transparency induces bias under load | Reversal of benefit |
| Karran et al. (2022) | General/lab | Low morphological clarity produces higher confidence than high clarity | Counter-intuitive visualization finding |
| Humer et al. (2024) | General/lab | Different XAI methods: reassuring, neutral, or misleading | No method is uniformly better |
| Conijn et al. (2023) | Education | Null XAI effects; grade discrepancy dominates | Outcome quality overrides transparency |

**Theoretical interpretation**: These findings are consistent with information overload theory and cognitive fit theory — transparency information beyond the user's processing capacity or workflow alignment reduces rather than improves outcomes.

---

## 4. Null Effects

Transparency manipulations sometimes have no significant effect on trust outcomes. Null findings are under-reported but important for understanding boundary conditions.

| Source | Domain | Null finding |
|---|---|---|
| Kleizen et al. (2023) | Government | Ethical AI messaging: no significant effect on citizen trust |
| Conijn et al. (2023) | Education | Explanations and accuracy statements: no effect on student trust or motivation |
| Diprose et al. (2020) | Healthcare | Explanations: no effect on intended physician behaviour |
| Kornowicz & Thommes (2025) | General/lab | Feature-selection transparency: no effect on actual advice reliance |
| Jansen et al. 2024 | Autonomous vehicles | Uncertainty visualization: no significant trust change (replicated) |
| Cramer et al. (2008) | E-commerce | Confidence displays: no effect on trust or acceptance |
| Nelekar et al. (2021) | Education | Explanation type: no between-group differences in trust or working alliance |
| Knapic et al. (2021) | Healthcare | LIME (p=0.738), SHAP (p=0.464), CIU (p=0.158): none significantly improve lay-user decision accuracy vs. no explanation |

**Pattern**: Null effects are most common when (a) prior institutional trust or dispositional factors dominate, (b) outcome quality strongly predicts trust, (c) users cannot process the transparency information provided, or (d) the explanation type is mismatched to user capacity (Knapic et al. show SHAP's complexity may cause lay users to perform worse than with no explanation at all).

---

## 5. Negative Effects

In some conditions, more transparency reduces trust or performance.

| Source | Domain | Negative finding |
|---|---|---|
| Schilke & Reimann (2025) | Organizational | AI disclosure by humans: interpersonal trust *decreases* (robust across 13 experiments) |
| Mukhtar et al. (2023) | Software engineering | LIME visualization explanations: performance worse than no explanation |
| Papenmeier et al. | Multi-domain | Transparency revealing errors: trust drops faster than it builds |
| Humer et al. (2024) | General/lab | Feature-importance: "deceptive reassurance" for wrong AI recommendations |
| Spitzer et al. (2025) | General/lab | Incorrect explanations: Deception of Reliance metric worsens performance |

---

## 6. Temporal Dynamics

Most studies measure trust at a single point. The few longitudinal or multi-session studies show a distinct picture:

- Trust increases over repeated exposures to uncertainty visualizations over 3 days, particularly in evening sessions (domain: autonomous vehicles; Jansen et al., 2025).
- Traceability (SIPA) develops non-linearly — does not appear until approximately 45+ system interactions (domain: healthcare; Schrills & Franke, 2023).
- Trust is asymmetric over time: errors erode trust faster than successes build it (domain: healthcare; Yu et al., 2025).

---

## Cross-Cutting Mechanisms

Several papers identify *mechanisms* (mediators) that explain the transparency–trust relationship:

| Mechanism | Evidence source |
|---|---|
| Perceived understanding → trust | Shin (2021); Diprose (2020); Sun et al. (dating) |
| Legitimacy → interpersonal trust | Schilke & Reimann (2025) |
| Metacognitive calibration → delegation | von Zahn et al. (2025) |
| Positive affect → affective trust → reliance | Bernardo & Seva (2023) |
| FAT perceptions → algorithmic trust | Shin (2021) |
| Uncertainty reduction → trust | Liu (2021); Du et al. (2019) |

---

## Summary: Effect Pattern Distribution

Based on qualitative coding across the 86 sources:

| Pattern | Approximate prevalence |
|---|---|
| Positive conditional effects | ~40% |
| Positive linear effects | ~25% |
| Null effects | ~20% |
| Non-linear / inverted-U | ~10% |
| Negative effects | ~5% |

These estimates reflect main findings rather than all outcomes reported.

---

## Identified Gaps

1. **Longitudinal designs**: Only 2 studies measure trust development over multiple sessions/days (Jansen et al.; Schrills & Franke). The temporal trajectory of transparency-induced trust is largely unknown.
2. **Mechanism studies**: Few papers test mechanisms (mediators) rather than only main effects. Understanding *why* transparency affects trust is underdeveloped.
3. **Meta-analytic synthesis**: The diversity of operationalizations prevents quantitative meta-analysis. A standardization effort is needed.
4. **Interaction studies**: Most studies test one type of transparency at a time. How different transparency types combine is understudied.

---

## Related pages

- [[trust-calibration]]
- [[appropriate-reliance]]
- [[algorithm-aversion]]
- [[outcome-transparency]]
- [[domain-context]]
- [[user-expertise]]
- [[rq1-conceptualizations]]
- [[rq3-user-roles]]

## References

Du, N., Haspiel, J., Zhang, Q., Tilbury, D., Pradhan, A. K., Yang, X. J., & Robert, L. P. (2019). Look who's talking now: Implications of AV's explanations on driver's trust, AV preference, anxiety and mental workload. *Transportation Research Part C: Emerging Technologies*, 104, 428–442.

Fleiß, J., Hiebl, J., & Müller, S. (2024). Mitigating algorithm aversion in recruiting. *Journal of Business and Psychology* [details TBD].

Jansen, R., Heesen, F., Diermeyer, F., & Bengler, K. (2025). Longitudinal effects of visualizing uncertainty of situation detection in automated driving on trust, perceived safety, and mental workload. *Transportation Research Part F* [details TBD].

Lee, J., & Chew, E. (2023). Understanding the effect of counterfactual explanations on trust and reliance on AI for human-AI collaborative clinical decision making. *Proceedings of the ACM on Human-Computer Interaction* (CSCW2), 7.

Liu, P. (2021). In AI we trust? Effects of agency locus and transparency on uncertainty reduction in human–AI interaction. *Journal of Computer-Mediated Communication*, 26(6), 384–402 [details TBD].

Mourali, M., Novakowski, D., Pogacar, F., & Brigden, R. (2025). Post hoc explanations improve consumer responses to algorithmic decisions. *Journal of Business Research* [details TBD].

Musick, G., Lee, M. K., Eslami, M., & Kuo, C.-L. (2024). Recommendations with benefits: Exploring explanations in information-presentation randomized experiments. *CHI Conference on Human Factors in Computing Systems* [details TBD].

Schrills, T., & Franke, T. (2023). How do users experience traceability of AI systems? Examining subjective information processing awareness in automated insulin delivery (AID) systems. *ACM Transactions on Interactive Intelligent Systems*, 13(4).

Sun, Q., Shi, X., Zhang, T., & Liu, J. (2026). Does transparency matter when an AI system meets performance? Understanding the moderating role of performance expectation confirmation. *Computers in Human Behavior* [details TBD].

Tatasciore, M., & Loft, S. (2024). Can increased automation transparency mitigate the effects of time pressure on automation use? *Applied Ergonomics*, 114, 104142.

Tatasciore, M., Bowden, V., & Loft, S. (2023). Do concurrent task demands impact the benefit of automation transparency? *Applied Ergonomics*, 110, 104022.

Yu, K., Guo, J., Shen, Y., & Martens, H. (2025). Research and analysis of trust and control in human–AI collaboration in healthcare. *Frontiers in Psychology* [details TBD].
