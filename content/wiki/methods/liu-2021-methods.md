# Liu 2021 — Methods

**Summary**: A 2 × 3 × 2 between-subjects online experiment (N = 491) examining how agency locus (human-programmed vs. machine-learned AI) and transparency level (none / placebic / real) affect social presence, uncertainty, and three dimensions of trust across two AI decision tasks.

**Sources**: Liu 2021_In AI we trust_.pdf

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-19

---

## Study design
experimental

## Sample
- N: 491
- Population: general US adult public (quota-sampled to approximate Census demographics); mean age 46.8
- Domain: general AI decision-making (fake news detection; personality assessment)
- Country / region: United States
- Recruitment method: Qualtrics panel (online, quota sampling)

## Transparency operationalization
- Type: process transparency and outcome transparency — provision of rationales for AI decisions
- Manipulation or measure: three-level between-subjects manipulation: (1) no transparency — no explanation provided; (2) placebic transparency — tautological, non-informative explanation mirroring the decision output (e.g., "this news is fake because it is not real"); (3) real transparency — substantive, informative explanation referencing evidence or reasoning (e.g., "this news is fake because its contents contradict other verified sources"); two AI tasks used (fake news detection; personality assessment) to enhance external validity
- Scale / instrument name: not applicable (experimental manipulation)
- Number of items: not applicable

## Trust operationalization
- Type: cognitive (trust in judgements, trust in system) and behavioural (use intention)
- Measure: three separate trust constructs assessed: (1) trust in judgements — confidence in the correctness of specific AI outputs (9-item scale adapted from Lee & See, 2004); (2) trust in system — perceived competence and credibility (12-item McCroskey & Teven, 1999 scale); (3) use intention — behavioural intention to adopt the system (4-item scale); uncertainty measured separately as mediator (6-item Clatterbuck, 1979 scale)
- Scale / instrument name: Lee & See (2004); McCroskey & Teven (1999); Clatterbuck (1979) uncertainty scale
- Number of items: 9 (trust in judgements), 12 (trust in system), 4 (use intention), 6 (uncertainty)
- Behavioural vs self-report: self-report for all trust and uncertainty measures; use intention is self-reported behavioural intention

## Moderators and covariates tested
- Agency locus (human-made rules vs. machine-learned rules): manipulated between-subjects; tested as moderator of transparency effects on uncertainty and trust — relevant to RQ2
- Task type (fake news vs. personality assessment): included to test external validity across two AI decision domains; not a focal moderator
- User expertise / AI literacy: not manipulated or measured; the paper notes machine-agency AI users processed explanations more carefully due to higher uncertainty, implying motivational differences adjacent to expertise — relevant to RQ3 implicitly

## Statistical approach
- Primary analysis method: OLS regression with moderated mediation; Hayes PROCESS macro for indirect effects
- Software: not reported
- Key model fit or effect size reported: Cohen's d = −0.20 (agency locus on social presence); Cohen's d = −0.64 (real transparency on uncertainty); ΔR² = 0.01, F = 9.30, p = 0.002 (placebic transparency × agency locus interaction on trust in judgements)

## Author-noted limitations
- User AI literacy and domain expertise not measured; depth of information processing may vary with these characteristics
- Two specific task domains (fake news, personality assessment) may not generalise to other AI decision contexts
- Online experiment limits ecological validity relative to real AI system use
- Placebic transparency manipulation targeted one specific tautological form; other non-informative explanation types may behave differently
- Social presence as a mediator is inferred from self-report and has not been validated against behavioral measures

## Related pages
- [[liu-in-ai-we-trust]]
- [[algorithmic-transparency]]
- [[process-transparency]]
- [[cognitive-trust]]
- [[algorithmic-trust]]
- [[behavioural-trust]]
- [[trust-calibration]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]
