# Conati 2021 — Methods

**Summary**: A between-subjects experiment (N = 47 who received hints) examining whether multi-level "why/how" explanations of an intelligent tutoring system's adaptive hints improve student trust, perceived usefulness, and learning, with user characteristics as moderators.

**Sources**: Conati et al._Toward personalized XAI.pdf

**Research questions addressed**: RQ1 / RQ2 / RQ3

**Last updated**: 2026-04-19

---

## Study design
experimental (between-subjects)

## Sample
- N: 47 (students who received adaptive hints; 30 in explanation condition, 17 in control)
- Population: students (undergraduate or graduate level, studying computer science / constraint satisfaction)
- Domain: education / intelligent tutoring systems
- Country / region: not reported
- Recruitment method: convenience (participants recruited through a university course or lab; not reported)

## Transparency operationalization
- Type: explainability / process transparency — multi-level "why" and "how" explanations of pedagogical AI decisions
- Manipulation or measure: Between-subjects manipulation — explanation condition had access to a six-page explanation interface (WhyHint, WhyLow, WhyRules, HowScore, HowHint, HowRank) explaining why hints were delivered and how scores and hint rankings were computed; control condition received no explanations. Interaction logs and eye tracking recorded explanation access patterns.
- Scale / instrument name: not applicable (system-level intervention)
- Number of items: not applicable

## Trust operationalization
- Type: cognitive (self-report) and behavioural (intention to use)
- Measure: (1) "I trust the system to deliver appropriate hints" — item H8 from the Perception of Hints Questionnaire (adapted from USE questionnaire and XAI literature); (2) Intention to use hints again (item H1); (3) Perceived helpfulness (item H3); (4) Actual explanation access patterns from interaction logs and eye tracking.
- Scale / instrument name: Perception of Hints Questionnaire (adapted from USE questionnaire)
- Number of items: not reported (individual items cited)
- Behavioural vs self-report: both used

## Moderators and covariates tested
- Need for Cognition (N4C): measured via validated scale; significantly predicted time spent on explanations (high N4C → more engagement) — relevant to RQ3
- Conscientiousness (Big-5): measured; significantly moderated effect of explanations on learning gain (low Conscientiousness benefited more from explanations) — relevant to RQ3
- Reading Proficiency: measured; significantly moderated effect on hint confusion (high proficiency → less confusion with explanations; low proficiency → more confusion) — relevant to RQ3
- Perceptual Speed: measured as individual difference covariate
- Visual Working Memory: measured as individual difference covariate
- Curiosity (two dimensions): measured as individual difference covariates; may relate to affective engagement

## Statistical approach
- Primary analysis method: Wilcoxon-Mann-Whitney tests (between-group trust/usability comparisons); ANOVA for moderator interactions (Conscientiousness × explanation condition); chi-square for reading proficiency moderation
- Software: not reported
- Key model fit or effect size reported: effect size r reported (e.g., r = .41 for trust, r = .49 for helpfulness); partial η² for ANOVA (e.g., η² = .11 for Conscientiousness interaction, η² = .28 for N4C and explanation access); F and p values reported

## Author-noted limitations
- Small sample size (N = 47 hint recipients; only 30 in explanation condition, 24 of whom accessed at least one explanation) limits statistical power
- Single domain (constraint satisfaction problem / CS education); generalisability across subjects and age groups unknown
- Confound between explanation access and willingness to engage: 6 students in explanation condition never accessed explanations
- Explanation design may not be optimal; completeness was partially sacrificed to avoid cognitive overload
- No control for time-on-task differences between conditions; explanation access took additional time
- Eye tracking data limited to a subset of participants

## Related pages
- [[conati-personalized-xai-education]]
- [[explainability]]
- [[process-transparency]]
- [[cognitive-trust]]
- [[behavioural-trust]]
- [[user-expertise]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]
- [[rq3-user-roles]]
