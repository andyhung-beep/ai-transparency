# Algorithm, Expert, or Both? Evaluating the Role of Feature Selection Methods on User Preferences and Reliance

**Source file**: [Original article](../../raw/Kornowicz & Thommes_Algorithm, expert, or both_.pdf)

**Summary**: An incentivised online behavioural experiment (n = 216) examines whether the method used to select features for a machine-learning model (algorithm-based, expert-based, or combined) affects users' stated preferences and actual advice reliance, finding a large attitude–behaviour gap: users prefer combined or expert methods but rely equally on all three.

**Sources**: Kornowicz & Thommes_Algorithm, expert, or both_.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Kornowicz and Thommes (2025), published in *PLOS ONE*, investigate human involvement in the machine-learning pipeline at the feature-selection stage. Feature selection — choosing which input variables are used to train a model — is argued to be an underexplored locus of transparency. The authors distinguish three conditions:

- **Algorithm**: features selected by a data-driven algorithm.
- **Expert**: features selected by domain experts.
- **Combination**: features selected by a joint algorithm-and-expert approach.

The study uses a between-subjects, incentivised judge-advisor system (JAS) with two decision domains (Cardio: cardiovascular disease classification; Football: soccer match outcome prediction). Participants were recruited from Prolific (n = 216 after exclusions, 59.7% women, mean age 34.2, UK-based). Two treatments were run: (1) a Choice treatment in which participants selected their preferred feature-selection method before performing tasks; (2) a No Choice treatment in which method was randomly assigned.

Advice reliance was operationalised as "Switch to Advice" — whether a participant changed a binary decision to align with the ML model's prediction when the two initially disagreed. Personality, risk-taking, technology affinity, and AI attitude scales were collected as covariates.

## Key Findings

- In the Choice treatment, Combination was selected most (47.7%), followed by Expert (32.1%) and Algorithm (20.2%), significantly deviating from chance; H1a and H1b were supported overall (domain: general/online experiment). (source: Kornowicz & Thommes_Algorithm, expert, or both_.pdf)
- Domain moderated preferences: in Cardio (medical), Combination and Expert were equally popular; in Football (sports), Combination was significantly more preferred than both others (domain: medical and sports). (source: Kornowicz & Thommes_Algorithm, expert, or both_.pdf)
- In the No Choice treatment, feature-selection method had no significant effect on Switch to Advice (the dependent variable for reliance), rejecting H2a and H2b (domain: general/online experiment). (source: Kornowicz & Thommes_Algorithm, expert, or both_.pdf)
- Giving users the choice of method also did not significantly affect reliance, rejecting H3 (domain: general/online experiment). (source: Kornowicz & Thommes_Algorithm, expert, or both_.pdf)
- A significant positive domain effect was found: reliance was 17.98 percentage points higher in the medical domain (Cardio) than in the sports domain (Football) even though payoff structures were identical, suggesting domain-specific norms or perceived AI competence drive reliance rather than objective stakes (domain: medical vs. sports). (source: Kornowicz & Thommes_Algorithm, expert, or both_.pdf)
- Self-reported confidence in one's own initial decision was negatively associated with reliance; older participants relied less on AI; Openness (Big Five) was negatively associated with reliance (domain: general/online experiment). (source: Kornowicz & Thommes_Algorithm, expert, or both_.pdf)
- Higher risk-taking was associated with preference for Algorithm and Combination over Expert, interpreted via Diffusion of Innovations theory (early adopters are more risk-prone). (source: Kornowicz & Thommes_Algorithm, expert, or both_.pdf)
- The attitude–behaviour gap is explained as consistent with dual-process theory: deliberate System 2 reasoning governs stated preferences while automatic System 1 governs actual reliance under cognitive load. (source: Kornowicz & Thommes_Algorithm, expert, or both_.pdf)

## Transparency Constructs

The paper treats **process transparency** — revealing how the ML pipeline was constructed (who selected the features) — as an operationalisation of algorithmic transparency. This is distinct from outcome explanations or post-hoc interpretability. The study shows that process-level transparency information (which method was used) shifts stated preferences but not behaviour, suggesting its impact on [[behavioural-trust]] (reliance) is limited. Related to [[algorithmic-transparency]] and [[process-transparency]].

Feature selection visibility (participants could see which 6 of 12 features the model used) adds a partial form of [[outcome-transparency]] by making the model's inputs visible.

## Trust Constructs

- **Behavioural trust (reliance)**: operationalised via Switch to Advice — a revealed-preference, incentivised measure. The paper explicitly distinguishes this from attitudinal trust scales.
- **Stated/attitudinal preferences**: captured pre-task and treated as a proxy for cognitive/affective trust, showing strong preference for human-expert involvement.
- **Algorithm aversion / algorithm appreciation**: the study is embedded in this literature — algorithm aversion refers to preference and/or reliance on human over algorithmic advice; appreciation is the reverse. Results document aversion in stated preferences but not in behaviour.

See [[behavioural-trust]], [[algorithm-aversion]], [[appropriate-reliance]], [[trust-calibration]].

## Relevance to Research Questions

**RQ1**: The paper contributes an operationalisation of transparency at the pipeline (process) level rather than at the prediction level. It highlights that transparency can be located in model construction (feature selection) rather than only in explanation of outputs. The distinction between stated preferences and actual reliance also speaks to the difference between attitudinal and behavioural measurement of trust. See [[rq1-conceptualizations]].

**RQ2**: The null finding for the effect of feature-selection method on actual reliance is a key conditional/null result. Despite strong stated preferences for human-involved methods, behavioural reliance is equivalent across methods. This replicates earlier attitude–behaviour gaps in the algorithm aversion literature (Rabinovitch et al. 2024; Rebitschek et al. 2021) and adds a new mechanism-specific instance. The positive domain effect (Cardio > Football) is a conditional pattern relevant to RQ2. See [[rq2-relationships]].

**RQ3**: The paper does not study professional experts but does include domain as a moderator and risk-taking as a user characteristic. The finding that domain (medical vs. sports) drives reliance more than feature-selection method suggests that contextual factors independent of user expertise shape reliance. The limitation of using lay participants rather than professionals is explicitly noted, with the authors arguing that known biases are similar across lay and expert populations. See [[rq3-user-roles]].

## Related pages

- [[algorithm-aversion]]
- [[behavioural-trust]]
- [[process-transparency]]
- [[appropriate-reliance]]
- [[domain-context]]
- [[rq2-relationships]]
