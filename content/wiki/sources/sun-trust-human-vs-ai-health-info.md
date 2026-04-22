# Understanding Trust Toward Human versus AI-generated Health Information through Behavioral and Physiological Sensing

**Source file**: [Original article](../../raw/Sun et al._Understanding trust toward human versus AI-generated health information.pdf)

**Summary**: A two-study investigation examining how the actual source (human professional vs. LLM) and disclosed label (human vs. AI) of online health information independently and jointly affect trust, using both self-report and novel multimodal physiological and eye-tracking measures.

**Sources**: Sun et al._Understanding trust toward human versus AI-generated health information.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Sun et al. (accepted, IJHCS; arXiv preprint 2025) investigated trust in online health information in the era of large language models. As AI-generated health content becomes indistinguishable from human-authored content, understanding the drivers of trust perceptions is critical. The authors conducted two complementary studies:

- **Study 1** (online survey, N=142): A mixed 2 (source: Human Professional vs. LLM) × 2 (label: Human Professional vs. AI) × 3 (information type: General, Symptom, Treatment) factorial design. Source was between-subjects; label and type were within-subjects.
- **Study 2** (laboratory, N=40): A fully within-subjects design replicating Study 1's factorial structure, augmented with continuous eye-tracking (Tobii Pro Fusion) and physiological recording (ECG, EDA, skin temperature).

The theoretical framework draws on the MATCH model of trust in AI systems, which integrates Model Attributes (source quality), Afforded Cues (interface signals such as labels), and Trust Heuristics (cognitive/affective shortcuts). This framing connects transparency labels to classic operationalizations of [[disclosure]] as an afforded trustworthiness cue.

---

## Key Findings

- **LLM-generated information was trusted more than human-generated information** (Study 1: mean trust score 3.97 vs. 3.89, p=.024, d=.14 medium; Study 2: mean 3.85 vs. 3.62, p<.01, d=.35 medium). Authors note this may reflect perceived objectivity and clear structure of AI-generated text. [Domain: online health information]
- **Information labeled as from human professionals was trusted more than information labeled as AI**, regardless of actual source (Study 1: mean 4.04 vs. 3.82, p<.001, d=-.39 medium; Study 2: mean 3.80 vs. 3.67, p=.01, d=-.23 medium). Labeling effects were stronger than source effects. [Domain: online health information]
- **The interaction between source and label was non-significant** in both studies, indicating that source and label exert independent additive effects on trust rather than interacting. [Domain: online health information]
- **Information type (general, symptom, treatment) did not significantly affect trust** nor did it interact with source or label (p=.505). Trust effects appear domain-invariant across health information subcategories. [Domain: online health information]
- **LLM-sourced information labeled as human received the highest trust** (Study 1: M=4.07), while human-sourced information labeled as AI received the lowest (Study 1: M=3.76), demonstrating vulnerability to mislabeling. [Domain: online health information]
- **Eye-tracking results (Study 2)**: Fixation count and saccade count in the main health information area were higher under AI labels, suggesting greater information scrutiny when AI authorship is disclosed. Fixation duration and pupil diameter on the label area differed by both source and label. [Domain: online health information, lab]
- **Physiological results (Study 2)**: HRV (RMSSD) and skin temperature differed significantly across label conditions, suggesting differential affective arousal when reading AI- vs. human-labeled health content. [Domain: online health information, lab]
- **Machine learning prediction**: Binary trust classification (high vs. low) from gaze and physiological features achieved 73% accuracy; information source classification achieved 65% accuracy, demonstrating that implicit behavioral signals partially reflect self-reported trust. [Domain: online health information, lab]
- **Qualitative themes (Study 1)**: Four themes emerged — (1) predisposition toward AI vs. humans; (2) perceived source of knowledge (training data vs. professional experience); (3) the human touch and accountability as trust-builders; (4) AI presentation quality and clarity as trust-enhancing. [Domain: online health information]
- **AI literacy and propensity to trust technology** showed stronger correlations with trust in LLM-sourced information than in human-sourced information, suggesting that individual differences in technology orientation moderate trust responses to AI content. [Domain: online health information]

---

## Transparency Constructs

This paper primarily addresses **[[disclosure]]** — specifically, whether and how the source label (human professional vs. AI) is disclosed alongside health information. The study decouples the actual information source from its disclosed label, creating a 2×2 design that isolates the independent effect of labeling as a transparency mechanism. This operationalization aligns with the **Afforded Cues** component of the MATCH model.

The paper does not examine process transparency, explainability, or algorithmic rationale disclosure; its focus is narrowly on source-attribution transparency (disclosure of authorship) in a consumer health information context.

---

## Trust Constructs

- **[[cognitive-trust]]**: Operationalized via a 13-item validated trust-in-online-health-information questionnaire (Cronbach's α=.92), capturing perceptions of objectivity, reliability, and credibility.
- **[[affective-trust]]**: Partially captured by physiological measures — HRV (RMSSD), skin conductance (EDA), and skin temperature — interpreted as indices of arousal/comfort during information evaluation.
- **[[behavioural-trust]]**: Implicit gaze behaviors (fixation, saccade, pupil dilation) serve as behavioral correlates of trust processing; not full behavioral reliance measures.
- **[[dispositional-trust]]** (measured as a moderator): Propensity to trust in technology (PPT, 6-item scale) and AI literacy (10-item MAILS) were collected as individual-difference moderators.

---

## Relevance to Research Questions

**RQ1**: Directly relevant. The paper operationalizes trust in online health information using a combination of self-report scales (cognitive trust), physiological indicators (affective correlates), and behavioral gaze measures. Transparency is operationalized narrowly as source-label disclosure, providing a precise definition of [[disclosure]] as an afforded cue in the MATCH framework.

**RQ2**: Directly relevant. The key finding is a dissociation between source and label effects: the actual source (LLM > human) and the disclosed label (human > AI) independently drive trust in opposite directions. This non-linear or dissociative pattern is notable — users trust LLM content more in terms of actual source but trust human-labeled content more when labels are present. The interaction is non-significant, supporting additive rather than multiplicative effects. This contributes nuance to the [[rq2-relationships]] synthesis, particularly regarding label-based trust manipulation in health contexts.

**RQ3**: Partially relevant. AI literacy and eHealth literacy correlated more strongly with trust in LLM content than human content, suggesting that users with greater AI familiarity calibrate trust differently toward AI-generated health information. This connects to [[user-expertise]] as a moderator of transparency–trust relationships in the health domain.

---

## Related pages

- [[disclosure]]
- [[algorithmic-trust]]
- [[cognitive-trust]]
- [[user-expertise]]
- [[domain-context]]
- [[rq2-relationships]]
