# Investigating Whether AI Will Replace Human Physicians and Understanding the Interplay of the Source of Consultation, Health-Related Stigma, and Explanations of Diagnoses on Patients' Evaluations of Medical Consultations

**Source file**: [Original article](../../raw/Guo & Chen_Investigating whether AI will replace human physicians.pdf)

**Summary**: A 3×2×2 randomized factorial experiment (n = 249) finding that patients functionally trust human physicians more than AI or human-involved AI for medical diagnosis, that health-related stigma does not drive AI preference even for stigmatized diseases, and that providing diagnosis explanations significantly improves functional, relational, and emotional evaluations of all three types of medical agents.

**Sources**: Guo & Chen_Investigating whether AI will replace human physicians.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Guo and Chen (2025), published in *Journal of Medical Internet Research* (vol. 27, e66760, doi: 10.2196/66760), conduct a within/between-subject factorial experiment manipulating three variables: (1) consultation source (autonomous AI vs. human-involved AI vs. human physician), (2) health-related stigma (AIDS — high stigma vs. heart disease — low stigma), and (3) diagnosis explanation (without vs. with explanation). The study measures patients' functional evaluations (source credibility, message credibility, persuasive effect), relational evaluations (perceived empathy, self-disclosure, psychological distance), and emotional evaluations (optimism, guilt). The study is grounded in algorithm aversion theory, machine heuristic theory, and the CASA paradigm, testing which framework best describes patient perceptions in medical contexts.

## Key Findings

- Human physicians were rated significantly higher than AI and human-involved AI on all three functional dimensions (source credibility, message credibility, persuasive effect; all p < .001), supporting algorithm aversion theory over machine heuristic in the medical domain. No significant difference was found between autonomous AI and human-involved AI. (source: Guo & Chen_Investigating whether AI will replace human physicians.txt; domain: healthcare)
- No significant differences across the three medical agents emerged on relational (perceived empathy, self-disclosure, psychological distance) or emotional (optimism, guilt) dimensions, suggesting that AI's relational and emotional presentation can match human physicians at current levels of anthropomorphism. (source: Guo & Chen_Investigating whether AI will replace human physicians.txt; domain: healthcare)
- Health-related stigma (AIDS vs. heart disease) did not significantly affect functional or relational evaluations or preferences for medical agent type, indicating that instrumental diagnostic needs override privacy concerns even for highly stigmatized conditions. (source: Guo & Chen_Investigating whether AI will replace human physicians.txt; domain: healthcare)
- Providing a diagnosis explanation significantly improved all functional and relational evaluations and both emotional outcomes (all p < .05 or better) for all three medical agent types, demonstrating a broad, cross-agent benefit of transparency. (source: Guo & Chen_Investigating whether AI will replace human physicians.txt; domain: healthcare)
- An interaction effect emerged: when explanations were provided, participants perceived significantly more empathy from the human physician than from AI or human-involved AI (p = .001 and p = .003 respectively). Without explanation, no empathy difference existed between agents. (source: Guo & Chen_Investigating whether AI will replace human physicians.txt; domain: healthcare)
- A further interaction between stigma and diagnosis explanation revealed that for unexplained diagnoses, AIDS patients rated source credibility higher than heart disease patients — suggesting stigmatized patients accept opaque AI diagnoses due to shame and urgency, bypassing the demand for transparency. This effect disappears when explanations are provided. (source: Guo & Chen_Investigating whether AI will replace human physicians.txt; domain: healthcare)

## Transparency Constructs

Transparency is operationalized as a **diagnosis explanation condition**: participants read either a brief conversation (diagnosis and treatment options only) or an extended conversation in which the medical agent explains symptom analysis, possible diagnoses, the rationale for the specific diagnosis, treatment options with rationale, and medication efficacy. This operationalization captures [[outcome-transparency]] (what the diagnosis is) combined with [[process-transparency]] (why this diagnosis was made) and [[natural-language-explanations]] (delivered in plain language via a simulated chat interface). The four-component explanation operationalization aligns with the principle of "intelligibility of explainable AI" cited by the authors (Arrieta et al., 2020).

The no-explanation condition represents the black-box opacity commonly criticized in AI medical systems, corresponding to a lack of [[algorithmic-transparency]] from the patient's perspective.

## Trust Constructs

The study measures multiple dimensions of trust:

- **Functional trust / [[cognitive-trust]]**: Operationalized as source credibility (4 items: trustworthiness, competence, knowledge, goodwill) and message credibility (3 items: accuracy, authenticity, believability). These capture belief-based, rational assessments of the AI's reliability.
- **Behavioural trust / [[behavioural-trust]]**: Operationalized as persuasive effect (5 items including treatment adherence, willingness to consult again), capturing the downstream behavioural dimension of trust.
- **Relational trust / [[affective-trust]]**: Operationalized as perceived empathy (5 items), self-disclosure comfort, and psychological distance — capturing the affective and relational dimensions of the patient–agent relationship.

The study explicitly tests [[algorithm-aversion]] (algorithm aversion theory predicts lower trust in AI for traditionally human decisions) against machine heuristic theory (predicts higher trust in AI due to objectivity stereotyping), finding evidence for algorithm aversion at the functional level.

## Relevance to Research Questions

**RQ1**: The paper provides a multi-dimensional operationalization of trust in an AI medical consultation context, decomposing it into functional (cognitive), relational (affective), and emotional dimensions. It also operationalizes transparency as a within-subject manipulation across all three medical agent types, illustrating how explanation can be defined operationally in the healthcare context. This contributes to RQ1's interest in how these constructs are defined and measured across domains.

**RQ2**: The study provides clear evidence of a direct positive effect of explanation on trust across all three dimensions and all agent types, with no interaction between explanation type and consultation source on functional trust (main effect only). The null effect of stigma on functional and relational trust is a notable null finding. The interaction effect on empathy (humans benefit more from explanation than AI) and the stigma × explanation interaction on source credibility are conditional effects relevant to RQ2's interest in non-linear or conditional patterns. The paper explicitly confirms algorithm aversion in healthcare, consistent with RQ2.

**RQ3**: The study does not manipulate user expertise directly; all participants are undergraduate students (mean age 18.67). The paper acknowledges this limitation and notes that reactions in real patients — particularly those with genuine stigmatized conditions — may differ. Patient role (vs. expert clinician) is implicitly central: the entire study takes a patient-centered perspective. This makes it relevant but limited for RQ3, which focuses more on professional expertise.

## Related pages

- [[cognitive-trust]]
- [[affective-trust]]
- [[behavioural-trust]]
- [[algorithm-aversion]]
- [[natural-language-explanations]]
- [[outcome-transparency]]
- [[process-transparency]]
- [[domain-context]]
- [[perceived-risk]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]
