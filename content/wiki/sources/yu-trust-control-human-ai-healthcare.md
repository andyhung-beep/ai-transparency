# Research and Analysis of Trust and Control in Human-AI Interaction for Decision-Making Systems in Optimizing Public Health Service

**Source file**: [Original article](../../raw/Yu et al._Research-and-Analysis-of-Trust-and-Control-in-Huma.pdf)

**Summary**: An empirical mixed-methods study with 42 clinicians in a Chinese radiology setting that applies cybernetic theory to model trust formation and calibration in AI-assisted clinical decision-making, finding that transparency boosts trust when AI performs correctly but accelerates trust erosion when errors occur.

**Sources**: Yu et al._Research-and-Analysis-of-Trust-and-Control-in-Huma.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Published in the *Journal of Organizational and End User Computing* (Vol. 37, Issue 1, January–December 2025), this paper by Xiaoxuan Yu et al. (Northeastern University China; China Medical University; University of Florida) investigates trust and control dynamics in AI-assisted healthcare decision-making using a cybernetic framework.

The study involved 42 clinicians (32 radiologists/physicians/residents; 10 medical students) at a Chinese tertiary-care hospital using an AI-powered clinical decision support (CDSS) system for interpreting chest X-ray images. Participants worked under two experimental conditions (unaided vs. AI-assisted) and two AI design conditions (explainable vs. black-box AI output; high- vs. low-autonomy AI). Quantitative measures (trust ratings, override frequency, diagnostic accuracy) were supplemented by semi-structured interviews analysed via thematic coding.

The cybernetic framework models trust as a dynamic, recalibrating variable governed by feedback loops: positive feedback when AI aligns with clinical reasoning (increasing reliance), negative feedback when errors accumulate (triggering correction or rejection).

## Key Findings

- AI-assisted diagnoses significantly outperformed unaided diagnoses (t = 5.67, p < 0.001). [domain: healthcare/radiology, China]
- Explainable AI yielded significantly higher trust ratings than black-box AI (t = 4.23, p = 0.002), with the explainability beta coefficient β = 0.42 (p = 0.001, R² = 0.48). [domain: healthcare/radiology, China]
- Higher AI autonomy led to significantly higher override rates (t = 3.89, p = 0.005), suggesting that reduced control increases resistance. [domain: healthcare/radiology, China]
- More experienced clinicians trusted AI more (r = 0.52, p = 0.002), and experience predicted higher reliance (r = 0.41, p = 0.011). [domain: healthcare/radiology, China]
- Qualitative findings: trust is not a single value but continuously recalibrated; clinicians trust AI more when it explains its reasoning; trust is fragile — errors erode it faster than successes build it. [domain: healthcare/radiology, China]
- A critical paradox: transparency enhances trust when AI is correct but also reveals AI limitations and accelerates trust loss when errors occur. [domain: healthcare/radiology, China]
- Clinicians overwhelmingly preferred to retain final decision authority; trust is highest when human oversight is maintained. [domain: healthcare/radiology, China]
- Over 60% of Chinese physicians in prior surveys reported unwillingness to accept AI recommendations autonomously without human supervision. [domain: healthcare, China]

## Transparency Constructs

The paper operationalises [[algorithmic-transparency]] primarily as **explainability** — AI systems providing reasoning for their recommendations (highlighted diagnostic indicators, clinical indicators). Two conditions are contrasted: explainable AI (with visual and clinical rationale) vs. black-box AI (outputs without reasoning).

The study also addresses [[process-transparency]] through the cybernetic framework: transparency of AI reasoning processes is treated as a feature that enables clinicians to calibrate trust appropriately. The paper notes that transparency is "one of the most important reasons" for AI non-adoption when absent.

## Trust Constructs

- **[[trust-calibration]]**: Central construct. The paper explicitly frames trust as a dynamic parameter requiring calibration between under-reliance and over-reliance (automation bias).
- **[[cognitive-trust]]**: Measured via Likert-scale items; driven by AI reliability, transparency, and alignment with clinical reasoning.
- **[[behavioural-trust]]** (reliance/override): Operationalised through override frequency and AI recommendation acceptance rates.
- **[[appropriate-reliance]]**: The cybernetic model posits an optimal "trust homeostasis" — neither too much nor too little.
- **[[algorithm-aversion]]**: Briefly noted as a risk when AI errors are encountered (clinicians may reject valid recommendations due to past errors).

## Relevance to Research Questions

**RQ1**: Operationalises transparency as explainability (reasoning provision) vs. black-box opacity. Trust is measured both quantitatively (Likert scale) and qualitatively (thematic coding). The cybernetic feedback model provides a process-level conceptualisation of trust formation and erosion. (source: Yu et al._Research-and-Analysis-of-Trust-and-Control-in-Huma.txt)

**RQ2**: Demonstrates a positive linear effect of AI transparency on trust (β = 0.42) but qualifies this with a non-linear/conditional dynamic: transparency amplifies both trust gain (when AI is correct) and trust loss (when AI errs). Reports that trust erosion after errors is disproportionately large relative to trust gains from successes — a key asymmetry. The relationship between autonomy and override rates is negative (less control → more overrides). [domain: healthcare, China] (source: Yu et al._Research-and-Analysis-of-Trust-and-Control-in-Huma.txt)

**RQ3**: Explicitly tests user expertise as a moderator. More experienced clinicians show significantly higher trust (β = 0.28, p = 0.015, R² = 0.32) and different reliance patterns. The study distinguishes between AI-exposed and AI-unexposed clinicians and between residents/physicians and students. (source: Yu et al._Research-and-Analysis-of-Trust-and-Control-in-Huma.txt)

## Related pages

- [[trust-calibration]]
- [[algorithmic-transparency]]
- [[appropriate-reliance]]
- [[algorithm-aversion]]
- [[user-expertise]]
- [[domain-context]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]
- [[rq3-user-roles]]
