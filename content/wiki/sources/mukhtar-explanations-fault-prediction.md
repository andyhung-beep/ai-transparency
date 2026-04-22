# Explaining Software Fault Predictions to Spreadsheet Users

**Source file**: [Original article](../../raw/Mukhtar et al._Explain software fault predictions to spreadsheet users.pdf)

**Summary**: A between-subjects user study (N = 120) comparing four explanation styles for a machine-learning-based spreadsheet fault prediction tool finds that well-designed natural language explanations most effectively improve user understanding and trust, while visualization-based explanations (LIME-style feature importance) perform no better than — and sometimes worse than — providing no explanation at all.

**Sources**: Mukhtar et al._Explain software fault predictions to spreadsheet users.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Mukhtar, Hofer, Jannach, and Wotawa (2023, Journal of Systems & Software) investigate how different forms of explanation for a machine-learning-based fault prediction tool affect spreadsheet users' ability to understand which cells are flagged as suspicious, and their trust and satisfaction with the tool. The study addresses a gap in XAI research: most work focuses on what makes explanations technically faithful, not how end-users perceive and trust them.

The tool evaluated is SmellChecker, a metric-based ML fault prediction system for spreadsheets. The study uses a real-world Enron Error corpus spreadsheet with three faulty cells (a range error, a double fault, and another range error). Participants were recruited via Prolific and screened for spreadsheet experience; over half had more than 7 years of experience and used spreadsheets daily.

A between-subjects design with N = 120 participants compared four conditions:
1. **Blackbox**: ranked list of suspicious cells only (no explanation)
2. **Visualization**: LIME-based feature importance chart
3. **NaturalLanguage**: LIME features translated into plain English sentences (e.g., "References to cells that are to the left or above this cell may be missing.")
4. **HumanExplanation**: manually crafted expert explanation (upper bound)

The domain is **software engineering / developer tooling**.

## Key Findings

- Natural language explanations significantly improved fault comprehension over the Blackbox condition. Average comprehension score across three faulty cells: HumanExplanation = 1.83/2, NaturalLanguage = 1.58/2, Blackbox = 1.40/2, Visualization = 1.12/2. (Domain: software engineering)
- Visualization-based explanations (LIME feature importance charts) performed worse than even the Blackbox condition on fault comprehension (1.12 vs. 1.40 out of 2). Qualitative review suggested participants misinterpreted feature importance values, and the visualization may have distracted them from the fault localization task. (Domain: software engineering)
- ANOVA analysis confirmed significant differences between explanation styles on fault comprehension measures.
- On trust and confidence (5-point Likert scales, TC1 "explanations are trustworthy" and TC2 "overall, I trust SmellChecker"), the HumanExplanation group scored highest (TC1 = 4.47, TC2 = 4.27), followed by NaturalLanguage (TC1 = 4.07, TC2 = 4.23), then Blackbox (TC1 = 4.07, TC2 = 3.87), then Visualization (TC1 = 3.50, TC2 = 3.57). Natural language explanations achieved similar trust levels to the blackbox baseline, with the human explanation as upper bound.
- Behavioral intentions (intention to use, I1 "would use again") followed the same pattern: HumanExplanation = 4.13, NaturalLanguage = 3.70, Blackbox = 3.13, Visualization = 2.90. Recommendation intentions (R1) were similarly ordered.
- Satisfaction scores were highest in the HumanExplanation condition and lowest in the Visualization condition.
- The study finds strong evidence that providing explanations for ML fault prediction outcomes can improve the perceived quality and usefulness of such tools, supporting the broader claim that adoption of AI-fueled technology may depend on a system's ability to explain its decisions.

## Transparency Constructs

The paper operationalizes transparency through a single questionnaire item T1: "I understand why the cells were marked suspicious through the explanations" (1–5 Likert). This reflects **outcome transparency** (understanding why specific outputs were produced; see [[outcome-transparency]]). The natural language explanations and human explanations also provide a degree of **process transparency** by describing the reasoning behind suspicious cell classifications ([[process-transparency]]).

The paper contrasts four types of explanation:
- Black-box output (no transparency)
- Visual feature importance (partially interpretable [[explainability]])
- Natural language feature descriptions ([[natural-language-explanations]])
- Human-authored explanations (ideal-case transparency)

The finding that visualizations of LIME feature importance did not improve understanding — and reduced it — is an important counterpoint to the assumption that any explanation improves transparency. It highlights that the form and comprehensibility of explanations matter as much as their presence.

## Trust Constructs

Trust is measured via two Likert items: TC1 (trustworthiness of explanations) and TC2 (overall trust in the tool). These map onto [[cognitive-trust]] — belief that the system is reliable and competent. Behavioral intentions to reuse or recommend the tool reflect [[behavioural-trust]].

The study finds that trust in the explanation system is highest when explanations are understandable (natural language or human-authored), supporting the idea that explanation comprehensibility drives cognitive trust rather than explanation presence alone.

## Relevance to Research Questions

**RQ1**: Provides operationalizations of both transparency (perceived understanding via T1 item) and trust (Likert-scale cognitive trust items TC1, TC2) in the software engineering domain. Demonstrates that these constructs can be measured in a non-expert user study context. Contributes to understanding how explanation form affects transparency perceptions.

**RQ2**: Key finding for RQ2: explanation type has a non-monotonic relationship with trust and understanding. Adding a visualization explanation decreases both comprehension and trust relative to no explanation, while natural language explanations improve them. This is strong evidence that the form of transparency can matter as much as its presence — and that poorly designed transparency tools can harm trust. Contributes to understanding conditional and potentially negative effects in the transparency–trust relationship.

**RQ3**: The study sample consists of experienced spreadsheet users (>50% with 7+ years experience, daily users), making this a study of domain-knowledgeable end-users rather than novices or experts. This positions findings in the "intermediate expertise" space for spreadsheet debugging. The differential performance of visualization vs. natural language across participants suggests that explanation form interacts with users' cognitive capabilities and familiarity with data visualization conventions, a finding relevant to [[user-expertise]] moderating effects.

## Related pages

- [[natural-language-explanations]]
- [[explainability]]
- [[outcome-transparency]]
- [[cognitive-trust]]
- [[behavioural-trust]]
- [[user-expertise]]
- [[rq2-relationships]]
