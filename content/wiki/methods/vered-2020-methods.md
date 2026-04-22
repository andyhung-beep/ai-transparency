# Vered 2020 — Methods

**Summary**: A between-subjects controlled experiment (N = 30) in a complex military multi-vehicle simulation comparing Demand-Driven Transparency (DDT) versus Sequential Transparency (ST) for AI agent explanation access, finding that DDT significantly increased perceived trust and reduced task completion time.

**Sources**: Vered et al._Demand-Driven_Transparency_for_Monitoring_Intelligent_Agents.pdf

**Research questions addressed**: RQ1 / RQ2 / RQ3

**Last updated**: 2026-04-19

---

## Study design
experimental (between-subjects)

## Sample
- N: 30
- Population: students (non-domain-expert participants; explicitly noted as a limitation by authors)
- Domain: military / defense simulation (multi-unmanned vehicle management)
- Country / region: not reported
- Recruitment method: convenience (student participants)

## Transparency operationalization
- Type: process transparency / algorithmic transparency (multi-level hierarchical explanation access)
- Manipulation or measure: Two between-subjects conditions: (1) Sequential Transparency (ST) — operators view all four ETM levels in a fixed order before deciding; (2) Demand-Driven Transparency (DDT) — operators choose which of the four Endsley-based Transparency Model (ETM) levels to view and in what order. ETM levels: Level 0 (no knowledge), Level 1 (perceived input), Level 2 (input reasoning), Level 3 (plan projection).
- Scale / instrument name: not applicable (between-subjects manipulation using the Endsley-based Transparency Model)
- Number of items: not applicable

## Trust operationalization
- Type: cognitive (self-report)
- Measure: 12-item Jian, Bisantz, and Drury (2000) Trust in Automation scale, administered post-experiment; mean DDT trust = 4.04 on a 7-point scale
- Scale / instrument name: Jian, Bisantz, and Drury (2000) Trust Between People and Automation scale
- Number of items: 12
- Behavioural vs self-report: both — self-report trust questionnaire plus behavioural proxies (plan acceptance/rejection rate, hard-constraint violation detection rate)

## Moderators and covariates tested
- User expertise / domain knowledge: not formally measured as a moderator; authors explicitly note that student participants lack real-world expertise and that replication with domain experts is needed (relevant to RQ3)
- Task difficulty (hard vs. soft constraint violations): examined descriptively; DDT participants detected more hard-constraint violations (27% vs. 0%, p = 0.03)
- Transparency level usage patterns: DDT participants' voluntary sequencing of ETM levels tracked; 80% retained the sequential order voluntarily

## Statistical approach
- Primary analysis method: independent samples t-tests (between-group comparisons on trust, task completion time, performance); chi-square tests for categorical comparisons (violation detection rates)
- Software: not reported
- Key model fit or effect size reported: p-values reported (e.g., task completion time p = 0.04; hard-constraint detection p = 0.03); mean trust scores reported; effect sizes not formally reported

## Author-noted limitations
- Student participants lack real-world domain expertise; results may not generalise to professional military operators
- Small sample size (N = 30) limits statistical power
- Single domain (military simulation); generalisability to other human-agent teaming contexts unknown
- The one DDT participant who distrusted the AI and viewed minimal explanations illustrates the risk of disuse under DDT, but N = 1 is insufficient for generalisation
- The study does not systematically examine which ETM levels were most informative or preferred
- Authors explicitly call for replication with domain experts to understand how expertise interacts with DDT versus ST

## Related pages
- [[vered-demand-driven-transparency]]
- [[process-transparency]]
- [[algorithmic-transparency]]
- [[trust-calibration]]
- [[appropriate-reliance]]
- [[user-expertise]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]
- [[rq3-user-roles]]
