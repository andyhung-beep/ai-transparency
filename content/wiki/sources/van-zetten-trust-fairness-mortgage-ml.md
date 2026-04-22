# Increasing Trust and Fairness in Machine Learning Applications within the Mortgage Industry

**Source file**: [Original article](../../raw/van Zetten et al._Increasing trust and fairness in machine learning applications within the mortgage industry.pdf)

**Summary**: A research-by-design case study at a Dutch financial institution that developed and evaluated two XAI prototype systems (local and global interpretability) for a mortgage fraud detection ML model, finding statistically significant improvements in trust, usability, and fairness processes among daily users and compliance stakeholders.

**Sources**: van Zetten et al._Increasing trust and fairness in machine learning applications within the mortgage industry.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Published in *Machine Learning with Applications* (Vol. 10, 2022, article 100406), this paper by W. van Zetten, G.J. Ramackers, and H.H. Hoos (Leiden University) reports a practical implementation and evaluation study of explainable AI techniques in a real-world financial institution — a large Dutch insurer/mortgage provider.

The study developed two XAI systems:

- **MLX1** (local interpretability): Uses SHAP (TreeSHAP) and Anchor to generate textual explanations for individual mortgage applications classified as fraud risks. Deployed to 11 daily mortgage application reviewers who previously used a 22-rule hand-crafted explanation system.
- **MLX2** (global interpretability + bias detection): Uses the What If? tool, BlackBoxAuditing, and Aequitas (a bias/fairness audit toolkit) to provide data scientists, legal, risk, and compliance officers with global model insights and demographic bias detection. Tested with CBS (Dutch Statistics Office) data on migration background.

The study was motivated by: (1) EU ethical AI guidelines (High-Level Expert Group on AI, European Commission); (2) the Dutch Ethical Framework for Insurers (30 guidelines); and (3) GDPR requirements. The organisation's existing 75-feature tree-ensemble fraud model used an opaque, limited rule-based explanation system that only covered 22 of 75 features.

## Key Findings

- MLX1 produced a statistically significant overall improvement in user experience (trust, explanation satisfaction, perceived performance) compared to the rule-based baseline (t-test: t-value = 2.58, p = 0.014). [domain: financial services / mortgage fraud detection, Netherlands]
- 10 of 11 mortgage reviewers reported that MLX1 gave better guidance on what to investigate first, improving quality and saving time; median agreement on trust and explanation satisfaction statements was "Agree". [domain: financial services, Netherlands]
- Reviewers reported that extra insights into the model's decision process increased trust; however, the authors caution that higher detail may lead reviewers to blindly follow model decisions, undermining required human oversight. [domain: financial services, Netherlands]
- MLX2 (Aequitas component) successfully enabled detection of demographic bias based on migration background using false positive rate (FPR) disparity — no Dutch insurer had previously done this quantitatively. [domain: financial services, Netherlands]
- Data scientists rated "clear work instructions" as the most important MLX2 improvement (average importance 4.5/5), suggesting that operationalising XAI tools requires extensive onboarding support. [domain: financial services, Netherlands]
- Both MLX1 and MLX2 helped the organisation adhere to multiple guidelines in the Dutch Ethical Framework for Insurers (including transparency, non-discrimination, human oversight, and accountability). [domain: financial services / regulatory, Netherlands]
- A key design tension emerged: the most informative variant of MLX1 (including context-based thresholds like "above average") was rejected by the department manager as too suggestive and potentially compromising reviewer independence. [domain: financial services, Netherlands]
- The paper warns that excessive reliance on detailed XAI outputs can risk "automation bias" — reviewers may defer to the model if they perceive it as more knowledgeable than it is. [domain: financial services, Netherlands]

## Transparency Constructs

The paper implements and evaluates multiple distinct transparency constructs:

- **[[explainability]]** (local): SHAP-based feature importance for individual mortgage applications; textual, feature-by-feature explanations ranked by impact.
- **[[algorithmic-transparency]]** (global): What If? tool and BlackBoxAuditing for model-level interpretability; feature importance rankings.
- **[[outcome-transparency]]**: The explanation shows reviewers which features drove the fraud risk score for a specific case.
- **[[process-transparency]]**: MLX2 provides insight into overall model logic and decision processes for compliance and model governance.
- **Fairness/bias transparency**: Aequitas quantifies demographic group disparities (FPR parity by migration background), making model bias visible and measurable.

The study explicitly distinguishes local interpretability (MLX1: case-level explanations for daily users) from global interpretability (MLX2: model-level transparency for data scientists and compliance officers).

## Trust Constructs

- **[[cognitive-trust]]**: Measured via Hoffman et al.'s (2018) Trust Scale (3 items on confidence in the model, predictability, reliability, believability). MLX1 significantly improved cognitive trust.
- **[[behavioural-trust]]** (reliance): Proxied by reviewers' reported improvement in decision speed and quality; intent to use the explanation in assessments.
- **[[institutional-trust]]**: MLX2 builds organisational-level trust by enabling audit-trail documentation (PID/Project Initiation Document) and demonstrable compliance with ethical guidelines.
- **[[appropriate-reliance]]**: A central concern — the paper repeatedly warns that higher trust/explanation detail must be balanced against the risk of reviewers over-relying on model output and undermining human oversight.
- **[[trust-calibration]]**: Implicit in the design of MLX1 (reviewer retains final decision authority; explanation is an input, not a directive).

## Relevance to Research Questions

**RQ1**: Operationalises trust using an adapted version of Hoffman et al.'s (2018) metrics (trust, explanation satisfaction, perceived performance). Distinguishes local and global transparency as different operationalisations with different stakeholder targets (daily users vs. governance roles). (source: van Zetten et al._Increasing trust and fairness in machine learning applications within the mortgage industry.txt)

**RQ2**: Demonstrates a positive causal effect of adding XAI functionality on trust (statistically significant, p = 0.014). Critically, identifies a risk of over-trust: more detailed explanation may increase trust beyond what is warranted, potentially leading reviewers to copy model decisions uncritically. This "trust inflation" risk qualifies the transparency–trust positive relationship. [domain: financial services / mortgage, Netherlands] (source: van Zetten et al._Increasing trust and fairness in machine learning applications within the mortgage industry.txt)

**RQ3**: Distinguishes different user roles explicitly: (a) **daily mortgage reviewers** (MLX1) — non-expert ML users who need local, case-level explanations; (b) **data scientists** (MLX2 technical component) — require global feature importance and bias metrics; (c) **legal/compliance/risk officers** (MLX2 Aequitas component) — need visualised, auditable fairness metrics. Trust effects and information needs differ by role. (source: van Zetten et al._Increasing trust and fairness in machine learning applications within the mortgage industry.txt)

## Related pages

- [[explainability]]
- [[algorithmic-transparency]]
- [[cognitive-trust]]
- [[institutional-trust]]
- [[appropriate-reliance]]
- [[trust-calibration]]
- [[user-expertise]]
- [[domain-context]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]
- [[rq3-user-roles]]
