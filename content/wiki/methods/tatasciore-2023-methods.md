# Tatasciore et al. (2023) — Methods

**Summary**: A mixed between-subjects (three transparency levels) and within-subjects (concurrent task presence/absence) experiment with 212 undergraduate participants using a simulated uninhabited vehicle (UV) management task, finding that high transparency improved automation use accuracy under both single- and dual-task conditions but also increased automation bias under concurrent task demands.

**Sources**: Tatasciore et al._Do concurrent task demands impact the benefit of automation transparency.pdf

**Research questions addressed**: RQ1 / RQ2 / RQ3

**Last updated**: 2026-04-19

---

## Study design
experimental (mixed between-subjects × within-subjects design)

## Sample
- N: 212
- Population: undergraduate students
- Domain: defence / uninhabited vehicle (UV) management simulation
- Country / region: not reported (Australian university implied by author affiliations)
- Recruitment method: convenience (university undergraduate participants)

## Transparency operationalization
- Type: process transparency — SAT (Situation-Awareness Agent-Based Transparency) model three-level framework
- Manipulation or measure: between-subjects manipulation of transparency level; (1) Low transparency — table showing Recommender's capability weightings for each UV (SAT Level 1: goal/intent); (2) Medium transparency — low display plus bar graphs showing calculated UV scores after environmental factors (SAT Level 2: reasoning); (3) High transparency — medium display plus detailed bar graphs showing step-by-step score calculation including individual environmental factor contributions (SAT Level 3: projection/outcome); automation reliability set at 80%
- Scale / instrument name: not applicable (transparency was an interface design manipulation)
- Number of items: not applicable

## Trust operationalization
- Type: cognitive trust (self-report) and behavioural trust / appropriate reliance (signal detection performance metrics)
- Measure: cognitive trust via 6-item Merritt (2011) questionnaire (α = 0.87–0.92 across conditions); behavioural trust via signal detection theory metrics — hit rate, correct rejection rate, sensitivity d', criterion c (automation bias); decision response time; concurrent task performance (false alarm rate on image analysis task)
- Scale / instrument name: Merritt (2011) trust questionnaire (6 items); usability not separately reported in summary
- Number of items: 6 (trust)
- Behavioural vs self-report: both

## Moderators and covariates tested
- Concurrent task demands: within-subjects manipulation — UV task performed alone vs. simultaneously with an image-analysis change-detection task emulating real multi-task UV operator workload; tested as moderator of transparency effects on accuracy, trust, and decision speed
- Note: user expertise not examined; all participants were undergraduate novices — relevant to RQ3 as a limitation and gap for expert replication

## Statistical approach
- Primary analysis method: mixed-model ANOVA (between: transparency level; within: concurrent task presence/absence); signal detection theory metrics (d', c) as primary outcome variables; post-hoc pairwise comparisons
- Software: not reported
- Key model fit or effect size reported: concurrent task effect on d': p = .002, η² = .05; concurrent task effect on workload η² = .39; high vs. low transparency under concurrent task on trust p = .004, d = 0.49; on decision time p = .01, d = 0.46; on bias c p = .01, d = 0.45; false alarms on image analysis task high vs. medium transparency p = .002, d = 0.55; no transparency × concurrent task interaction for overall sensitivity (F < 1)

## Author-noted limitations
- Sample consisted exclusively of undergraduate novices; expert operator replication is explicitly identified as needed
- The concurrent image-analysis task was designed to simulate dual-task operator workloads but may not fully capture real-world UV operator complexity
- Medium transparency showed an unexpected pattern of inferior performance relative to high transparency under concurrent demands, raising questions about intermediate information complexity effects
- Automation reliability was fixed at 80%; varying reliability levels may alter the transparency–reliance relationship
- Within-subjects component introduces potential carryover effects between concurrent-task-absent and concurrent-task-present trials

## Related pages
- [[tatasciore-concurrent-tasks-transparency]]
- [[tatasciore-loft-time-pressure-transparency]]
- [[process-transparency]]
- [[traceability]]
- [[trust-calibration]]
- [[appropriate-reliance]]
- [[behavioural-trust]]
- [[algorithm-aversion]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]
- [[rq3-user-roles]]

## References
Tatasciore, M., Bowden, V., & Loft, S. (2023). Do concurrent task demands impact the benefit of automation transparency? *Applied Ergonomics*, 110, 104022. https://doi.org/10.1016/j.apergo.2023.104022

Merritt, S. M. (2011). Affective processes in human–automation interaction. *Human Factors, 53*(4), 356–370.

Chen, J. Y. C., Procci, K., Boyce, M., Wright, J., Garcia, A., & Barnes, M. (2014). *Situation awareness-based agent transparency* (ARL-TR-6905). U.S. Army Research Laboratory.
