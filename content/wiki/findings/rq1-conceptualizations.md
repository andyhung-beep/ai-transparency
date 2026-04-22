# RQ1: How Transparency and Trust Have Been Conceptualized and Operationalized

**Summary**: This page synthesizes how AI transparency and user trust are defined and measured across the 86 sources in this corpus, identifying the range of constructs used, key conceptual distinctions, and gaps in operationalization.

**Sources**: All 86 source documents.

**Research questions addressed**: RQ1

**Last updated**: 2026-04-18

---

## Overview

Research Question 1 asks: *How have AI transparency and user trust been conceptualized and operationalized across domains?*

The corpus reveals remarkable diversity in construct definitions and measurement approaches, with limited standardization across domains or research communities. This diversity reflects genuine theoretical disagreement as well as domain-specific requirements.

---

## Transparency Constructs

### Post-hoc Explanation Methods

The most common transparency operationalization is a specific post-hoc explanation technique applied as an experimental manipulation. Key methods appearing across the corpus:

| Method | Description | Representative sources |
|---|---|---|
| SHAP | Feature importance attributed via Shapley values; local and global | Wang & Ding; van Zetten; Rezaeian; Salehi; La Gatta (PASTLE); Karagoz |
| LIME | Local approximation by interpretable surrogate | Mukhtar; Okolo; Humer; La Gatta; Weitz |
| Grad-CAM / saliency | Gradient-based visual attribution for image models | Humer; Ihongbe; Leichtmann; Karran |
| Counterfactual | What-if contrastive explanations | Lee & Chew; Naiseh (classes); Suffian ×2; Woodcock; Mourali |
| Anchors | Rule-based local explanations | Cau & Spano; La Gatta |
| DiCE | Diverse counterfactual explanations | Suffian ×2 |
| Example-based | Nearest-neighbour or prototype cases | Perlmutter; Humer; Naiseh; Angerschmid |
| Rule lists | Decision trees, if-then rules | Galanti; Kornowicz; Jaziri |
| Natural language | Free-text rationales | Mukhtar; Brand; Li; Weitz; Woodcock; Lim |

Most studies test a small number of methods (1–4) in controlled experiments. Cross-method comparisons within the same study are rare, making it difficult to draw general conclusions about relative effectiveness.

### Structural/Design-Level Transparency

A smaller number of papers operationalize transparency at the level of system design rather than explanation output:

- **Automation transparency levels** (SAT model): Level 1 (what the system perceives), Level 2 (what it will do), Level 3 (projected outcomes) — used by Bhaskara, Tatasciore series, Vered.
- **Demand-driven vs. sequential transparency**: user control over information access (Vered et al.).
- **Interpretability-by-design**: fuzzy logic classifiers, decision trees (Yeganejou; Gunning & Aha).
- **Explanation timing**: before vs. after AI action (Du et al.).
- **Explanation depth**: number of features shown, levels of detail (Rezaeian; Conijn; Karran morphological clarity).

### Novel Constructs

Several papers introduce transparency-adjacent constructs not captured by the standard explainability taxonomy:

| Construct | Definition | Source |
|---|---|---|
| [[causability|Causability]] | User-side ability to reach causal understanding | Shin 2021 |
| [[traceability|Traceability]] / SIPA | Subjective experience of following AI processing | Schrills & Franke 2023 |
| Meaningful explanation | Tailored transparency designed for specific user mental models | Larasati et al. 2023 |
| Placebic transparency | Disclosure that appears informative but is not actionable | Liu 2021 |
| Learning to Defer (LtD) | AI explicitly signals when to delegate to human | Sajno et al. |

---

## Trust Constructs

### Taxonomy of Trust Dimensions

| Trust type | Definition | Key measurement approaches |
|---|---|---|
| [[cognitive-trust|Cognitive trust]] | Judgment-based assessment of competence and reliability | Jian et al. (2000); Madsen & Gregor; Körber TiA scale |
| [[affective-trust|Affective trust]] | Emotion-based bonds; feelings of security and care | Emotion scales; working alliance (Nelekar); single items |
| [[behavioural-trust|Behavioural trust]] | Reliance, adoption, override, advice-following | Agreement rates; override rates; WoA; delegation frequency |
| [[institutional-trust|Institutional trust]] | Trust in deploying organisations or regulatory systems | Policy support; general government trust scales |
| [[algorithmic-trust|Algorithmic trust]] | Dispositional trust in AI/algorithmic systems | General AI attitude scales; Liu (2021) |
| [[trust-calibration|Trust calibration]] | Alignment between subjective trust and actual AI reliability | d'; DoR metric; self-report vs. accuracy comparison |
| Metacognitive calibration | Alignment between confidence in own judgments and performance | Confidence elicitation + performance scoring (von Zahn) |

### Key Conceptual Distinctions

Several papers make distinctions that are often collapsed in single-measure studies:

1. **Trust ≠ acceptance ≠ reliance**: Cramer et al. show that explanations increase recommendation acceptance without increasing system trust. Diprose et al. show explanations increase preference without changing behaviour. These three constructs must be measured separately (Cramer et al., 2008; Diprose et al., 2020).

2. **Explainability (system) ≠ causability (user)**: Shin (2021) distinguishes the system's capacity to explain from the user's capacity to understand causally. Both matter for trust, but through different mechanisms (Shin, 2021).

3. **Objective transparency ≠ subjective transparency**: Schrills & Franke show that experienced traceability (SIPA) diverges from actual comprehension and can become miscalibrated (Schrills & Franke, 2023).

