# Tatasciore & Loft (2024) — Methods

**Summary**: A within-subjects experiment (N = 64 undergraduates) crossing automation transparency level (low vs. high) and time pressure (low vs. high) in a simulated uninhabited vehicle management task, finding that high transparency improved accuracy and trust but did not buffer the negative effects of time pressure on automation use performance.

**Sources**: Tatasciore, M., & Loft, S. (2024). Can increased automation transparency mitigate the effects of time pressure on automation use_.pdf

**Research questions addressed**: RQ1 / RQ2 / RQ3

**Last updated**: 2026-04-19

---

## Study design
experimental (2 × 2 fully within-subjects repeated-measures design)

## Sample
- N: 64
- Population: undergraduate students
- Domain: defence / uninhabited vehicle (UV) management simulation
- Country / region: not reported (Australian university implied by author affiliations)
- Recruitment method: convenience (university undergraduate participants)

## Transparency operationalization
- Type: process transparency — SAT (Situation-Awareness Agent-Based Transparency) model two-level manipulation
- Manipulation or measure: within-subjects manipulation of transparency level; (1) Low transparency — table display showing Recommender's capability weightings per UV (broadly SAT Level 1); (2) High transparency — low display plus additional bar graphs showing step-by-step UV score calculations including individual environmental factor contributions (broadly SAT Levels 1+2+3); automation reliability set at 80%
- Scale / instrument name: not applicable (transparency was an interface design manipulation)
- Number of items: not applicable

## Trust operationalization
- Type: cognitive trust (self-report) and behavioural trust / appropriate reliance (signal detection performance metrics)
- Measure: cognitive trust via 6-item Merritt (2011) questionnaire; behavioural trust via signal detection theory metrics — hit rate, correct rejection rate, sensitivity d', criterion c (automation bias); usability via System Usability Scale (SUS); perceived workload via NASA-TLX or similar (described as workload measure in source)
- Scale / instrument name: Merritt (2011) trust questionnaire (6 items); System Usability Scale (SUS)
- Number of items: 6 (trust); 10 (SUS)
- Behavioural vs self-report: both

## Moderators and covariates tested
- Time pressure: within-subjects manipulation — low (25 s per decision) vs. high (12 s per decision); tested as moderator of transparency effects on accuracy, workload, trust, and usability; no significant transparency × time pressure interaction found for accuracy
- Note: user expertise not examined; all participants were undergraduate novices — relevant to RQ3 as a limitation; authors explicitly call for expert operator replication

## Statistical approach
- Primary analysis method: repeated-measures ANOVA (2 × 2 within-subjects factorial design); effect sizes as partial η²; Cohen's d for trust and usability comparisons
- Software: not reported
- Key model fit or effect size reported: transparency main effect on d' p = .02, η² = .09; time pressure main effect on d' η² = .44; high transparency increased automation bias c from -0.21 to -0.40 p < .001, η² = .32; trust increase d = 0.45; usability increase d = 0.32; transparency × time pressure interaction on d' non-significant; time pressure main effect on correct rejection rate p < .001

## Author-noted limitations
- Sample consisted exclusively of undergraduate novices; findings may not generalise to experienced UV operators or professional military personnel
- Within-subjects design introduces potential order and carryover effects despite counterbalancing
- High transparency increased automation bias (over-reliance risk) alongside accuracy improvements — the net effect on operational safety is unclear
- Time pressure levels were defined by fixed durations (12 s vs. 25 s) that may not capture the range of operational stressors in real settings
- Automation reliability (80%) was fixed; varying reliability may alter how transparency affects trust calibration

## Related pages
- [[tatasciore-loft-time-pressure-transparency]]
- [[tatasciore-concurrent-tasks-transparency]]
- [[tatasciore-loft-transparency-effects]]
- [[process-transparency]]
- [[traceability]]
- [[trust-calibration]]
- [[appropriate-reliance]]
- [[behavioural-trust]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]
- [[rq3-user-roles]]

## References
Tatasciore, M., & Loft, S. (2024). Can increased automation transparency mitigate the effects of time pressure on automation use? *Applied Ergonomics*, 114, 104142. https://doi.org/10.1016/j.apergo.2023.104142

Merritt, S. M. (2011). Affective processes in human–automation interaction. *Human Factors, 53*(4), 356–370.

Chen, J. Y. C., Procci, K., Boyce, M., Wright, J., Garcia, A., & Barnes, M. (2014). *Situation awareness-based agent transparency* (ARL-TR-6905). U.S. Army Research Laboratory.
