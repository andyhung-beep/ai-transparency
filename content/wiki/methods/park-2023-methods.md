# Park 2023 — Methods

**Summary**: A two-phase mixed-methods study developing and validating a 9-factor AI UX questionnaire (N = 105 AI speaker users) and applying it in a pre-post usability test (N = 20) to evaluate interface upgrades to a military AI defense system.

**Sources**: Park et al._Designing_and_Evaluating_User_Experience_of_an_AI-Based_Defense_System.pdf

**Research questions addressed**: RQ1 / RQ2 / RQ3

**Last updated**: 2026-04-19

---

## Study design
mixed-methods (survey-based scale development + quasi-experimental pre-post usability test)

## Sample
- N: 105 (Phase 1 — questionnaire validation with AI speaker users); 20 (Phase 2 — usability test of defense system)
- Population: Phase 1 — general AI speaker users; Phase 2 — non-expert participants (deliberately recruited to minimize prior defense knowledge)
- Domain: Phase 1 — general AI / smart speakers; Phase 2 — national defense / military surveillance (South Korea)
- Country / region: South Korea
- Recruitment method: not reported (convenience for Phase 2)

## Transparency operationalization
- Type: explainability and causality as distinct UX dimensions; measured as self-report questionnaire factors
- Manipulation or measure: Phase 2 uses a pre-post design comparing the original AI defense system UI against an upgraded UI. Transparency-related upgrades included: (a) help functions and tutorials explaining system operation; (b) additional data panels displaying bases for change-detection and target-detection judgments; (c) disabled-state representations clarifying unavailable functions; (d) colour coding for cross-modality unity. Transparency outcomes measured via the validated AI UX questionnaire subscales for explainability and causality.
- Scale / instrument name: AI UX Questionnaire (developed by authors in Phase 1; 9 factors); individual subscales for explainability and causality
- Number of items: not reported per subscale (total questionnaire item count not reported)

## Trust operationalization
- Type: cognitive (self-reported confidence and willingness to rely)
- Measure: Trust subscale of the AI UX Questionnaire; scored on a 0–10 scale. Phase 2 compares pre-upgrade (M = 5.42) vs. post-upgrade (M = 7.90) trust scores.
- Scale / instrument name: Trust subscale of the AI UX Questionnaire (authors' own instrument); internal consistency α = 0.925
- Number of items: not reported
- Behavioural vs self-report: self-report

## Moderators and covariates tested
- Gender: noted in referenced literature (Reeder et al., 2023) as moderating XAI comprehension; not systematically tested in this study
- Educational background: cited from prior work as a moderator; not tested here
- AI user expertise: Phase 2 participants were non-experts by design; subgroup analyses by expertise not conducted (relevant to RQ3 as a noted gap)

## Statistical approach
- Primary analysis method: Phase 1 — exploratory factor analysis (EFA) and confirmatory factor analysis (CFA); Phase 2 — Wilcoxon signed-rank tests or paired comparisons for pre-post differences
- Software: not reported
- Key model fit or effect size reported: CFI = 0.961, RMSEA = 0.057 (Phase 1 CFA); Cronbach's α per subscale (trust α = 0.925, satisfaction α = 0.923, safety α = 0.918); pre-post mean differences with significance reported per subscale

## Author-noted limitations
- Phase 2 usability test is small (N = 20) and limited to non-expert participants in a single domain (military defense)
- The AI UX questionnaire was validated on AI speaker users (Phase 1) but applied to a defense system (Phase 2); domain transferability not established
- Gender and educational diversity of participant samples may limit generalisability
- Single-site study conducted in South Korea; cultural factors may affect results
- Fairness subscale did not improve, attributed to domain specifics — alternative explanations not ruled out

## Related pages
- [[park-ai-ux-defense-system]]
- [[explainability]]
- [[causability]]
- [[cognitive-trust]]
- [[trust-calibration]]
- [[user-expertise]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]
