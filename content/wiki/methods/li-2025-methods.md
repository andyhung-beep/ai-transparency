# Li 2025 — Methods

**Summary**: A four-phase between-subjects experiment with 60 human graders (56 completers) recruited via Prolific comparing no AI support, important-word highlights (XAI), and GenAI natural-language grading explanations (GPT-4) on feedback quality, grading accuracy, and perceived usefulness in educational assessment.

**Sources**: Li et al._When AI explains in natural language.pdf

**Research questions addressed**: RQ1 / RQ2 / RQ3

**Last updated**: 2026-04-19

---

## Study design
experimental (between-subjects; four-phase longitudinal design)

## Sample
- N: 60 recruited; 56 completed all phases
- Population: experienced educators (K-12 and secondary school teachers with teaching experience in relevant subjects)
- Domain: educational assessment (secondary students' short-answer grading — English comprehension/summarisation Q9 and science reasoning Q10 from ASAP-SAS KAGGLE dataset)
- Country / region: not reported
- Recruitment method: Prolific

## Transparency operationalization
- Type: (G2) feature-attribution explanation (important-word highlights); (G3) natural-language explanation (chain-of-thought reasoning)
- Manipulation or measure: three-group between-subjects manipulation across four phases (Pre-Training → Pre-Eval → Exp-1 → Exp-2; Exp-2 one week after Exp-1 with no AI support to measure transfer): (G1) no AI support; (G2) important-word highlights derived via integrated-gradients XAI applied to BERT-based automatic grader; (G3) chain-of-thought natural-language explanations from GPT-4 grader describing assessment rationale step-by-step; Exp-1 used only correctly-graded answers to control for AI error exposure
- Scale / instrument name: not applicable
- Number of items: not applicable

## Trust operationalization
- Type: behavioural (adoption intent); cognitive (perceived usefulness, comprehensibility)
- Measure: trust is not formally measured with a validated psychometric scale; trust-adjacent constructs assessed via survey items: willingness to grade/compile feedback with AI-powered insights (adoption intent, 4-item questionnaire); perceived informativeness, usefulness, comprehensibility, and efficiency-enhancement of AI insights (Likert scale comparisons between G2 and G3); objective behavioural outcomes: grading correctness and learner-centred feedback quality (agency, sense-making, learning impact dimensions)
- Scale / instrument name: not reported (custom survey items)
- Number of items: 4 (adoption intent questionnaire); not reported (perceived usefulness items)
- Behavioural vs self-report: both (objective grading correctness and feedback quality as behavioural outcomes; survey items for adoption intent and perceived usefulness)

## Moderators and covariates tested
- Question type (Q9 English comprehension vs. Q10 Science reasoning): used as a covariate in multilevel models; no significant interaction with condition reported
- Phase (Exp-1 vs. Exp-2): temporal moderator — transfer effects at one week showed non-significant trends toward better feedback quality for G2 and G3; G2 grading duration increased significantly in Exp-2 (suggesting highlights slowed autonomous workflow)
- Task difficulty / ceiling effect: noted — grading tasks relatively easy for experienced educators, limiting ceiling for accuracy improvement
- User expertise level within educator sample: not varied — all participants are experienced educators; novice–expert comparison not included (relevant to RQ3 as a gap)

## Statistical approach
- Primary analysis method: multilevel linear regression (feedback quality and grading accuracy as DVs; condition, phase, question as predictors); Mann-Whitney U test (between-group perceived usefulness comparisons G2 vs. G3)
- Software: not reported
- Key model fit or effect size reported: G3 feedback quality β = 0.190, p = 0.010; G2 feedback quality β = 0.065, p = 0.366 (ns); G3 grading accuracy β = 0.556, p = 0.093 (marginally ns); perceived usefulness comparisons G2 vs. G3: all p < 0.05, effect sizes r ∈ [0.382, 0.664]; G3 efficiency reduction ~20 s less than G1 during Exp-1

## Author-noted limitations
- Grading tasks relatively easy for experienced educators; ceiling effects likely limit detectable accuracy improvements
- No strong evidence of lasting skill transfer from GenAI explanation exposure within one-week timeframe
- Concern about over-reliance: educators could uncritically align with AI decisions; Exp-1 controlled for incorrect AI outputs by design, limiting examination of this risk
- All correctly-graded answers in Exp-1 prevents studying miscalibration/overreliance
- Prolific sample of educators may not represent full range of educational contexts and expertise levels
- No comparison of novice vs. expert graders; generalizability to less experienced educators unestablished

## Related pages
- [[li-ai-natural-language-explanations]]
- [[natural-language-explanations]]
- [[explainability]]
- [[appropriate-reliance]]
- [[behavioural-trust]]
- [[user-expertise]]
