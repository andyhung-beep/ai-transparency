# Effect of Automation Transparency in the Management of Multiple Unmanned Vehicles

**Source file**: [Original article](../../raw/Bhaskara et al._Effect of automation tranparency in the management of multiple unmanned vehicles.pdf)

**Summary**: This paper experimentally tests three levels of automation transparency in an unmanned vehicle (UV) mission-assignment task, finding that intermediate transparency (Level 1+2) improved accuracy of automation use, while higher transparency (Level 1+2+3) unexpectedly induced automation bias and reduced accuracy.

**Sources**: Bhaskara et al._Effect of automation tranparency in the management of multiple unmanned vehicles.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Bhaskara et al. (2021) report a between-participants experiment (N = 176 undergraduate students) examining whether increased automation transparency, operationalized using the Situation Awareness-based Agent Transparency (SAT) model, could improve the accuracy with which human operators accept or reject recommendations from an automated decision aid. The study simulated a defense domain context in which participants selected the most suitable unmanned vehicle (UV) to complete surveillance and rescue missions. Automation reliability was set at 75% (Plan A was optimal on 75% of trials), and participants needed to integrate contextual intelligence updates (Intel) that the automated system could not access.

Three transparency levels were manipulated between participants. Level 1 provided basic plan information (purpose and intent). Level 1+2 additionally disclosed the mathematical formulae underlying the Recommender's calculations. Level 1+2+3 further provided a projected-outcome visualization showing how the two candidate UVs would perform relative to each other on each weighted mission attribute. Outcome measures included signal detection sensitivity (d'), hit rate, correct rejection rate, response bias (c), decision time, NASA-TLX workload, trust in automation (Merritt scale), and perceived usability (SUS).

The study is grounded in the SAT model (Chen et al., 2014) and Lee and See's (2004) theory of trust in automation. It is notable for testing the SAT model under time-pressure conditions with complex quantitative data, contrasting with prior qualitative paradigms (Mercado et al., 2016; Stowers et al., 2020) in which all three levels of transparency produced monotonic accuracy gains.

## Key Findings

- Participants in the Level 1+2 transparency condition used automation significantly more accurately (higher d') than those in the Level 1 condition, without increasing decision time or workload (defense/autonomous systems domain). (source: Bhaskara et al._Effect of automation tranparency in the management of multiple unmanned vehicles.txt)
- Contrary to SAT model predictions, participants in the Level 1+2+3 condition used automation less accurately than those in the Level 1+2 condition, because they were more biased toward agreeing with automation (defense/autonomous systems domain). (source: Bhaskara et al._Effect of automation tranparency in the management of multiple unmanned vehicles.txt)
- The Level 1+2+3 projected-outcome visualization led to faster correct and incorrect decisions, suggesting the visualization induced rapid, less deliberative processing (defense/autonomous systems domain). (source: Bhaskara et al._Effect of automation tranparency in the management of multiple unmanned vehicles.txt)
- Subjective trust in automation and perceived usability did not differ across transparency conditions, indicating that behavioral automation use and reported trust dissociated (defense/autonomous systems domain). (source: Bhaskara et al._Effect of automation tranparency in the management of multiple unmanned vehicles.txt)
- The finding that higher transparency can induce automation bias rather than calibrated reliance challenges the assumption that more transparency always yields better human-automation teaming (defense/autonomous systems domain). (source: Bhaskara et al._Effect of automation tranparency in the management of multiple unmanned vehicles.txt)
- A possible framing effect is proposed: the projected outcome visualization prominently framed Plan A as superior, leading participants to anchor on it and under-weigh contradictory Intel (defense/autonomous systems domain). (source: Bhaskara et al._Effect of automation tranparency in the management of multiple unmanned vehicles.txt)

## Transparency Constructs

The study operationalizes three levels of the SAT model:
- **Level 1 (process transparency / intent disclosure)**: Communicates what the automation is trying to achieve and the mission attribute weightings.
- **Level 1+2 (algorithmic transparency / rationale)**: Adds the mathematical formulae the Recommender used to calculate UV capability scores, revealing the reasoning behind the recommendation.
- **Level 1+2+3 (outcome transparency / projection visualization)**: Adds a bar-chart visualization of projected relative performance of the two recommended plans on each weighted attribute.

The study thus spans [[process-transparency]], [[algorithmic-transparency]], and [[outcome-transparency]] constructs within the SAT framework. No uncertainty visualization (Level 3 uncertainty) was included because the task context did not involve environmental uncertainty.

## Trust Constructs

Trust was measured as a self-reported construct using a modified six-item Merritt (2011) scale (5-point Likert), capturing perceived competence and overall trust in the automated recommender. This aligns primarily with [[cognitive-trust]] (competence-based evaluation). The study also captures behavioral trust operationalized as actual automation use (hit rate, correct rejection rate, d'), which maps to [[behavioural-trust]] and [[appropriate-reliance]]. A key finding is that reported (cognitive) trust did not differ across conditions while behavioral (reliance) accuracy did, suggesting that transparency affected calibration of reliance more than subjective trust ratings. The study explicitly discusses [[trust-calibration]] and [[algorithm-aversion]] concepts (disuse vs. misuse).

## Relevance to Research Questions

**RQ1**: The study operationalizes transparency as a three-level construct following the SAT model, covering intent, rationale, and projected outcomes. Trust is decomposed into subjective ratings and behavioral reliance, illustrating the gap between these two operationalizations. Workload (NASA-TLX) and signal detection (d', c) are used as complementary performance outcomes.

**RQ2**: The paper reports a non-linear (inverted-U) relationship between transparency level and accuracy of automation use: Level 1+2 improved accuracy over Level 1, but Level 1+2+3 impaired accuracy relative to Level 1+2. This is a rare empirical demonstration that increasing transparency can be counterproductive, constituting direct evidence of a non-monotonic effect pattern. The study explicitly advocates against the "file drawer problem" of publishing only positive transparency results.

**RQ3**: User expertise was not a primary independent variable; the sample consisted of undergraduate novices. The authors acknowledge this as a limitation and call for future research with expert UV operators, noting that differences in cognitive skills and motivation between novices and experts are likely to affect transparency effects.

## Related pages

- [[algorithmic-transparency]]
- [[process-transparency]]
- [[outcome-transparency]]
- [[trust-calibration]]
- [[appropriate-reliance]]
- [[rq2-relationships]]
