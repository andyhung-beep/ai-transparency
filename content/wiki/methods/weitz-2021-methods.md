# Weitz 2021 — Methods

**Summary**: A between-subjects experiment (N = 60) comparing four XAI interface conditions (no agent, text agent, voice agent, embodied visual agent) in a speech recognition task, finding a significant linear trend whereby increasing human-likeness of the virtual explanation agent increased user trust in the AI system.

**Sources**: Weitz_Let me explain.pdf

**Research questions addressed**: RQ1 / RQ2

**Last updated**: 2026-04-19

---

## Study design
experimental (between-subjects, four conditions)

## Sample
- N: 60
- Population: general public (non-expert participants; varied background experience with voice assistants)
- Domain: speech recognition / human-computer interaction
- Country / region: Germany (Augsburg University)
- Recruitment method: not reported (convenience)

## Transparency operationalization
- Type: explainability (local, post-hoc, model-agnostic) via LIME; delivery modality manipulation (explanation interface humanization)
- Manipulation or measure: Four between-subjects conditions, all receiving LIME (Local Interpretable Model-Agnostic Explanations) visualizations — saliency-map-style highlights on spectrograms showing which audio segments most influenced the neural network's keyword classification: (1) No-agent (XAI only) — LIME visualisation without any virtual agent; (2) Text-agent — LIME plus text-based commentary from virtual agent "Gloria"; (3) Voice-agent — LIME plus voice-based commentary from Gloria; (4) Embodied-visual-agent — LIME plus commentary from full embodied visual avatar of Gloria with gestures. The explanation content was identical across agent conditions; only the delivery modality varied.
- Scale / instrument name: not applicable (between-subjects manipulation)
- Number of items: not applicable

## Trust operationalization
- Type: cognitive / situational (self-report)
- Measure: Trust in Automation (TiA) questionnaire (Jian et al., 2000), administered post-experiment; mean scores ranged from 4.48 (no agent) to 5.42 (embodied visual agent) on a 7-point scale
- Scale / instrument name: Trust in Automation (TiA) questionnaire, Jian et al. (2000)
- Number of items: not reported
- Behavioural vs self-report: self-report

## Moderators and covariates tested
- Human-likeness of agent (primary manipulation; linear trend tested): significant linear trend confirmed (R² = .16, F(3,56) = 3.45, p = .02, f = 0.42)
- Prior experience with voice assistants: noted as varying across participants but not formally tested as moderator
- Technical background (signal processing knowledge): identified as a potential internal trust factor in discussion but not measured or tested
- LIME visualisation ratings: compared across groups; no significant difference found (F(1,58) = 0.47, p = .495), suggesting halo effect from overall system trust

## Statistical approach
- Primary analysis method: one-way ANOVA with linear trend contrast (test of linear relationship between human-likeness levels and trust); post-hoc comparisons between conditions
- Software: not reported
- Key model fit or effect size reported: R² = .16; F(3,56) = 3.45, p = .02; Cohen's f = 0.42 (medium effect size); mean trust scores per condition reported on 7-point scale

## Author-noted limitations
- Small sample (N = 60, 15 per group) limits statistical power
- Single domain (speech recognition / keyword spotting); generalisability to other XAI contexts unclear
- Potential over-trust risk: humanizing explanation delivery may inflate trust beyond what is calibration-appropriate
- Participants requested more linguistic (natural language) explanations, comparative visualizations, and greater interactivity — suggesting LIME visualisations alone are insufficient
- Background knowledge in signal processing not controlled; could function as unmeasured moderator
- Trust measured only post-experiment (cross-sectional); no longitudinal assessment of trust dynamics

## Related pages
- [[weitz-virtual-agents-xai]]
- [[explainability]]
- [[natural-language-explanations]]
- [[process-transparency]]
- [[cognitive-trust]]
- [[trust-calibration]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]
