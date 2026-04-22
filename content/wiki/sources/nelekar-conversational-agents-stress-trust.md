# Effectiveness of Embodied Conversational Agents for Managing Academic Stress at an Indian University (ARU) during COVID-19

**Source file**: [Original article](../../raw/Nelekar et al._Effectiveness embodied conveersational agents for managing academic stress.pdf)

**Summary**: A between-subjects study with 61 Indian university students testing whether an explainable embodied conversational agent (ARU) can reduce study stress and build a working alliance through three patterns of tailored explanations (belief-based, goal-based, belief-and-goal-based); finds significant stress reduction and positive trust across all explanation groups, with user context and personality moderating behaviour-change intention.

**Sources**: Nelekar et al._Effectiveness embodied conveersational agents for managing academic stress.pdf

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Published in the *British Journal of Educational Technology* (2021), this paper by Nelekar, Abdulrahman, Gupta, and Richards adapts a Western Explainable Agent (Sarah) for Indian undergraduate students as ARU (mAnaging stRess at University). ARU is a belief-desire-intention (BDI) agent that provides personalised, culturally adapted explanations for study-stress coping behaviours (physical activity, healthy diet, studying in groups, meeting new people) during the COVID-19 pandemic. The study addresses cultural portability of explainable AI and agent-based health interventions.

The three explanation types manipulated are:
1. **Belief-based**: References the student's stated barriers to a behaviour.
2. **Goal-based**: References the student's stated motivations.
3. **Belief-and-goal-based**: Combines both.

Trust is measured using an adapted Mayer and Davis (1999) scale covering ability, benevolence, integrity, and trust. Working alliance (task, goal, bond dimensions) is measured with the Working-Alliance Inventory Short Revised.

## Key Findings

- All three explanation groups showed a **significant reduction in self-reported study stress** after interacting with ARU (Wilcoxon signed-rank tests, p < 0.01). (Domain: higher education/mental health, India)
- **No significant between-group differences in trust** (ability, benevolence, integrity, or overall trust) were found, contrary to the hypothesis that explanation type would affect relationship quality. (Domain: higher education)
- Participants in the **belief-and-goal group showed the highest average trust and working alliance** scores and the lowest non-response rates, suggesting combined explanations may be most engaging, though the difference was not significant. (Domain: higher education)
- Indian students showed a very **high propensity to trust** (above 4.5/5), significantly higher than Western samples (3.12/5). This high dispositional trust correlated with trust in ARU, suggesting that trust in the agent may partly reflect cultural trait-level trust rather than the agent's explanation design. (Domain: higher education, cross-cultural)
- **Goal-based explanations** produced the largest number of significant behaviour-change intentions across all four target behaviours; belief-and-goal explanations produced significant change in fewer behaviours. (Domain: higher education)
- **Student achievement aim** was the strongest predictor of behaviour-change intention: only students aiming for a high GPA (8.5–10) showed consistent significant changes.
- Personality traits moderated specific outcomes: conscientiousness correlated with intention to exercise (belief group); emotional stability and extroversion moderated healthy eating intention (goal group).

## Transparency Constructs

- **Natural language explanations**: ARU provides tailored verbal explanations referencing the student's own beliefs and goals. These are a form of [[natural-language-explanations]] in a conversational interface.
- **Process transparency**: The agent's reasoning (why a recommendation is given) is disclosed to the user at the point of recommendation, instantiating a local, user-centred transparency mechanism. See [[process-transparency]].
- **Disclosure**: ARU discloses the basis for its advice (the user's stated beliefs and goals), making the recommendation rationale explicit. See [[disclosure]].

## Trust Constructs

- **Cognitive trust**: Measured via ability and integrity sub-scales of the Mayer & Davis instrument. See [[cognitive-trust]].
- **Affective trust**: Measured via the benevolence sub-scale and the working-alliance bond dimension. See [[affective-trust]].
- **Behavioural trust**: Operationalised as intention to change behaviour (not yet actual behaviour change). See [[behavioural-trust]].
- **Dispositional trust**: Propensity to trust was measured as a baseline covariate; Indian students' high propensity correlates with trust in the agent, raising questions about cross-cultural measurement. See [[algorithmic-trust]].

## Relevance to Research Questions

**RQ1**: Contributes an operationalisation of trust in a conversational AI context using the Mayer and Davis (1999) ability-benevolence-integrity-trust framework alongside the working alliance inventory—both distinct from the HCT scale used in clinical decision support literature. Explainability is operationalised as BDI explanation patterns (belief-based, goal-based, or combined), distinct from feature-importance or contrastive explanation types. See [[rq1-conceptualizations]].

**RQ2**: Finds a mostly null effect of explanation type on trust—all three patterns produced equivalent trust and working alliance. Stress reduction and behaviour-change intention were more sensitive to individual and cultural factors (personality, achievement aim, GPA aspiration) than to explanation type. This constitutes a conditional null finding: explanation style matters less than user context. See [[rq2-relationships]].

**RQ3**: Cultural context (India vs. Western), personality traits, academic achievement aim, and gender all modulate agent effectiveness. The paper foregrounds that findings from Western ECA studies do not straightforwardly transfer to non-Western, lower-resource, high-stigma contexts. User propensity to trust is identified as a possible confound for trust measurement in this domain. See [[rq3-user-roles]], [[user-expertise]], [[domain-context]].

## Related pages

- [[natural-language-explanations]]
- [[affective-trust]]
- [[cognitive-trust]]
- [[behavioural-trust]]
- [[domain-context]]
- [[rq2-relationships]]
