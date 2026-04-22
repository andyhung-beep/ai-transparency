# Brand et al. (2023) — Methods

**Summary**: Technical paper introducing E-BART, a BART-based transformer architecture for joint veracity prediction and explanation generation, evaluated via automated NLP metrics on three datasets and a crowdsourced human study (Amazon Mechanical Turk) assessing whether machine-generated explanations improve human misinformation detection accuracy.

**Sources**: Brand et al._A neural model to jointly predict and explain truthfulness.pdf

**Research questions addressed**: RQ1 / RQ2

**Last updated**: 2026-04-19

---

## Study design
mixed-methods (technical model development + automated benchmark evaluation + crowdsourced human evaluation experiment)

## Sample
- N: not reported (crowdsourced human evaluation on Amazon Mechanical Turk; exact N not specified in source summary); automated evaluation on three datasets: FEVER (185,445 claims), e-FEVER (FEVER extension), e-SNLI (570,000 sentence pairs)
- Population: general public (non-expert crowdworkers on Amazon Mechanical Turk for human study); no domain expertise required
- Domain: information quality / automated fact-checking (AFC); misinformation detection
- Country / region: not reported (MTurk platform; US-centric by default)
- Recruitment method: Amazon Mechanical Turk (crowdsourced human evaluation)

## Transparency operationalization
- Type: natural language explanation generation (intrinsic / joint explanation) and uncertainty communication (calibrated confidence scores)
- Manipulation or measure: four task variants in the crowdsourced human study — (Task 1) no explanation provided; (Task 2) E-BART machine-generated explanation provided alongside veracity prediction; (Task 3) ground truth explanation provided; (Task 4) both E-BART and ground truth explanations with explicit preference rating. E-BART generates abstractive natural language explanations via a joint prediction head conditioning both veracity classification and explanation on the same decoder hidden states (joint architecture). A separate pipeline (Separate-BART) served as comparison. Calibrated confidence scores produced via temperature scaling (ECE reduced from 11.44% to 1.61%).
- Scale / instrument name: not applicable (explanation was a system output, not a measured construct)
- Number of items: not applicable

## Trust operationalization
- Type: behavioural (trust operationalized indirectly through decision accuracy and appropriate skepticism; no psychometric trust scale used)
- Measure: human annotator accuracy in correctly classifying claims as true or false (aggregated across Task 1 vs. Task 2 comparison); false positive rate (claims incorrectly judged as true) as a measure of over-trust in misinformation; false negative rate as a measure of appropriate skepticism. No self-report trust scale administered.
- Scale / instrument name: not applicable (trust inferred from behavioral accuracy outcomes)
- Number of items: not applicable
- Behavioural vs self-report: behavioural (accuracy and error rates as the primary trust-related outcomes)

## Moderators and covariates tested
- Explanation type (no explanation vs. E-BART explanation vs. ground truth explanation): primary manipulation in human study; moderated human claim classification accuracy
- Note: user expertise was NOT examined — MTurk annotators were non-expert crowdworkers. No manipulation or measurement of domain knowledge, AI familiarity, or fact-checking experience. Relevant to RQ3 as a gap (expert fact-checkers not studied).

## Statistical approach
- Primary analysis method: automated NLP metrics (classification accuracy, ROUGE-1/2/L, BLEU) for model evaluation; descriptive statistics for human study accuracy rates; coherence assessed via an independent "judge" model comparing joint vs. separate pipeline outputs; temperature scaling for confidence calibration
- Software: not reported (standard NLP evaluation libraries implied)
- Key model fit or effect size reported: classification accuracy: FEVER joint E-BART = 75.0–75.1; human study aggregated accuracy: Task 1 (no explanation) = 0.83, Task 2 (E-BART) = 0.90, Task 3 (ground truth) = 0.65; false positives reduced from 122 (no explanation) to 93 (E-BART explanation); ECE after temperature scaling = 1.61%

## Author-noted limitations
- Crowdsourced non-expert annotators may not represent the intended end-users of automated fact-checking systems (journalists, professional fact-checkers)
- Ground truth explanations performed worse than E-BART explanations on human accuracy (Task 3 accuracy = 0.65 vs. Task 2 = 0.90) — a counterintuitive finding not fully explained
- E-BART explanations improve human classification for some claim types but may not generalize across all domains or languages
- The study does not measure trust using validated psychometric scales; behavioral accuracy is used as a proxy, which conflates trust and comprehension effects
- Training datasets (FEVER, e-SNLI) are Wikipedia-derived; generalizability to non-Wikipedia domains (news, social media) is untested

## Related pages
- [[brand-neural-model-truthfulness]]
- [[natural-language-explanations]]
- [[explainability]]
- [[uncertainty-visualization]]
- [[trust-calibration]]
- [[algorithmic-trust]]
- [[rq1-conceptualizations]]

## References
Brand, L., Roitero, K., Soprano, M., Rahimi, S., & Demartini, G. (2023). *A neural model to jointly predict and explain truthfulness of statements*. *ACM Journal of Data and Information Quality, XX*(XX), XXXX. [Volume and page not reported in source summary.]

Toreini, E., et al. (2020). The relationship between trust in AI and trustworthy machine learning technologies. In *Proceedings of the 2020 Conference on Fairness, Accountability, and Transparency* (pp. 272–283).
