# Meaningful Explanation Effect on User's Trust in an AI Medical System: Designing Explanations for Non-Expert Users

**Source file**: [Original article](../../raw/Larasati et al._Meaningful explanation effect on user_s trust in an AI medical system.pdf)

**Summary**: Using a participatory, stage-based design process involving AI experts, medical professionals, and lay users, this paper proposes 14 explanation design guidelines for AI healthcare systems and a working prototype (CARE) for breast cancer self-assessment, then evaluates their effect on non-expert users' trust; meaningful explanations reduced extreme trust responses (both overtrust and distrust) and improved perceived technical competence.

**Sources**: Larasati et al._Meaningful explanation effect on user_s trust in an AI medical system.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Larasati, De Liddo, and Motta (2023), published in *ACM Transactions on Interactive Intelligent Systems*, address the gap between AI explanation research focused on experts and the practical need for explanations accessible to laypeople (patients, carers). The paper defines a **meaningful explanation** as one that is acceptable and understandable to the user — useful, relevant, accurate, complete, and clearly presented.

The methodology adapts Eiband et al.'s stage-based participatory design process across five stages in three phases:

1. **Explanation Models Development**: separate Expert Explanation Models (from 3 AI/ML practitioners and 3 junior medical doctors) and a User Explanation Model (from 12 lay users stratified by dispositional trust: 4 sceptics, 4 open-minded, 4 enthusiasts) are constructed, then integrated into a Target Explanation Model.
2. **Design Guidelines and Prototyping**: 14 Explanation Design Guidelines (EDGs) are derived and implemented in the CARE prototype — a web-based breast cancer thermography self-assessment system.
3. **Evaluation**: Two surveys (First: n = 55 from Mechanical Turk, within-subjects trust measurement before/after prototype interaction; Second: n = 88, with control group receiving no explanation) plus semi-structured interviews with 7 participants assess the guidelines and prototype.

The breast-cancer scenario was chosen because portable thermography devices enable self-managed assessment, making layperson-facing AI particularly salient.

## Key Findings

- The CARE prototype was rated as possessing meaningful explanation characteristics: Contrastive (median 6), Domain-independent (median 6), General (median 6), Truthful (median 6), Thorough (median 6), and Social (median 5) on a 7-point scale (domain: healthcare). (source: Larasati et al._Meaningful explanation effect on user_s trust in an AI medical system.txt)
- Within-subjects trust comparison (First Survey): significant differences in perceived reliability (p = .009), perceived technical competence (p = .001), personal attachment (p = .015), and helpfulness (p = .029) after prototype interaction; only perceived technical competence survived Bonferroni correction (p = .00148) (domain: healthcare). (source: Larasati et al._Meaningful explanation effect on user_s trust in an AI medical system.txt)
- The overall distribution of trust ratings moved toward the middle after interaction with the explanation prototype — both extreme overtrust and distrust decreased — suggesting that meaningful explanation promoted more calibrated trust rather than uniformly increasing it (domain: healthcare). (source: Larasati et al._Meaningful explanation effect on user_s trust in an AI medical system.txt)
- Self-reported trust (single global item) did not show a statistically significant change, suggesting multi-dimensional trust measurement is more sensitive than a single item (domain: healthcare). (source: Larasati et al._Meaningful explanation effect on user_s trust in an AI medical system.txt)
- All 14 Explanation Design Guideline components were rated as relevant or important (median 4–5 on 5-point scale) for users' understanding and trust (domain: healthcare). (source: Larasati et al._Meaningful explanation effect on user_s trust in an AI medical system.txt)
- System Output (EDG7: the AI prediction itself) received the highest relevance rating (mean 4.67); System Information (EDG4: technical details, accuracy, certifications) received the lowest (mean 4.11), consistent with experts' and users' lower interest in technical specifics (domain: healthcare). (source: Larasati et al._Meaningful explanation effect on user_s trust in an AI medical system.txt)
- The CARE prototype scored 81.34 on the System Usability Scale, in the "excellent usability" range (domain: healthcare). (source: Larasati et al._Meaningful explanation effect on user_s trust in an AI medical system.txt)
- Expert Explanation Models differed by expertise type: medical experts focused on disease information, treatment options, next steps, and empathetic delivery; AI experts focused on system inputs/outputs and process transparency, but explicitly doubted non-experts' interest in algorithmic details (domain: healthcare). (source: Larasati et al._Meaningful explanation effect on user_s trust in an AI medical system.txt)
- Lay users prioritised disease information, treatment, next steps, and empathy most highly; system process received lower ratings, corroborating AI experts' assessment that technical transparency is less salient to non-experts (domain: healthcare). (source: Larasati et al._Meaningful explanation effect on user_s trust in an AI medical system.txt)

