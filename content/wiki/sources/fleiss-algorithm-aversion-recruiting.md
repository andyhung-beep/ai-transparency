# Mitigating Algorithm Aversion in Recruiting: A Study on Explainable AI for Conversational Agents

**Source file**: [Original article](../../raw/Fleiß et al._Mitigating algorithm aversion in recruiting.pdf)

**Summary**: A quota-representative experiment (n = 490) testing how different XAI explanation types and decision objectivity (soft skills vs. verifiable qualifications) affect acceptance of AI-based conversational agents in recruiting contexts, finding that explanation content matters more than explanation type.

**Sources**: Fleiß et al._Mitigating algorithm aversion in recruiting.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Fleiß, Bück, and Thalmann (2024) examine algorithm aversion and AI acceptance in the recruiting domain, where AI-based conversational agents (CAs) are increasingly used for applicant pre-selection. The study employs a within-subject experimental design (n = 490, quota-representative sample from Germany and Austria) to test two main factors: (1) the type of XAI explanation (post-hoc feature list, post-hoc comparison visualization, or intrinsic decision tree) and (2) the objectivity of the assessed skills (soft skills vs. verifiable qualifications). The key outcome variable is "overall acceptance," a composite measure combining intention to use, trust, and fairness perception. Published in *The DATA BASE for Advances in Information Systems*, Volume 55, Number 1, February 2024.

## Key Findings

- Providing any explanation significantly increases acceptance over a no-explanation baseline (all p < 0.001), replicating the general positive effect of transparency on AI acceptance in the HR/recruiting domain. (source: Fleiß et al._Mitigating algorithm aversion in recruiting.txt)
- Contrary to predictions from algorithm aversion theory, intrinsic explanations (decision trees) did not outperform post-hoc explanations. No significant difference was found between explanation types, suggesting that a full model-level understanding is not necessary and may be difficult to achieve in first-encounter situations. (source: Fleiß et al._Mitigating algorithm aversion in recruiting.txt)
- Explanations based on verifiable qualifications (work experience, English proficiency, computer knowledge) produced significantly higher acceptance than explanations based on soft skills (teamwork, communication, diligence), across all explanation types. This is consistent with task-technology fit theory and prior HR research on standardized testing. (source: Fleiß et al._Mitigating algorithm aversion in recruiting.txt)
- The study concludes that XAI is not a "one-size-fits-all" approach: contextual factors of the decision problem (data objectivity) are more important determinants of explanation effectiveness than the technical form of the explanation. (source: Fleiß et al._Mitigating algorithm aversion in recruiting.txt)
- General trust in AI (not affinity for technology) was the strongest individual-level predictor of acceptance (coefficient 0.669, p < 0.001). Age had a small negative effect. (source: Fleiß et al._Mitigating algorithm aversion in recruiting.txt)

## Transparency Constructs

The paper operationalizes transparency through three XAI conditions:

- **Post-hoc feature list (EXPLAIN_LIST)**: Names the three criteria most relevant to the rejection decision — an instance of [[explainability]] via feature attribution.
- **Post-hoc comparison visualization (EXPLAIN_COMPARE)**: Displays the applicant's scores on three criteria alongside average scores of other applicants, adding a comparative context.
- **Intrinsic model explanation (EXPLAIN_INTERPRET)**: Shows a simple decision tree whose path leading to the rejection is highlighted, constituting [[algorithmic-transparency]] at the model level.

The study draws on Rudin's (2019) distinction between inherently interpretable models and post-hoc explanations of black-box models. The baseline (no explanation) represents [[algorithmic-transparency]] at its lowest; all three treatment conditions represent increasing levels of [[outcome-transparency]] and, in the intrinsic case, [[process-transparency]].

## Trust Constructs

Trust is operationalized as a single item within the overall acceptance scale ("Do you trust the chatbot decision just described?"), alongside intention to use and fairness perception. This captures a dimension of [[cognitive-trust]] (belief-based judgement of the CA's reliability) and [[behavioural-trust]] (intention to choose the CA, willingness to apply). General dispositional trust in AI was measured as a control via the Jian et al. (2000) scale.

The construct of [[algorithm-aversion]] is central: the paper frames low acceptance of the no-explanation condition as algorithm aversion and tests whether XAI reduces it.

## Relevance to Research Questions

**RQ1**: The paper operationalizes transparency via three distinct XAI types (list, comparison, decision tree) and acceptance via a composite measure including trust and fairness — illustrating how transparency constructs can be decomposed and operationalized in a high-stakes HR context. It also operationalizes algorithm aversion as a driver of low trust.

**RQ2**: The study documents a clear positive effect of XAI on acceptance (H1 supported), a null effect for explanation type (H2 not supported), and a significant conditional effect of decision objectivity on explanation effectiveness (H3 supported). This is a conditional effect: XAI benefits depend on the nature of the decision content, not the form of explanation. The non-linear pattern — where all explanation types cluster together but the soft/verifiable distinction creates two clear clusters — is a nuanced contribution to understanding when transparency increases trust.

**RQ3**: The study does not explicitly manipulate user expertise, but it measures general trust in AI and affinity for technology as individual-difference controls. It implicitly speaks to RQ3 by showing that the characteristics of the decision (task objectivity) moderate explanation effects more than individual-level technological characteristics. The authors suggest future work on tailoring explanations to cognitive styles.

## Related pages

- [[algorithm-aversion]]
- [[algorithmic-transparency]]
- [[explainability]]
- [[behavioural-trust]]
- [[cognitive-trust]]
- [[user-expertise]]
- [[domain-context]]
- [[rq2-relationships]]
