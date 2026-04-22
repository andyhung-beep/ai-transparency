# Towards Trustworthy AI-Enabled Decision Support Systems: Validation of the Multisource AI Scorecard Table (MAST)

**Source file**: [Original article](../../raw/Salehi et al._Towards trustworthy AI-enabled decision support systems.pdf)

**Summary**: This validation study tests whether the Multisource AI Scorecard Table (MAST) — a nine-criterion checklist derived from U.S. Intelligence Community tradecraft standards — can reliably distinguish high from low trustworthy AI decision support systems, finding strong associations between MAST ratings and trust perceptions across two high-stakes expert domains (airport security screening and intelligence analysis).

**Sources**: Salehi et al._Towards trustworthy AI-enabled decision support systems.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Salehi et al. (2024, *Journal of Artificial Intelligence Research*) present a validation study for MAST (the Multisource AI Scorecard Table), a structured checklist that operationalizes nine criteria for trustworthy AI systems derived from Intelligence Community Directive (ICD) 203: sourcing, uncertainty, distinguishing, analysis of alternatives, customer relevance, logic, change, accuracy, and visualization.

The study develops two AI-DSS testbeds to compare High-MAST and Low-MAST system versions:
- **Facewise**: A face-recognition identity-verification system used by airport Transportation Security Officers (TSOs). N = 146 TSOs (73 per condition).
- **READIT**: A text-summarization and data visualization system for intelligence analysts (REporting Assistant for Defense and Intelligence Tasks). N = 23 DHS intelligence analysts (11/12 per condition).

Both High- and Low-MAST versions of each platform were designed to have equivalent usability and engagement to isolate the MAST criteria as the manipulation. Outcome variables included: MAST criteria ratings, trust (Jian et al., 2000; Chancey et al., 2017), credibility, perceived risk, perceived benefit, usability (SUS), engagement, and objective task performance.

The domain spans national security / airport security screening and intelligence analysis.

## Key Findings

- High-MAST versions of Facewise received significantly higher ratings on all 9 MAST criteria. MAST-total was positively associated with trust (Jian: β = 0.1, R² = 0.31; Chancey: β = 0.12, R² = 0.37), credibility (β = 0.11, R² = 0.30), and perceived benefit (β = 0.091, R² = 0.33), and negatively with perceived risk (β = –0.067, R² = 0.14). [Domain: airport security]
- High-MAST Facewise was rated significantly more trustworthy (Jian et al., p = 0.023) and less risky (p = 0.021) and more beneficial (p = 0.031) than Low-MAST Facewise. No significant difference in credibility or in objective performance accuracy was found between the conditions. [Domain: airport security]
- PCA for Facewise showed that the first two principal components explained 84% of variance in perception metrics. The first PC — representing an overall positive perception average (trust + benefit + credibility, inversely weighted for risk) — was significantly predicted by MAST-total (R² = 0.41). [Domain: airport security]
- For READIT, High-MAST reached significantly higher scores on 6 of 9 MAST criteria (all except uncertainty, relevance, and visualization). MAST-total positively predicted trust (R² = 0.58–0.61) and credibility (R² = 0.70), and negatively predicted risk (R² = 0.52). PCA explained 87.65% of variance, with MAST-total predicting first PC (R² = 0.74). [Domain: intelligence analysis]
- No significant differences in objective task performance (identification accuracy for Facewise; report quality score for READIT) were found between High-MAST and Low-MAST conditions in either platform. Higher MAST and higher trust did not translate to better human-AI performance. [Domain: airport security and intelligence analysis]
- The Jian et al. (2000) trust questionnaire showed significant between-condition differences for Facewise but not READIT; the Chancey et al. (2017) questionnaire showed significant differences only on the "purpose" dimension for READIT. Item valence (mixed vs. all positive) may explain discrepant results between these two trust instruments. [Domain: airport security and intelligence analysis]
- No significant between-condition differences in usability (SUS) or engagement were found for either platform, confirming that these factors were successfully held constant as potential confounds. [Domain: airport security and intelligence analysis]
- High-MAST TSOs spent significantly more time on the Facewise task without corresponding accuracy gains, suggesting that richer information may increase cognitive load without improving decisions. [Domain: airport security]

## Transparency Constructs

MAST embeds multiple transparency-related criteria:

