# Dominguez 2020 — Methods

**Summary**: Two crowdsourced Amazon Mechanical Turk user studies (Study 1 N = 121; Study 2 N = 177) using structural equation modelling to examine how explanation style, recommendation algorithm, device type, and explanation optionality affect user experience with an art image recommender system.

**Sources**: Dominguez et al._Algorithmic and HCI aspects for explaining recommendations.pdf

**Research questions addressed**: RQ1 / RQ2 / RQ3

**Last updated**: 2026-04-19

---

## Study design
experimental (two studies: Study 1 — 3×2 mixed design; Study 2 — 2×2 between-subjects design; both analysed with structural equation modelling)

## Sample
- N: 121 valid participants (Study 1); 177 valid participants (Study 2); approximately 298 total
- Population: general public (crowdsourced workers)
- Domain: e-commerce / art image recommendation
- Country / region: United States (Amazon Mechanical Turk)
- Recruitment method: crowdsourced online (Amazon Mechanical Turk)

## Transparency operationalization
- Type: explainability — example-based (similarity) and feature-based (visual attribute) explanations
- Manipulation or measure: Study 1 — three interface conditions: (1) No explanation; (2) Black-box explanation — top-3 visually similar items from user's past preferences shown alongside the recommendation; (3) Transparent explanation — visual feature bar chart showing attractiveness features (brightness, saturation, sharpness, colorfulness). Crossed with two algorithms: DNN (accurate, opaque) and AVF (less accurate, interpretable visual features). Study 2 — single DNN algorithm; manipulation of device (mobile vs. desktop) and explanation obligatoriness (mandatory vs. optional similar-item explanation).
- Scale / instrument name: ResQue recommender evaluation framework items for perceived explainability/understandability
- Number of items: not reported (individual SEM indicator items from ResQue framework)

## Trust operationalization
- Type: cognitive (self-report)
- Measure: Single self-report item from the ResQue recommender evaluation framework: "I trusted the recommendations made" (0–100 scale)
- Scale / instrument name: ResQue (Pu et al., 2011)
- Number of items: 1
- Behavioural vs self-report: self-report

## Moderators and covariates tested
- Algorithm accuracy (DNN vs. AVF): manipulated in Study 1; positively affected understandability and satisfaction — not a user-level moderator but a system-level boundary condition
- Cognitive load / effort/haste: measured via SEM latent variable; negatively moderated understandability and trust — relevant to RQ3
- Domain expertise (art experience): measured as personal characteristic in Study 2 SEM; experienced art users reported higher satisfaction — relevant to RQ3
- Device type (mobile vs. desktop): manipulated in Study 2; affected preference elicitation time but only indirect effects on satisfaction
- Explanation obligatoriness (mandatory vs. optional): manipulated in Study 2; no significant effect on user experience

## Statistical approach
- Primary analysis method: Structural Equation Modelling (SEM) based on Knijnenburg et al.'s recommender evaluation framework; path coefficients and model fit indices reported for both studies
- Software: not reported
- Key model fit or effect size reported: SEM path coefficients reported (e.g., trust effect on satisfaction approximately 3× understandability in Study 1; 10× in Study 2); model fit indices not explicitly listed in source summary; Cronbach's α for individual scales not reported in source

## Author-noted limitations
- Crowdsourced sample (MTurk) may not represent typical art consumers or engaged recommender system users
- Single-item trust measure lacks psychometric robustness
- SEM models cannot establish causal direction without experimental manipulation of all paths
- No measures of long-term trust or repeated-use behaviour
- Visual feature explanations (AVF) are domain-specific to visual art and may not generalise

## Related pages
- [[dominguez-art-recommendations-hci]]
- [[explainability]]
- [[example-based-explanations]]
- [[algorithmic-transparency]]
- [[cognitive-trust]]
- [[behavioural-trust]]
- [[user-expertise]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]
- [[rq3-user-roles]]
