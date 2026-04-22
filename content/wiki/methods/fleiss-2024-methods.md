# Fleiß 2024 — Methods

**Summary**: A within-subject quota-representative experiment (N = 490) from Germany and Austria testing three XAI explanation types and decision objectivity (soft skills vs. verifiable qualifications) on acceptance of AI conversational agents in a recruiting context.

**Sources**: Fleiß et al._Mitigating algorithm aversion in recruiting.pdf

**Research questions addressed**: RQ1 / RQ2 / RQ3

**Last updated**: 2026-04-19

---

## Study design
experimental (within-subject design; participants exposed to multiple explanation conditions)

## Sample
- N: 490
- Population: general public (quota-representative sample matching working-age population demographics)
- Domain: human resources / recruiting
- Country / region: Germany and Austria
- Recruitment method: quota-representative online panel (not reported which panel provider)

## Transparency operationalization
- Type: explainability and algorithmic transparency — three XAI explanation types
- Manipulation or measure: Within-subject manipulation across three XAI explanation types, each presented for two decision objectivity conditions (soft skills vs. verifiable qualifications), with a baseline no-explanation control: (1) Post-hoc feature list (EXPLAIN_LIST) — names the three criteria most relevant to the rejection decision (feature attribution); (2) Post-hoc comparison visualization (EXPLAIN_COMPARE) — displays applicant scores on three criteria alongside average scores of other applicants; (3) Intrinsic model explanation (EXPLAIN_INTERPRET) — shows a simple decision tree with the path leading to rejection highlighted. All explanations provided for AI-based conversational agent (CA) decisions in applicant pre-selection.
- Scale / instrument name: not applicable (between-conditions manipulation)
- Number of items: not applicable

## Trust operationalization
- Type: cognitive (single-item within composite acceptance measure)
- Measure: Trust operationalised as a single item within the overall acceptance composite scale: "Do you trust the chatbot decision just described?" Acceptance composite also includes intention to use and fairness perception. General dispositional trust in AI measured as control variable via Jian et al. (2000) scale.
- Scale / instrument name: Jian et al. (2000) scale for dispositional trust in AI (control); researcher-designed single item for situational trust
- Number of items: not reported for Jian et al. scale; 1 item for situational trust (within composite)
- Behavioural vs self-report: self-report

## Moderators and covariates tested
- General trust in AI (dispositional): measured via Jian et al. (2000); strongest individual-level predictor of acceptance (coefficient 0.669, p < .001) — relevant to RQ3
- Affinity for technology: measured as individual difference covariate; not a significant predictor (weaker than general AI trust)
- Age: measured; small negative effect on acceptance — relevant to RQ3
- Decision objectivity (soft skills vs. verifiable qualifications): manipulated within-subject; significantly moderated explanation effectiveness — verifiable qualifications produced higher acceptance across all explanation types

## Statistical approach
- Primary analysis method: multilevel / mixed-effects regression (within-subject design with repeated measures; specific method not detailed in source summary); pairwise comparisons for explanation type effects
- Software: not reported
- Key model fit or effect size reported: coefficient for general trust in AI = 0.669, p < .001; all XAI conditions vs. no-explanation p < .001; no significant differences between explanation types; specific test statistics not reported in source summary

## Author-noted limitations
- Within-subject design may introduce demand characteristics or response fatigue across multiple vignettes
- Sample limited to Germany and Austria; cultural generalisability uncertain
- First-encounter paradigm; long-term algorithm aversion or trust calibration not assessed
- Intrinsic decision tree explanation may be more complex than realistic applicants would encounter in practice
- Trust measured as single item within composite; lacks psychometric depth
- Does not examine individual cognitive styles (e.g., Need for Cognition) as moderators

## Related pages
- [[fleiss-algorithm-aversion-recruiting]]
- [[algorithm-aversion]]
- [[algorithmic-transparency]]
- [[explainability]]
- [[behavioural-trust]]
- [[cognitive-trust]]
- [[user-expertise]]
- [[domain-context]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]
