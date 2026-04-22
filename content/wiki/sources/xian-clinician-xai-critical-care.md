# Clinician Preferences for Explainable AI in Critical Care: A Comparative Study of Interpretable Models and Visualizations for Intubation Decision Support

**Source file**: [Original article](../../raw/Xian et al._Clinician preference for explainable AI in critical care.pdf)

**Summary**: This study develops and evaluates three novel time-aware SHAP-based visualization formats for an ICU intubation prediction model, finding that clinicians (n = 206) strongly prefer a dual-encoded heatmap over a temporal force plot and a temporal bar chart, primarily because the heatmap aligns with clinicians' cognitive workflows and minimizes the mental effort required to connect physiological trends with predicted risk.

**Sources**: Xian et al._Clinician preference for explainable AI in critical care.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Published in the International Journal of Medical Informatics (Vol. 210, 2026), this paper by Xian, Mehandjiev, Constantinides, Chen, Quboa, and Kitchen (University of Manchester) addresses the gap between technical XAI development and clinical adoption. Using ICU time-series data from the MIMIC-III database (4,608 patients, 10 medical variables over 7 hours), the authors trained multiple ML models, selected a Random Forest (AUC = 0.94), and applied SHAP to generate feature importance explanations.

Three novel, time-aware visualization formats were designed to address the limitation that standard SHAP plots lack temporal context:
1. **Temporal force plot**: segments and color-codes SHAP values by time intervals.
2. **Temporal bar chart**: aggregates absolute feature contributions over time windows.
3. **Dual-encoded heatmap**: overlays SHAP contribution values (color intensity) with raw variable values (text), enabling simultaneous assessment of feature importance and clinical measurements.

An online survey via Prolific (n = 206 clinicians) assessed comprehension, perceived usefulness, perceived ease of use, and preference.

## Key Findings

- The dual-encoded heatmap was preferred by approximately 55% of clinicians, the force plot by 30%, and the bar chart by only 15% (source: Xian et al._Clinician preference for explainable AI in critical care.txt; domain: critical care / ICU).
- The heatmap received the highest TAM3 ratings for Perceived Ease of Use (M = 3.84), Perceived Usefulness (M = 3.84), and Behavioral Intention to Use (M = 3.79) out of 5 (source: Xian et al._Clinician preference for explainable AI in critical care.txt; domain: critical care / ICU).
- Despite highest preference ratings, the heatmap scored lowest in objective comprehension accuracy (76%), while the bar chart (90%) and force plot (92%) were better understood on factual questions (source: Xian et al._Clinician preference for explainable AI in critical care.txt; domain: critical care / ICU).
- Overall comprehension accuracy across all formats was 78%, with Q1 (comparing all three formats simultaneously) scoring lowest at 47% (source: Xian et al._Clinician preference for explainable AI in critical care.txt; domain: critical care / ICU).
- Random Forest (RF) outperformed more complex deep learning architectures (LSTM, CNN) for this ICU tabular time-series task, achieving AUC = 0.94; FiO2 was the most influential predictor (source: Xian et al._Clinician preference for explainable AI in critical care.txt; domain: critical care / ICU).
- Force and bar chart formats required clinicians to mentally reconnect separated clinical data and model reasoning, increasing cognitive load and reducing perceived usability compared to the heatmap's integrated view (source: Xian et al._Clinician preference for explainable AI in critical care.txt; domain: critical care / ICU).
- Explanation presentation format independently influences clinician trust, separate from prediction content — supporting human-centered XAI principles (source: Xian et al._Clinician preference for explainable AI in critical care.txt; domain: critical care / ICU).

## Transparency Constructs

The paper centers on **SHAP-based feature contribution explanations**, operationalized as [[explainability]] in a clinical context. All three visualization formats represent variants of local, instance-level XAI.

Key innovation: introducing **temporal explainability** — existing SHAP plots are static (single time-point), but the authors redesign them to show how feature contributions evolve over a 7-hour window. This temporal dimension is operationalized differently across the three formats.

The heatmap's superiority is theorized through **cognitive fit** (Vessey & Galletta, 1991): effectiveness depends on the match between the problem representation and the user's task structure. Clinicians mentally integrate time series to assess deterioration trajectories; the heatmap mirrors this integrated view, reducing cognitive effort.

This also connects to **graphical integrity** (Tufte) — the heatmap maintains a direct link to raw clinical data while encoding model attribution, minimizing abstraction. The formats represent different points on a [[process-transparency]]–readability tradeoff.

## Trust Constructs

Trust is measured indirectly through the Technology Acceptance Model 3 (TAM3) constructs: Perceived Usefulness, Perceived Ease of Use, and Behavioral Intention to Use. These capture [[cognitive-trust]] (utility-based evaluation) and a behavioral intention dimension adjacent to [[behavioural-trust]].

The paper also references explanations' role in enabling clinicians to "validate recommendations against the patient's recent physiological trajectory" — framing XAI as a mechanism for [[appropriate-reliance]] rather than blind trust or [[algorithm-aversion]].

The study explicitly notes that explanation presentation format shapes clinician trust independently of content, contributing to the understanding of how transparency delivery (not just quantity or accuracy) affects [[algorithmic-trust]] in high-stakes contexts.

## Relevance to Research Questions

**RQ1**: Provides a domain-specific (critical care) operationalization of transparency as time-aware visual XAI. The paper contributes to understanding how transparency must be tailored to clinical reasoning workflows rather than adopting universal formats. Adds to [[rq1-conceptualizations]] by showing that cognitive fit is an explanatory adequacy criterion beyond accuracy.

**RQ2**: Demonstrates that explanation format significantly affects clinician acceptance and perceived trust even when prediction content is identical. The superior heatmap performance despite lower objective comprehension is a counterintuitive non-linear finding — clinicians may prefer and trust something they find less precisely comprehensible if it aligns with their workflow. Contributes to [[rq2-relationships]].

**RQ3**: Clinicians are the user population throughout; the study does not formally segment by clinical specialty or experience level, though the sample includes a mix of clinician types with only a minority being practicing ICU clinicians. The authors acknowledge this as a limitation. The study nonetheless addresses RQ3 by centering clinician (expert) preferences specifically, contrasting with lay-user XAI research. Relevant to [[rq3-user-roles]].

## Related pages

- [[explainability]]
- [[uncertainty-visualization]]
- [[causability]]
- [[cognitive-trust]]
- [[appropriate-reliance]]
- [[user-expertise]]
- [[domain-context]]
- [[rq3-user-roles]]