- **Sourcing** (RQ criterion 1): Can the system identify underlying data sources and training methodology? [Aligns with [[algorithmic-transparency]]]
- **Uncertainty** (criterion 2): Can the system indicate and explain uncertainty in its outputs? [Aligns with [[uncertainty-visualization]]]
- **Distinguishing** (criterion 3): Can the system clearly distinguish derived results from underlying data? [Aligns with [[process-transparency]]]
- **Analysis of Alternatives** (criterion 4): Can the system identify and assess alternative results? [Aligns with [[counterfactual-explanations]] and reasoning transparency]
- **Customer Relevance** (criterion 5): Does the system present information in a user-relevant way? [Aligns with user-centered explainability design]
- **Logic** (criterion 6): Can the system help the user understand how it derived its results? [Aligns with [[explainability]]]
- **Change** (criterion 7): Can the system indicate consistency or change from prior analyses? [Aligns with longitudinal transparency]
- **Accuracy** (criterion 8): Does the system communicate the accuracy of its judgments? [Aligns with calibration disclosure]
- **Visualization** (criterion 9): Does the system use appropriate visual displays to enhance understanding? [Aligns with [[uncertainty-visualization]] and interface design]

MAST thus constitutes a multi-dimensional operationalization of transparency, covering process, output, uncertainty, source, and visual dimensions. This is broader than most individual XAI studies, which typically focus on a single transparency technique.

## Trust Constructs

The study measures trust using two validated instruments:

1. **Jian et al. (2000)**: A 12-item scale measuring general trust perceptions of automation, with both positively and negatively valenced items (e.g., "I can trust the system"; "The system looks deceptive"). Scale range 1-7.
2. **Chancey et al. (2017)**: A 15-item scale decomposing trust into three theoretically grounded dimensions: purpose trust (belief the system will help achieve goals), process trust (belief in system reliability), and performance trust (belief in output accuracy). All positively valenced.

The study also measures message credibility (Appelman & Sundar, 2016), perceived risk, and perceived benefit as trust-adjacent constructs. This combination allows cross-validation between different trust operationalizations and reveals that item valence affects results — negatively valenced items (Jian scale) produced significant differences where the all-positive Chancey scale did not for Facewise; the opposite pattern appeared for READIT.

MAST ratings were highly correlated with both trust instruments, supporting MAST's construct validity as a proxy for trustworthiness-related perceptions. However, the critical finding is that MAST/trust perceptions and [[trust-calibration]] (appropriate trust relative to actual system reliability) are distinct: high MAST ratings did not yield better performance.

## Relevance to Research Questions

**RQ1**: MAST provides a practitioner-oriented, multi-dimensional operationalization of AI trustworthiness that is conceptually distinct from but empirically related to trust perceptions. The study demonstrates that trust and trustworthiness should not be conflated: MAST ratings capture perceived trustworthiness properties, while actual reliability (performance) is a separate dimension. This distinction is central to the trust calibration literature and [[rq1-conceptualizations]]. The study also contributes by cross-validating two trust measurement instruments (Jian et al., Chancey et al.) and finding meaningful differences in their sensitivity, with implications for survey instrument selection (source: Salehi et al._Towards trustworthy AI-enabled decision support systems.txt).

**RQ2**: Strong positive associations between MAST-total and trust perceptions (R² = 0.31-0.61 across platforms and instruments) support the view that transparency-enhancing design features causally influence users' trust perceptions. The null performance result — high MAST does not yield better performance — replicates a broader pattern in the literature that trust perceptions and objective performance gains from AI transparency are dissociable. This has direct implications for the [[rq2-relationships]] question of whether transparency-trust effects translate to behavioral outcomes (source: Salehi et al._Towards trustworthy AI-enabled decision support systems.txt).

**RQ3**: All participants are domain experts (Transportation Security Officers; DHS Intelligence Analysts). The study does not vary expertise level within samples, but the Facewise TSO sample shows that even highly experienced security specialists show expected MAST-trust associations. The READIT intelligence analyst sample is too small for subgroup analysis but provides a proof of concept for MAST use with a different expert population. The study notes that expert communities may define trustworthiness differently depending on their domain priorities, which is relevant to how user role should be considered in transparency-trust research (source: Salehi et al._Towards trustworthy AI-enabled decision support systems.txt).

## Related pages

- [[algorithmic-transparency]]
- [[uncertainty-visualization]]
- [[process-transparency]]
- [[explainability]]
- [[cognitive-trust]]
- [[trust-calibration]]
- [[appropriate-reliance]]
- [[institutional-trust]]
- [[domain-context]]
- [[user-expertise]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]
