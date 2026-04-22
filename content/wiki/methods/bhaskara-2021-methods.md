# Bhaskara et al. (2021) — Methods

**Summary**: Between-subjects online experiment (N = 176 undergraduate students) manipulating three levels of automation transparency (SAT model: Level 1, Level 1+2, Level 1+2+3) in a simulated unmanned vehicle mission-assignment task to test effects on automation use accuracy, trust, workload, and usability.

**Sources**: Bhaskara et al._Effect of automation tranparency in the management of multiple unmanned vehicles.pdf

**Research questions addressed**: RQ1 / RQ2 / RQ3

**Last updated**: 2026-04-19

---

## Study design
experimental (between-subjects online controlled experiment)

## Sample
- N: 176
- Population: undergraduate students (novice; no prior unmanned vehicle operation experience implied)
- Domain: defense / autonomous systems (simulated unmanned vehicle surveillance and rescue mission assignment)
- Country / region: not reported
- Recruitment method: convenience (undergraduate student sample)

## Transparency operationalization
- Type: automation transparency (three levels of the Situation Awareness-based Agent Transparency model — SAT model)
- Manipulation or measure: between-subjects manipulation of transparency level — (1) Level 1 (process transparency / intent disclosure): communicates what the automation is trying to achieve and mission attribute weightings; (2) Level 1+2 (algorithmic transparency / rationale): adds mathematical formulae underlying the Recommender's calculations of UV capability scores; (3) Level 1+2+3 (outcome transparency / projection visualization): adds a bar-chart visualization of projected relative performance of the two candidate unmanned vehicles on each weighted mission attribute. Automation reliability was set at 75% (Plan A was optimal on 75% of trials).
- Scale / instrument name: SAT model (Chen et al., 2014)
- Number of items: not applicable (experimental manipulation via interface design)

## Trust operationalization
- Type: cognitive (self-reported trust in automation; competence-based)
- Measure: self-reported trust in the automated recommender assessed with a modified six-item Merritt (2011) scale (5-point Likert) capturing perceived competence and overall trust; behavioral trust operationalized via signal detection metrics (hit rate, correct rejection rate, d') and decision time as objective automation use accuracy measures
- Scale / instrument name: Merritt (2011) trust in automation scale (modified, 6 items)
- Number of items: 6
- Behavioural vs self-report: both (signal detection d', hit rate, correct rejection rate, decision time as behavioral; Merritt scale as self-report)

## Moderators and covariates tested
- Transparency level (Level 1 vs. Level 1+2 vs. Level 1+2+3): primary between-subjects manipulation; non-linear (inverted-U) effect on accuracy — Level 1+2 best, Level 1+2+3 induced automation bias
- Note: user expertise was NOT included as an independent variable — all participants were undergraduate novices. The authors acknowledge this as a limitation and call for future research with expert unmanned vehicle operators (relevant to RQ3).

## Statistical approach
- Primary analysis method: ANOVA (between-subjects) for primary outcome variables (d', hit rate, correct rejection rate, decision time, NASA-TLX, trust, SUS); pairwise comparisons where significant main effects found
- Software: not reported
- Key model fit or effect size reported: p-values reported for significant effects (e.g., d' difference Level 1 vs. Level 1+2 significant; Level 1+2+3 vs. Level 1+2 significant); specific effect sizes (η², Cohen's d) not reported in source summary

## Author-noted limitations
- Sample consisted exclusively of undergraduate novices; expert unmanned vehicle operators may respond differently to transparency levels
- Time-pressure conditions in the experiment may have constrained deliberative processing in ways that differ from real-world settings
- No environmental uncertainty was present in the task (Level 3 uncertainty visualization not included); findings may not generalize to tasks with explicit uncertainty displays
- The study's task was simulated and lacked the emotional and operational stakes of real defense contexts
- Automation bias at Level 1+2+3 may partly reflect a framing effect from the projected outcome visualization rather than a general transparency ceiling effect

## Related pages
- [[bhaskara-automation-transparency-uav]]
- [[algorithmic-transparency]]
- [[process-transparency]]
- [[outcome-transparency]]
- [[trust-calibration]]
- [[appropriate-reliance]]
- [[rq2-relationships]]

## References
Bhaskara, A., et al. (2021). *Effect of automation transparency in the management of multiple unmanned vehicles*. [Journal not reported in source summary.]

Chen, J. Y. C., et al. (2014). Agent transparency: What agents communicate and agent-human team performance. *Proceedings of the Human Factors and Ergonomics Society Annual Meeting.*

Merritt, S. M. (2011). Affective processes in human-automation interactions. *Human Factors, 53*(4), 356–370.

Lee, J. D., & See, K. A. (2004). Trust in automation: Designing for appropriate reliance. *Human Factors, 46*(1), 50–80.
