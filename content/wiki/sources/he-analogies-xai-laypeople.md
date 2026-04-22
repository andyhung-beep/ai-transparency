# Opening the Analogical Portal to Explainability: Can Analogies Help Laypeople in AI-assisted Decision Making?

**Source file**: [Original article](../../raw/He et al._Opening the analogical portal to explainability.pdf)

**Summary**: This paper proposes and evaluates analogy-based explanations as a method to bridge the knowledge gap between concept-level XAI outputs and laypeople, finding that while high-quality analogies show qualitative promise, they did not produce statistically significant improvements in appropriate reliance in a skin cancer detection task.

**Sources**: He et al._Opening the analogical portal to explainability.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

He et al. (2024), published in the *Journal of Artificial Intelligence Research*, investigate whether analogy-based explanations can make concept-level AI explanations more accessible to non-expert users. The authors argue that concept-level explanations from XAI systems (e.g., references to "cribriform and fused glands in needle core biopsy") remain opaque to laypeople lacking domain knowledge. Analogies—structural mappings from unfamiliar target domains to familiar source domains—are proposed as a bridge. The paper proceeds in two phases: (1) a crowd-based analogy generation and expert evaluation study, and (2) an empirical human-AI decision-making study (N = 280) using a skin cancer detection task.

## Key Findings

- A crowd-computing method produced 600 analogy-based explanations; approximately 80% were factually correct and 87% were valid (domain-compliant). [domain: general/crowd-computing]
- Expert evaluation of analogy quality showed that dimensions of simplicity (M = 4.11) and familiarity (M = 4.19) scored highest, while structural correspondence (M = 2.66) and relational similarity (M = 3.01) scored lowest — suggesting generated analogies are comprehensible but structurally imprecise. [domain: crowd-computing]
- In the human-AI decision-making study, providing target-domain information only (Concept-Imp condition) was most effective at reducing under-reliance but also introduced over-reliance. [domain: healthcare/medical imaging]
- Full analogy-based explanations did not significantly increase appropriate reliance (RAIR or RSR) compared to concept-only conditions; analogies could even have some negative effects on appropriate reliance in certain conditions. [domain: healthcare/medical imaging]
- Analogies did not impose a significantly higher cognitive load (NASA-TLX) and did not significantly delay decision-making efficiency. [domain: healthcare/medical imaging]
- Qualitative analysis revealed that human intuition and perceived plausibility of analogies shaped reliance patterns, sometimes overriding the informational content of the analogy. [domain: healthcare/medical imaging]
- User medical expertise moderated the effect: understanding of commonsense explanations varied with recipient experience, pointing to the need for personalization. [domain: healthcare/medical imaging]
- Significant positive correlations were found between all analogy quality dimensions (structural correspondence, relational similarity, familiarity, transferability, simplicity) and the perceived helpfulness of the explanation. [domain: crowd-computing]

## Transparency Constructs

The paper operationalizes [[explainability]] at the concept level (concept bottleneck models producing high-level feature labels) and proposes analogy-based explanation as an enhancement of [[natural-language-explanations]]. The analogy framework is essentially a form of [[example-based-explanations]] extended into a commonsense domain. Nine qualitative dimensions for assessing analogy quality are proposed: structural correspondence, relational similarity, transferability, helpfulness, familiarity, simplicity, misunderstanding, syntactic correctness, and factual correctness.

## Trust Constructs

Trust and reliance are operationalized primarily as [[behavioural-trust]]: the paper measures Switch Fraction, Relative Positive AI Reliance (RAIR), and Relative Positive Self-Reliance (RSR) as indices of [[appropriate-reliance]]. Subjective trust is measured via the Trust in Automation (TiA) questionnaire covering reliability/competence, understanding/predictability, propensity to trust, and overall trust in automation. The paper also measures [[cognitive-trust]] implicitly through participants' understanding of the AI system as measured by post-task concept identification.

## Relevance to Research Questions

**RQ1**: The paper operationalizes XAI explanations through a concept-bottleneck model and introduces analogy-based explanation as a novel operationalization aimed at bridging domain knowledge gaps for layperson users. It provides a detailed taxonomy of analogy quality dimensions (structural correspondence, relational similarity, familiarity, simplicity, transferability), contributing to how explainability is measured.

**RQ2**: The paper reports a null or near-null effect of analogy-based explanations on appropriate reliance compared to concept-only explanations in a high-stakes medical decision-making task, contributing to the literature on conditional and non-linear effects of XAI. Concept-Imp (target domain only) significantly reduced under-reliance but also produced over-reliance — a non-linear/mixed effect. Full analogy conditions showed no statistically significant benefit.

**RQ3**: The paper explicitly examines user expertise as a moderator: medical domain knowledge and skin cancer expertise were measured as covariates, and the study found that the understanding of commonsense explanations varied with recipient experience. This directly addresses how non-expert versus expert users process different explanation styles.

## Related pages

- [[explainability]]
- [[example-based-explanations]]
- [[natural-language-explanations]]
- [[appropriate-reliance]]
- [[user-expertise]]
- [[rq2-relationships]]
