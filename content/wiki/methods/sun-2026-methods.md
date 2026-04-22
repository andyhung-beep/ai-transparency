# Sun et al. (2026) — Methods

**Summary**: A 3×3 between-subjects online experiment (N = 227) crossing three levels of algorithmic transparency (absent, low, high) with three levels of performance expectation confirmation (positive disconfirmation, simple confirmation, negative disconfirmation) in a fictitious AI-powered online dating platform, testing a moderated mediation model in which perceived understanding mediates transparency's effect on cognitive trust.

**Sources**: Sun et al._Does transparency matter when an AI system meets performance.pdf

**Research questions addressed**: RQ1 / RQ2

**Last updated**: 2026-04-19

---

## Study design
experimental (3×3 between-subjects online experiment)

## Sample
- N: 227
- Population: general public (lay users; no domain expertise required)
- Domain: online dating / matchmaking (AI-powered romantic partner recommendation platform "SmartMatch")
- Country / region: United States (CloudResearch / MTurk)
- Recruitment method: CloudResearch panel (Amazon Mechanical Turk)

## Transparency operationalization
- Type: algorithmic transparency — three-level manipulation of disclosure depth
- Manipulation or measure: between-subjects manipulation; (1) No transparency — dating site provides no information about recommendation process; (2) Low transparency — discloses algorithm name and one sentence stating it "analyzes and matches individuals according to scientific principles" (minimal disclosure); (3) High transparency — discloses algorithm name ("Duet Total Compatibility System"), the theoretical principles (similarity and complementarity), and the six personality-factor criteria used (process transparency)
- Scale / instrument name: not applicable (transparency was a vignette-based scenario manipulation)
- Number of items: not applicable

## Trust operationalization
- Type: cognitive trust and behavioural intentions (as proxy for behavioural trust)
- Measure: self-report Likert-scale items assessing users' beliefs about the AI system's reliability, competence, and dependability (cognitive trust); behavioural intentions measured as self-reported likelihood of continuing to use the dating site
- Scale / instrument name: not reported (adapted items; scale name not specified in source)
- Number of items: not reported
- Behavioural vs self-report: self-report

## Moderators and covariates tested
- Performance expectation confirmation / disconfirmation: between-subjects manipulation — (1) positive disconfirmation (more attractive and numerous matches than expected); (2) simple confirmation (average number and attractiveness of matches); (3) negative disconfirmation (fewer and less attractive matches than expected); tested as moderator of the transparency → perceived understanding → trust mediation chain
- Perceived understanding: measured as a mediator, not a moderator; operationalized as self-reported comprehension of how the AI system works
- Note: user expertise and AI literacy were not measured or included — relevant to RQ3 as a gap

## Statistical approach
- Primary analysis method: moderated mediation analysis (PROCESS macro or equivalent); ANOVA for transparency main effect on perceived understanding; indirect effect tests with 95% confidence intervals (bootstrapping)
- Software: not reported
- Key model fit or effect size reported: transparency main effect on understanding F(2, 217) = 6.445, p = .002, η² = 0.06; moderated mediation index for cognitive trust b = -0.51, 95% CI [-0.92, -0.10]; for behavioural intentions b = -0.72, 95% CI [-1.30, -0.17]; indirect effect for no vs. low transparency on trust b = -0.27, 95% CI [-0.49, -0.08]

## Author-noted limitations
- The online dating context may limit generalisability to other AI application domains where trust stakes differ
- The transparency manipulations are vignette-based and do not involve real AI system interaction, reducing ecological validity
- User AI literacy and prior experience with algorithmic recommendations were not measured or controlled
- The study does not measure affective trust or dispositional trust; focus is exclusively on cognitive trust
- Expectation manipulation relied on outcome framing; actual AI performance quality was not independently varied

## Related pages
- [[sun-transparency-performance-expectations]]
- [[algorithmic-transparency]]
- [[cognitive-trust]]
- [[behavioural-trust]]
- [[trust-calibration]]
- [[disclosure]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]

## References
Sun, Y., et al. (2026). Does transparency matter when an AI system meets performance expectations? An experiment with an online dating site. *Computers in Human Behavior*.

Bhattacherjee, A. (2001). Understanding information systems continuance: An expectation-confirmation model. *MIS Quarterly, 25*(3), 351–370.

Chaiken, S. (1980). Heuristic versus systematic information processing and the use of source versus message cues in persuasion. *Journal of Personality and Social Psychology, 39*(5), 752–766.
