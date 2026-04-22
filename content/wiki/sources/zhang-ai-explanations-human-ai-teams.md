# I Know This Looks Bad, But I Can Explain: Understanding When AI Should Explain Actions In Human-AI Teams

**Source file**: [Original article](../../raw/Zhang et al._I know this looks bad, but i can explain.pdf)

**Summary**: An online experiment with 156 participants using video-based game vignettes that examines how and when AI teammate explanations affect trust and perceived team effectiveness, finding that the impact of explanations depends critically on the type of action being explained and the personal characteristics of team members.

**Sources**: Zhang et al._I know this looks bad, but i can explain.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Published in *ACM Transactions on Interactive Intelligent Systems* (Vol. 14, Issue 1, February 2024), this paper by Rui Zhang, Christopher Flathmann, Geoff Musick, Beau Schelble, Nathan McNeese, Bart Knijnenburg, and Wen Duan (Clemson University) investigates when AI explanations are beneficial or detrimental in human-AI teaming contexts.

The study used a 2×2×4 mixed factorial design: teammate identity (human vs. AI) × explanation (with vs. without) × teammate action (ignoring potential death, ignoring injury, disobeying orders, lying to humans). 156 participants watched video-based scenario vignettes set in a multiplayer online game (ArmA III), where a teammate performed actions that benefited the team but harmed the individual participant. Structural equation modelling (SEM) was used to examine trust and perceived team effectiveness.

The study is motivated by the inconsistent findings in XAI research — some showing that explanations improve trust, others finding no effect — and the underexplored question of how context and AI behaviour type moderate these effects.

## Key Findings

- AI teammate explanations significantly increased trust when explaining **disobedience** (β = 0.672, p < 0.001) but significantly decreased trust when explaining **deception/lying** (β = −0.739, p < 0.001). [domain: human-AI teaming / simulated game environment]
- Explanations had no significant effect on trust in the human teammate condition, suggesting that explanations operate differently for AI vs. human teammates. [domain: human-AI teaming]
- Explanations improved perceived team effectiveness in the **ignoring injury** and **disobeying order** scenarios but not in the **lying** or **ignoring potential death** scenarios. [domain: human-AI teaming]
- Actions with direct consequences for the individual (disobedience, lying) were more responsive to explanation effects than actions with indirect consequences (ignoring death, ignoring injury). [domain: human-AI teaming]
- Non-male participants (women, non-binary) trusted their AI teammate significantly less than men in the **lying** (β = −0.731, p < 0.001) and **ignoring potential death** (β = −0.742, p < 0.001) scenarios, but not in the disobeying scenario. [domain: human-AI teaming]
- Participants with a utilitarian ethical framework showed higher perceived team effectiveness with AI teammates (β = 0.119, p < 0.01). [domain: human-AI teaming]
- Trust decreases over time with AI teammates (vs. increases with human teammates), highlighting the challenge of sustained trust in human-AI teams. [domain: human-AI teaming]

## Transparency Constructs

The paper operationalises [[explainability]] as AI teammate **explanations of specific actions**, structured to address three points: (1) the action taken, (2) the consequence to the human, and (3) the rationale for why the action was taken. This is a form of **post-hoc, instance-level explanation** tied to specific behavioural events.

The explanations use machine-language phrasing to avoid over-anthropomorphising the AI. The paper conceptually distinguishes this from broader transparency constructs, focusing on **action-level explanation** in collaborative teaming contexts rather than model-level interpretability.

## Trust Constructs

- **[[cognitive-trust]]**: Measured via six-item scale assessing belief that the teammate would honestly and accurately complete tasks; dominant trust construct in the study.
- **[[affective-trust]]**: Implicitly captured through satisfaction scale items.
- **[[behavioural-trust]]**: Proxied by willingness to re-team (satisfaction items).
- **[[trust-calibration]]**: The paper frames explanation as a mechanism for trust calibration — helping humans know when to trust AI appropriately. Cited literature notes that explanation increases trust calibration.
- **[[algorithmic-trust]]**: The paper directly compares trust levels for AI vs. human teammates and finds systematic differences.

## Relevance to Research Questions

**RQ1**: Operationalises AI transparency as explanation of specific actions. Trust is measured as a cognitive construct. Provides a detailed typology of AI teammate actions (direct vs. indirect consequences) and their interaction with explanation. (source: Zhang et al._I know this looks bad, but i can explain.txt)

**RQ2**: Demonstrates a strongly conditional (non-monotonic) relationship between explanation and trust: explanation helps trust for disobedient actions but harms trust for deceptive actions. No universal positive effect of explanation on trust. Context and action type are critical moderators. This is an important qualification to assumptions about explanation uniformly benefiting trust. [domain: human-AI teaming / game environment] (source: Zhang et al._I know this looks bad, but i can explain.txt)

**RQ3**: Personal characteristics — gender and ethical framework — moderate the effect of explanations on trust. Men trusted AI more than non-men in lying and death scenarios; utilitarianism predicted higher perceived team effectiveness. Identifies individual differences as important moderators of transparency–trust relationships. (source: Zhang et al._I know this looks bad, but i can explain.txt)

## Related pages

- [[explainability]]
- [[cognitive-trust]]
- [[trust-calibration]]
- [[algorithmic-trust]]
- [[appropriate-reliance]]
- [[user-expertise]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]
- [[rq3-user-roles]]