## Transparency Constructs

The paper works with a broad conception of explanation that transcends algorithmic transparency:

- **Natural language explanations**: the CARE prototype delivers text-based explanations of disease information, treatment options, and AI output alongside visual elements.
- **Outcome transparency**: the AI's prediction (EDG7: System Output) and its confidence/accuracy (EDG4) are surfaced as critical explanation components.
- **Process transparency**: system process (EDG6) and system information (EDG4) are included but rated lower by lay users than by AI experts, suggesting a tension between expert-designed transparency and lay user needs.
- **Uncertainty visualization**: the prototype includes statements like "CARE is only 98% accurate" and "highly likely" qualifiers to communicate probabilistic uncertainty, supporting calibrated trust.
- **Counterfactual / contrastive elements**: input comparison visualisation (EDG13) enables users to compare their results to contrasting cases, functioning as a form of [[counterfactual-explanations]] or [[example-based-explanations]].
- **Causability**: disease information (EDG1) and system process (EDG6) together aim for what Holzinger defines as causability — making causal explanations understandable to the user in their context.

See [[explainability]], [[natural-language-explanations]], [[outcome-transparency]], [[process-transparency]], [[uncertainty-visualization]], [[causability]].

## Trust Constructs

The paper explicitly operationalises trust as a multi-dimensional construct using a validated Human-AI Trust in AI Healthcare scale (Jian et al. derivative, adapted), covering:

- **Perceived understandability**: cognitive trust component — did the user understand the system?
- **Perceived reliability**: cognitive/behavioural — will the system perform consistently?
- **Perceived technical competence**: cognitive — does the system have the required capabilities?
- **Faith**: affective — an optimistic expectation of system behaviour.
- **Personal attachment**: affective — emotional connection to the system.
- **Helpfulness**: functional/behavioural — does the system assist the user?
- **Institution credibility** and **user autonomy** (Second Survey refined scale).

The paper also operationalises **trust calibration**: by reducing extreme responses (overtrust and distrust), the meaningful explanation is argued to have promoted appropriate rather than inflated trust. This connects to [[trust-calibration]], [[cognitive-trust]], and [[affective-trust]].

Dispositional trust (trust propensity) is controlled by stratifying lay participants into sceptics, open-minded, and enthusiasts.

## Relevance to Research Questions

**RQ1**: The paper makes a substantial contribution to the operationalisation of both explanation and trust. It distinguishes meaningful explanation (layperson-adequate, understandable) from algorithmic explanation (technically faithful but potentially inaccessible), and proposes the first explanation model framework explicitly designed for non-expert users in healthcare. The 14 EDGs and three-model framework (Expert, User, Target Explanation Models) are themselves a theorisation of transparency constructs. Trust is operationalised multi-dimensionally. See [[rq1-conceptualizations]].

**RQ2**: The evaluation demonstrates that meaningful explanation produces more calibrated trust (reducing both overtrust and distrust) rather than monotonically increasing trust, which is an important non-linear finding. Perceived technical competence improved significantly, but self-reported overall trust and other metrics showed mixed results. The study also highlights that explanation effects differ by measurement instrument (multi-item vs. single item; objective performance vs. self-report). See [[rq2-relationships]].

**RQ3**: This is perhaps the most directly RQ3-relevant paper in the batch. The entire design process is structured around expertise differences: the Expert Explanation Model captures what AI/ML and medical professionals think should be explained, the User Explanation Model captures what laypeople want, and the Target Explanation Model bridges the two. The finding that non-experts are less interested in system-process details than AI experts assumed is a key empirical contribution about how user role shapes explanation needs and trust. See [[rq3-user-roles]].

## Related pages

- [[explainability]]
- [[natural-language-explanations]]
- [[cognitive-trust]]
- [[affective-trust]]
- [[trust-calibration]]
- [[user-expertise]]
- [[rq3-user-roles]]