4. **Self-reported trust ≠ behavioural trust**: Wang & Ding (2024), Kornowicz & Thommes (2025), Suffian et al. (2025), and Rezaeian et al. (2025) all document significant dissociations between trust ratings and reliance/performance measures [NEEDS SOURCE for each].

5. **Trust in AI system ≠ trust in human AI user**: Schilke & Reimann uniquely study how AI *disclosure by the human user* affects interpersonal trust in the disclosing person — not trust in the AI (Schilke & Reimann, 2025).

---

## Cross-Domain Patterns

### Measurement Standardization

There is little standardization of transparency or trust measures across domains. Healthcare studies use clinical decision tasks and domain-specific accuracy metrics; recommender system studies use acceptance rates and satisfaction scales; unmanned vehicle studies use signal detection measures. This fragmentation makes cross-domain meta-analysis difficult.

### Outcome Measures Used

Among behavioural trust measures, the most commonly used are:
1. Reliance/agreement rate (frequency of following AI advice)
2. Decision accuracy (whether the human-AI team produced correct decisions)
3. Adoption intention (self-reported likelihood of future use)

Among subjective trust measures:
1. Jian et al. (2000) scale — most widely used
2. Domain-adapted trust scales (TiA, Madsen & Gregor)
3. Single-item trust ratings

---

## Gaps and Contradictions

1. **Conflation of trust types**: Many studies measure a single "trust" variable without specifying whether it is cognitive, affective, or behavioural, preventing interpretation of mechanisms.
2. **Absence of affective trust measurement**: Affective trust is measured in only a handful of studies (Bernardo & Seva; Suen & Hung) despite theoretical arguments for its importance.
3. **Underspecification of transparency type**: Several papers use generic "explanation" manipulations without specifying or justifying the method.
4. **Self-report dominance**: Most trust measurement is self-report; implicit, physiological, or behavioural measures are rare (exceptions: Schrills & Franke with SIPA; Sun et al. with eye-tracking and physiological signals; Karran et al. with pupillometry).
5. **Limited longitudinal measurement**: Trust is almost always measured in a single session. The few longitudinal studies (Jansen et al. 3-day; Schrills & Franke) show different patterns from cross-sectional research.

---

## Summary Table: Key Papers by Contribution to RQ1

| Source                     | Contribution                                                               |
| -------------------------- | -------------------------------------------------------------------------- |
| Gunning & Aha (2019)       | Taxonomy of XAI approaches and psychological framework for transparency    |
| Shin (2021)                | Causability vs. explainability distinction; dual-process model             |
| Cramer et al. (2008)       | Trust vs. acceptance distinction in recommender systems                    |
| Naiseh et al. C-XAI (2024) | Framework linking XAI technical properties to trust calibration design     |
| Tintarev & Masthoff (2012) | Seven explanation aims taxonomy (transparency, effectiveness, trust, etc.) |
| Schrills & Franke (2023)   | SIPA / traceability construct; objective vs. subjective transparency       |
| Salehi et al. (2024)       | MAST framework; multi-criterion trustworthiness operationalization         |
| Park et al. (2023)         | 9-factor AI UX framework including causality and explainability            |
| Bernardo & Seva (2023)     | XAITC model; affective trust pathway                                       |
| Liu (2021)                 | Real vs. placebic transparency distinction                                 |
| Schilke & Reimann (2025)   | Disclosure as transparency; interpersonal trust outcome                    |
| Wang & Ding (2024)         | Behavioural vs. self-reported trust dissociation                           |

---

## Related pages

- [[explainability]]
- [[causability]]
- [[traceability]]
- [[cognitive-trust]]
- [[affective-trust]]
- [[behavioural-trust]]
- [[trust-calibration]]
- [[rq2-relationships]]
- [[rq3-user-roles]]

## References

Cramer, H., Evers, V., Ramlal, S., Van Someren, M., Rutledge, L., Stash, N., Aroyo, L., & Wielinga, B. (2008). The effects of transparency on trust in and acceptance of a content-based art recommender. *User Modeling and User-Adapted Interaction*, 18(5), 455–496 [details TBD].

Diprose, J. P., Buist, N., Chu, N., Edlin, R., Milinovich, A., & Nunns, M. (2020). Physician understanding, explainability, and trust in a hypothetical machine learning risk calculator. *Journal of the American Medical Informatics Association*, 27(4), 592–600 [details TBD].

Kornowicz, J., & Thommes, K. (2025). Algorithm, expert, or both? Determinants of algorithm adoption in managerial decision-making. *Journal of Behavioral Decision Making* [details TBD].

Rezaeian, A., Asan, O., & Bayrak, A. E. (2025). The impact of AI explanations on clinicians' trust and diagnostic accuracy in breast cancer. *Applied Ergonomics* [details TBD].

Schilke, O., & Reimann, M. (2025). The transparency dilemma: How AI disclosure erodes trust. *Organizational Behavior and Human Decision Processes* [details TBD].

Schrills, T., & Franke, T. (2023). How do users experience traceability of AI systems? Examining subjective information processing awareness in automated insulin delivery (AID) systems. *ACM Transactions on Interactive Intelligent Systems*, 13(4).

Shin, D. (2021). The effects of explainability and causability on perception, trust, and acceptance: Implications for explainable AI. *International Journal of Human-Computer Studies*, 146, 102551.

Suffian, M., Panigutti, C., Ntoutsi, E., Pedreschi, D., & Giannotti, F. (2025). The role of user feedback in enhancing understanding and trust in counterfactual explanations for explainable AI. *International Journal of Human-Computer Studies* [details TBD].

Wang, D., & Ding, Y. (2024). The rationality of explanation or human capacity? A study of human-AI collaboration in clinical decision support. *Journal of the American Medical Informatics Association* [details TBD].
