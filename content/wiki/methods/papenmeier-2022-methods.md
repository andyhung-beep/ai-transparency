# Papenmeier 2022 — Methods

**Summary**: A large-scale between-subjects online experiment (N = 959) testing how explanation faithfulness (faithful/random/none) and classifier accuracy (high/medium/antagonistic) jointly affect self-reported and behavioural trust in a text-classification decision-support system.

**Sources**: Papenmeier et al._It_s complicated.pdf

**Research questions addressed**: RQ1 / RQ2 / RQ3

**Last updated**: 2026-04-19

---

## Study design
experimental (between-subjects, 3 × 3 factorial design)

## Sample
- N: 959
- Population: general public (crowdsourced online participants)
- Domain: social media moderation / offensive-language classification
- Country / region: not reported
- Recruitment method: online crowdsourcing (platform not specified)

## Transparency operationalization
- Type: local explanation / explainability (word-highlight saliency)
- Manipulation or measure: Between-subjects manipulation across three levels — (1) faithful explanation: top-4 words most decisive for the classifier identified via L2X algorithm; (2) random explanation: 4 arbitrarily chosen words highlighted; (3) no explanation: classification output only. Manipulation check confirmed faithful highlights retained ~98% label agreement vs. ~74% for random.
- Scale / instrument name: not applicable (between-subjects experimental manipulation)
- Number of items: not applicable

## Trust operationalization
- Type: cognitive (self-reported) and behavioural
- Measure: (1) Self-reported trust via Körber's (2020) validated 19-item Trust in Automation questionnaire covering reliability/competence, predictability/understanding, familiarity, intention of developers, propensity to trust, and trust in automation; (2) Behavioural trust via switching rate — proportion of classifications participants changed to match the classifier between a no-AI block (block 1) and a with-AI block (block 2).
- Scale / instrument name: Körber Trust in Automation Scale (2020)
- Number of items: 19
- Behavioural vs self-report: both used; correlation between measures reported (r = 0.30 overall)

## Moderators and covariates tested
- Age: measured demographic covariate; no significant moderation found
- Gender: measured demographic covariate; no significant moderation found
- Language proficiency: measured covariate (relevant given tweet language classification task); no significant moderation found
- Note: AI literacy and domain expertise were not examined — flagged as a gap relevant to RQ3

## Statistical approach
- Primary analysis method: mixed ANOVA (between-subjects: accuracy × explanation; within-subjects: block) and Pearson correlations for trust measure comparison
- Software: not reported
- Key model fit or effect size reported: partial η², Pearson r (self-report vs. behavioural trust correlation = 0.30); specific p-values and means reported per condition

## Author-noted limitations
- Sample was recruited online and may not reflect domain experts or professional content moderators
- AI literacy and domain expertise were not measured or controlled
- Single use case (offensive tweet classification) limits generalisability
- Self-reported and behavioural trust measures diverge substantially, raising questions about which outcome variable is theoretically appropriate
- No longitudinal follow-up; trust effects measured after a single session

## Related pages
- [[papenmeier-its-complicated-transparency-trust]]
- [[explainability]]
- [[algorithmic-transparency]]
- [[cognitive-trust]]
- [[behavioural-trust]]
- [[trust-calibration]]
- [[rq2-relationships]]
- [[rq3-user-roles]]
