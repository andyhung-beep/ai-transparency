# Demand-Driven Transparency for Monitoring Intelligent Agents

**Source file**: [Original article](../../raw/Vered et al._Demand-Driven_Transparency_for_Monitoring_Intelligent_Agents.pdf)

**Summary**: This paper introduces Demand-Driven Transparency (DDT), a user-controlled mode of interacting with AI agent explanations that allows operators to selectively request information at their own discretion, contrasting it with Sequential Transparency (ST) in a complex military multi-vehicle simulation. DDT significantly increased perceived trust and reduced task completion time compared to the fixed-order ST approach.

**Sources**: Vered et al._Demand-Driven_Transparency_for_Monitoring_Intelligent_Agents.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Published in IEEE Transactions on Human-Machine Systems (Vol. 50, No. 3, June 2020), this paper by Vered, Howe, Miller, Sonenberg, and Velloso addresses the challenge of providing transparency in human-agent teaming without overloading human operators. The study introduces a four-level Endsley-based transparency model (ETM) and contrasts two modes of engaging with it: Sequential Transparency (ST), in which operators must view all levels of transparency in a fixed order, and Demand-Driven Transparency (DDT), in which operators choose what to view and in what order.

A controlled experiment with 30 participants used a complex simulated military scenario involving 12 unmanned vehicles (UxVs) with 9 capability types, where an intelligent planning agent suggested courses of action that could contain several types of errors.

## Key Findings

- DDT participants rated their perceived trust in the IA significantly higher than ST participants (mean DDT = 4.04 on a 7-point scale) (source: Vered et al._Demand-Driven_Transparency_for_Monitoring_Intelligent_Agents.txt; domain: military/defense simulation).
- DDT participants completed tasks using only 55% of allotted time on average vs. 65% for ST participants (p = 0.04), indicating reduced workload (source: Vered et al._Demand-Driven_Transparency_for_Monitoring_Intelligent_Agents.txt; domain: military/defense simulation).
- Performance was non-significantly higher for DDT (55% correct) vs. ST (50.6% correct), with DDT participants better at detecting hard-constraint violations (27% vs. 0%, p = 0.03) (source: Vered et al._Demand-Driven_Transparency_for_Monitoring_Intelligent_Agents.txt; domain: military/defense simulation).
- 80% of DDT participants still followed the sequential ETM order voluntarily, suggesting the Endsley-based ordering is intuitive even when not mandated (source: Vered et al._Demand-Driven_Transparency_for_Monitoring_Intelligent_Agents.txt; domain: military/defense simulation).
- Level 3 (Plan Projection) was most consulted by both groups; Level 2 (Input Reasoning) was most often skipped by DDT participants (skipped ~13% of tasks) (source: Vered et al._Demand-Driven_Transparency_for_Monitoring_Intelligent_Agents.txt; domain: military/defense simulation).
- One DDT participant who distrusted the IA viewed minimal transparency levels and succeeded in only 1 of 12 tasks, illustrating the risk of disuse under DDT (source: Vered et al._Demand-Driven_Transparency_for_Monitoring_Intelligent_Agents.txt; domain: military/defense simulation).
- Usability scores did not differ significantly between conditions, indicating DDT gains efficiency without sacrificing usability (source: Vered et al._Demand-Driven_Transparency_for_Monitoring_Intelligent_Agents.txt; domain: military/defense simulation).

## Transparency Constructs

The paper operationalizes transparency through the **Endsley-based Transparency Model (ETM)**, a four-level hierarchical framework:

- **Level 0 – No Knowledge**: IA decisions presented without explanation.
- **Level 1 – Perceived Input**: Factual data as perceived by the IA, enabling detection of missing or erroneous inputs.
- **Level 2 – Input Reasoning**: Inferences made by the IA from Level 1 data.
- **Level 3 – Plan Projection**: Predictions about future outcomes and uncertainties, with justification for recommended plans.

This constitutes a form of [[process-transparency]] (revealing internal reasoning steps) and [[outcome-transparency]] (projecting future states). The framework draws on Situation Awareness (SA) theory and aligns with the SAT model from prior work. It falls under [[algorithmic-transparency]] broadly, making an agent's decision-making process legible to operators.

DDT is distinguished from ST as an **adaptive** transparency mode, giving users coarse-grained control over the order and depth of information acquisition.

## Trust Constructs

Trust was measured using the 12-item Jian, Bisantz, and Drury (2000) scale for trust between people and automation — a standard instrument capturing [[cognitive-trust]] (rational assessment of system reliability). The study also captures [[behavioural-trust]] implicitly through operators' acceptance or rejection of the IA's recommended plans, and through the hard-constraint violation detection rate.

The paper explicitly references the misuse/disuse framework (Parasuraman & Riley, 1997), framing [[trust-calibration]] as a primary design objective. Too much trust leads to automation misuse (over-reliance); too little leads to disuse and under-utilization.

## Relevance to Research Questions

**RQ1**: The paper operationalizes transparency as a multi-level, hierarchical construct grounded in Endsley's Situation Awareness model. Trust is measured via a validated automation trust questionnaire, treated as a perceived, subjective construct that influences reliance behavior. This contributes a domain-specific (military HCI) operationalization to [[rq1-conceptualizations]].

**RQ2**: The paper provides direct evidence that the *modality* of transparency delivery — not just its presence — matters for trust. DDT produced significantly higher perceived trust than ST despite equivalent content availability. This supports a conditional relationship where user control over information flow moderates the transparency-trust link. The non-linear/control dimension contributes to [[rq2-relationships]].

**RQ3**: The study uses student participants with no prior domain expertise; the authors explicitly note the need to replicate with experts. They hypothesize that experts may better exploit DDT's flexibility and may show greater tendency toward automation misuse. This gap is a direct contribution to [[rq3-user-roles]].

## Related pages

- [[process-transparency]]
- [[algorithmic-transparency]]
- [[trust-calibration]]
- [[appropriate-reliance]]
- [[user-expertise]]
- [[rq2-relationships]]
