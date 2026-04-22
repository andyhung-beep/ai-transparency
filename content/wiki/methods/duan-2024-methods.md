# Duan 2024 — Methods

**Summary**: A fully between-subjects online experiment (N = 350) using an 18-condition factorial video-vignette design to examine whether feature-contribution XAI explanations mitigate gender stereotyping of AI agents, supplemented by 9 qualitative interviews.

**Sources**: Duan et al._Mitigating gender stereotypes toward AI agents.pdf

**Research questions addressed**: RQ1 / RQ2 / RQ3

**Last updated**: 2026-04-19

---

## Study design
experimental (fully between-subjects factorial; 3 × 3 × 2 video-vignette design; supplemented by qualitative interviews)

## Sample
- N: 350 (Prolific; fully between-subjects; plus 9 qualitative interview participants)
- Population: general public (US adults)
- Domain: human-computer interaction / social AI / decision support
- Country / region: United States
- Recruitment method: crowdsourced online (Prolific)

## Transparency operationalization
- Type: algorithmic transparency / explainability — feature-contribution explanations
- Manipulation or measure: Between-subjects manipulation — XAI presence (present vs. absent). In the XAI condition, participants viewed a video vignette depicting a ChatGPT-style AI agent providing decision support via a comparative table with feature-contribution explanations (quantifying the weight of each parameter in the agent's final decision). The XAI type was deliberately chosen as feature-contribution (vs. counterfactual or example-based) to highlight the difference between AI and human decision-making and disrupt anthropomorphic heuristics.
- Scale / instrument name: not applicable (between-subjects manipulation; video vignette)
- Number of items: not applicable

## Trust operationalization
- Type: cognitive (domain-specific trust) and behavioural (conformity/decision alignment)
- Measure: (1) Domain-specific trust — 5-item scale measuring willingness to take the agent's advice on a given topic (α = .91); (2) Conformity — behavioural measure of whether participants changed their own decision to match the agent's recommendation (binary; logistic regression used).
- Scale / instrument name: researcher-designed 5-item domain-specific trust scale
- Number of items: 5 (trust scale)
- Behavioural vs self-report: both used (domain trust = self-report; conformity = behavioural decision)

## Moderators and covariates tested
- Agent gender (woman / man / gender-neutral): manipulated (3 levels); interacted with task gender to predict conformity — key moderator of stereotyping effect
- Task gender (feminine / masculine / gender-neutral): manipulated (3 levels); interacted with agent gender in stereotyping analyses
- Need for Cognition: measured; examined as individual difference moderator of XAI response — relevant to RQ3
- Attitudes toward sex roles: measured; examined as individual difference moderator — relevant to RQ3
- Participant gender identity: measured; women and non-binary participants more likely to consciously articulate gender concerns; men showed more implicit stereotyping — relevant to RQ3
- Domain knowledge: measured as covariate
- Perceived humanlikeness: measured as mediator between XAI and conformity (Sobel test for partial mediation)
- Understanding of how agent works: measured as mediator between XAI and humanlikeness

## Statistical approach
- Primary analysis method: factorial ANOVA (for understanding, cognitive effort, perceived humanlikeness, trust); logistic regression (for conformity as binary outcome); Sobel mediation tests; qualitative thematic analysis for interview data
- Software: not reported
- Key model fit or effect size reported: F[1,332] = 50.32, p < .001, η² = .13 (XAI effect on understanding); F[1,332] = 11.72, p < .001 (XAI effect on humanlikeness); Sobel z = 2.49, p = .013 (mediation); logistic regression ORs reported (e.g., OR = 0.05, p = .002 for woman agent on feminine topic in non-XAI condition); α = .91 (trust scale)

## Author-noted limitations
- Video vignette methodology limits ecological validity compared to direct interaction with an AI system
- Prolific US sample may not generalise to other cultural contexts
- Feature-contribution XAI type chosen for theoretical reasons; other XAI types may have different effects on stereotyping
- Self-report trust measure may not capture implicit bias (conformity measure partially addresses this)
- Study focused on first-encounter perceptions; longitudinal stereotyping effects not examined
- Gender operationalized through agent name and pronoun; more nuanced gender expressions not tested

## Related pages
- [[duan-xai-gender-stereotypes-ai]]
- [[explainability]]
- [[algorithmic-transparency]]
- [[cognitive-trust]]
- [[behavioural-trust]]
- [[trust-calibration]]
- [[user-expertise]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]
- [[rq3-user-roles]]
