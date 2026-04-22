# Zhang 2024 — Methods

**Summary**: A 2×2×4 mixed factorial online experiment (N = 156) using video-based game vignettes to examine when AI teammate explanations affect trust and perceived team effectiveness, finding that explanation effects are strongly conditional on the type of action explained (disobedience vs. deception) and individual characteristics (gender, ethical framework).

**Sources**: Zhang et al._I know this looks bad, but i can explain.pdf

**Research questions addressed**: RQ1 / RQ2 / RQ3

**Last updated**: 2026-04-19

---

## Study design
experimental (2×2×4 mixed factorial design; online; video-based vignette scenarios)

## Sample
- N: 156
- Population: general public (online participants; mixed gender and ethical orientation)
- Domain: human-AI teaming / simulated game environment (multiplayer online game ArmA III scenario)
- Country / region: United States (Clemson University)
- Recruitment method: not reported (online experiment)

## Transparency operationalization
- Type: explainability (action-level explanation; post-hoc, instance-specific)
- Manipulation or measure: 2×2×4 mixed factorial design crossing: (1) Teammate identity (between-subjects): human teammate vs. AI teammate; (2) Explanation (between-subjects): with explanation vs. without explanation; (3) Teammate action (within-subjects, four levels): ignoring potential death, ignoring injury, disobeying orders, lying to humans. Explanations were structured to address three elements: (a) the action taken, (b) the consequence to the human, and (c) the rationale for why the action was taken. Machine-language phrasing used to avoid over-anthropomorphizing the AI. Video vignettes set in ArmA III game scenario where a teammate performed actions that benefited the team but harmed the individual participant.
- Scale / instrument name: not applicable (between-subjects manipulation)
- Number of items: not applicable

## Trust operationalization
- Type: cognitive (self-report) and affective/behavioural intention proxy
- Measure: (1) Cognitive trust — six-item scale assessing belief that the teammate would honestly and accurately complete tasks; (2) Perceived team effectiveness — satisfaction-based scale items capturing willingness to re-team and assessment of team outcomes; Structural Equation Modelling (SEM) used to examine relationships between explanation, trust, and perceived effectiveness
- Scale / instrument name: not reported (six-item cognitive trust scale; satisfaction items for team effectiveness)
- Number of items: 6 (cognitive trust)
- Behavioural vs self-report: self-report (with behavioural intention proxy via willingness to re-team)

## Moderators and covariates tested
- Teammate identity (AI vs. human): between-subjects factor; explanations increased trust for AI disobedience but had no effect on trust for human teammate — explanations operate differently depending on agent type (relevant to RQ2)
- Gender: moderated explanation effects; non-male participants (women, non-binary) trusted AI less than men in lying (β = −0.731, p < 0.001) and ignoring potential death (β = −0.742, p < 0.001) scenarios but not in disobeying scenario (relevant to RQ3)
- Ethical framework (utilitarian vs. deontological): measured via self-report; utilitarian ethical orientation predicted higher perceived team effectiveness with AI teammates (β = 0.119, p < 0.01) — relevant to RQ3
- Action type (within-subjects): primary within-subjects factor; explanations helped trust for disobedient actions (β = 0.672, p < 0.001) but harmed trust for deceptive actions (β = −0.739, p < 0.001)
- Action directness (direct vs. indirect consequences for participant): explanations more effective for actions with direct consequences to the individual

## Statistical approach
- Primary analysis method: Structural Equation Modelling (SEM) for examining paths from explanation and action type to trust and perceived team effectiveness; mixed ANOVA for within-between interaction effects
- Software: not reported
- Key model fit or effect size reported: SEM path coefficients reported (e.g., explanation → trust for disobedience β = 0.672 p < 0.001; explanation → trust for lying β = −0.739 p < 0.001; gender → trust β = −0.731 p < 0.001); model fit indices not reported in source summary

## Author-noted limitations
- Game-based scenario (ArmA III) may not generalise to real-world human-AI teaming contexts (e.g., healthcare, autonomous vehicles, workplace)
- Trust decreases over time with AI teammates (vs. increases with humans); cross-sectional vignette design cannot fully capture longitudinal trust dynamics
- Video-based vignettes limit ecological validity; participants observe rather than actively participate
- Sample demographics and recruitment details not fully reported
- Explanation content held constant across conditions; real-world explanations vary in quality and truthfulness
- The study does not examine actual task performance outcomes, only subjective trust and effectiveness perceptions

## Related pages
- [[zhang-ai-explanations-human-ai-teams]]
- [[explainability]]
- [[cognitive-trust]]
- [[trust-calibration]]
- [[algorithmic-trust]]
- [[appropriate-reliance]]
- [[user-expertise]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]
- [[rq3-user-roles]]
