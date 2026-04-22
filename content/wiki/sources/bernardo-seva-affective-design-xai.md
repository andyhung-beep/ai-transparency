# Affective Design Analysis of Explainable Artificial Intelligence (XAI): A User-Centric Perspective

**Source file**: [Original article](../../raw/Bernardo & Seva_Affective_Design_Analysis_of_Explainable.pdf)

**Summary**: Bernardo and Seva propose and test an XAI Trust Calibration (XAITC) model, arguing that affective (emotion-based) processing is a viable route for trust calibration from XAI alongside cognitive processing, using survey data (N = 202) and structural equation modeling to identify explanation form, communication style, and supplementary information as key design components, with AI anxiety, incidental emotion, AI reliability, and usage experience as significant moderators.

**Sources**: Bernardo & Seva_Affective_Design_Analysis_of_Explainable.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

This study fills a gap in XAI research by shifting focus from developer-centric, cognitively oriented explanations to an end-user-centric, affectively grounded perspective. The authors argue that the dominant assumption in XAI — that interpretability enhances trust through cognitive processing (analytic and analogic routes) — neglects a third trust calibration route identified by Lee and See (2004): the affective route, whereby emotions triggered during interaction with an AI system directly shape trust judgments. Building on Norman's three-level processing model and affective design theory, the authors develop the XAI Trust Calibration (XAITC) model, which proposes that XAI design elements evoke specific emotional states (drawn from the XAI Emotion Set, or XES, developed by Bernardo and Seva), which in turn mediate perceived trust and downstream reliance.

Data were collected in two phases. A pre-study online survey (N = 202) identified key XAI design components from end-user preferences. A main testbed experiment then exposed participants to different design configurations (varying explanation form, communication style, and supplementary information), measuring emotional responses, perceived usefulness, perceived trust, and behavioral reliance. Structural equation modeling with 2000 bootstrap iterations, exploratory factor analysis (KMO = 0.919, p < 0.001), and confirmatory factor analysis (CFI = 0.991, RMSEA = 0.039) were used to test the XAITC model and identify mediators and moderators. The study's domain is general AI/XAI with an industrial engineering and human-computer interaction perspective, conducted at De La Salle University, Manila.

## Key Findings

- Affective processing is a statistically supported route for trust calibration from XAI: emotions such as "interestingly surprised" and "trusting" significantly and positively mediated the relationship between explanation form and perceived trust, while "fearfully dismayed" mediated the relationship between communication style and perceived trust negatively (domain: general AI/XAI interface).
- Example-based explanation form increased "interestingly surprised" (β = 0.530, p = 0.001) and "trusting" (β = 0.419, p = 0.002) emotions more than feature- or rule-based explanations, while logic-robotic (vs. humanized) communication style significantly increased "fearfully dismayed" and "anxiously suspicious" emotional responses (domain: general AI/XAI interface).
- Perceived usefulness mediates the relationship between cognitive design elements (explanation form, communication style) and perceived trust, with communication style being a significant negative predictor of perceived usefulness under logic-robotic conditions (β = −0.940, p = 0.002) (domain: general AI/XAI interface).
- Perceived trust has a significant positive direct effect on behavioral reliance (β = 0.439, p = 0.001), confirming the cognitive-affective-to-behavioral trust chain hypothesized in the XAITC model (domain: general AI/XAI interface).
- Four moderators were found to significantly affect the calibration process: AI anxiety and incidental emotion (human factors), and perceived AI reliability and user experience with AI systems (AI factors); trust disposition and learning capability were not significant moderators (domain: general AI/XAI interface).
- Users with high AI anxiety exhibited lower perceived trust when "fearfully dismayed" emotions were evoked (β = −0.059 vs. β = 0.021 for low anxiety, z = 2.195, p = 0.014), and lower reliance from perceived trust (p = 0.039), demonstrating that emotional susceptibility to negative AI-related affect is a meaningful individual-difference moderator (domain: general AI/XAI interface).

## Transparency Constructs

The study examines XAI design as a transparency-delivery mechanism and identifies three key design components:
- **Explanation form**: the type or modality of explanation presented to the user (e.g., example-based, feature importance/saliency, rule-based); found to be the most affectively salient design dimension.
- **Communication style**: the register or tone used to convey the explanation, ranging from logic-robotic to humanized; logic-robotic style reliably evoked negative affect.
- **Supplementary information**: the presence or absence of contextual or background information accompanying the explanation; its absence increased "fearfully dismayed" emotions, suggesting that sparse explanations create uncertainty and discomfort.

These three components are operationalized as design-level constructs rather than method-level constructs, positioning the paper at the intersection of XAI and affective/emotional design.

## Trust Constructs

The XAITC model distinguishes:
- **Perceived trust** (cognitive-evaluative): measured by a three-item self-report scale; positioned as a mediator between emotional responses and reliance behavior.
- **Affective trust** (emotion-based): operationalized indirectly through discrete emotional states drawn from the XAI Emotion Set — "interestingly surprised," "trusting," "fearfully dismayed," and "anxiously suspicious" — which mediate the effect of design on perceived trust.
- **Behavioural trust / reliance**: the downstream behavioral outcome (intention to rely on the AI system), measured as a self-report reliance scale.
- **Trust disposition**: a baseline individual-difference measure of general propensity to trust, found not to be a significant moderator.
- **Perceived usefulness**: a cognitive mediator bridging explanation design and perceived trust.

The paper is notable for distinguishing these constructs empirically and showing that the affective path (emotion → perceived trust → reliance) operates in parallel with and sometimes more strongly than the purely cognitive path (design → perceived usefulness → perceived trust → reliance).

## Relevance to Research Questions

**RQ1**: The paper makes a direct contribution to conceptualization by proposing the XAITC model as an integrated account of how XAI design elements generate both affective and cognitive outcomes that jointly determine trust. It operationalizes affective trust via a purpose-built emotion set (XES) developed for the XAI context, extending beyond existing dichotomies of cognitive vs. affective trust to include discrete emotional states as measurable trust antecedents.

**RQ2**: The paper supports a **mediated, conditional relationship** between XAI design (transparency) and trust. The effect is not direct but runs through emotional and cognitive mediators. The relationship is further moderated by AI anxiety and incidental emotion, meaning that the same transparency design can produce very different trust outcomes depending on the user's affective state and predispositions. This identifies a non-linear and conditional transparency-trust relationship not captured by simple linear models.

**RQ3**: User experience with AI systems was a significant moderator of the trust calibration process: long-experience users showed a different moderation pattern than short-experience users, and experienced users (71.78% of the sample reported more than five years of AI experience) may calibrate trust differently than novices. AI anxiety is identified as a user-role-adjacent construct — users with high AI anxiety behave like a distinct "expertise" category in terms of trust sensitivity to emotional stimuli.

## Related pages

- [[explainability]]
- [[example-based-explanations]]
- [[affective-trust]]
- [[cognitive-trust]]
- [[behavioural-trust]]
- [[trust-calibration]]
- [[user-expertise]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]
- [[rq3-user-roles]]
