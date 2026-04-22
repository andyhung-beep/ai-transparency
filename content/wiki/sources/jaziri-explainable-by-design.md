# Explainable by Design: Enhancing Trustworthiness in AI-Driven Control Systems

**Source file**: [Original article](../../raw/Jaziri & Sassi_Explainable by design.pdf)

**Summary**: A hybrid Deep Reinforcement Learning (DRL) framework that embeds symbolic reasoning, multi-head self-attention, and Layer-wise Relevance Propagation (LRP) directly into the learning process, evaluated across 20,000 simulated episodes and a 120-participant human-AI interaction study, demonstrating that intrinsic explainability improves user trust and comprehension with only a modest performance trade-off.

**Sources**: Jaziri & Sassi_Explainable by design.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Jaziri and Sassi (2025) propose and evaluate a hybrid DRL architecture designed around an "explainability-by-construction" principle: rather than attaching post hoc explanation methods (such as SHAP or LIME) after training, the model integrates three complementary explanation mechanisms during learning itself:

1. **Symbolic reasoning** — decision trees mapping state-action pairs to logical rules (CART algorithm, max depth 12), providing discrete, human-readable justifications.
2. **Multi-head self-attention** (12 heads) — attention weights highlighting which state features drove each decision.
3. **Layer-wise Relevance Propagation (LRP)** — backward propagation of relevance scores attributing each neuron's contribution to a decision.

The underlying policy network is a Double-Deep Q-Network (DDQN) trained on two simulated domains: (1) autonomous vehicle control in CARLA simulator (12,000 scenarios), and (2) sepsis treatment planning using synthetic MIMIC-IV/eICU-based data (8,000 patient cases). Human-AI interaction was evaluated in a controlled lab study with 120 participants (60 clinicians, 60 engineers) using 4K displays, eye tracking (Tobii Pro), and haptic feedback.

## Key Findings

- The hybrid model achieved a task-completion rate (TCR) of 91.9% in the AV domain versus 96.2% for standard DDQN — a ~4% performance trade-off. [Domain: autonomous vehicles / healthcare]
- Safety scores improved: 95.8% (hybrid) vs. 92.4% (DDQN) in the AV domain; 92.5% vs. 89.4% in sepsis treatment. [Domain: autonomous vehicles / healthcare]
- Critical error rate decreased by 15.3% (from 6.0% to 5.1%, p<0.001). [Domain: autonomous vehicles / healthcare]
- Mean inference latency was 42 ms (well below the 50 ms real-time threshold), with P95 at 48 ms. [Domain: autonomous vehicles / healthcare]
- User trust score increased 19% with the hybrid model (mean=6.0/7) vs. DDQN (5.0/7), a large effect (d=1.05, p<0.001). [Domain: autonomous vehicles / healthcare]
- Comprehension reached 91.3% vs. 65.7% for DDQN (+25.6%, d=1.23, p<0.001). [Domain: autonomous vehicles / healthcare]
- Response time decreased from 3.7 s (DDQN) to 2.9 s (hybrid, −22.7%, d=0.97, p<0.001). [Domain: autonomous vehicles / healthcare]
- Cognitive load (NASA-TLX) decreased from 68 to 56 (−15.3 points, d=0.90, p<0.001). [Domain: autonomous vehicles / healthcare]
- User trust and comprehension showed a very strong positive correlation (R²=0.94, p<0.001, N=120), confirming that higher understanding directly fosters trust. [Domain: autonomous vehicles / healthcare]
- Ablation analysis: symbolic reasoning contributed ~45% of comprehension gains; multi-head attention +35% comprehension and +0.5 trust points; LRP +0.2 clarity points and identified 89% of critical neurons. [Domain: autonomous vehicles / healthcare]
- Clinicians showed higher trust (11 vs. 10) and comprehension (90% vs. 89%), while engineers showed lower cognitive load (53 vs. 59) and faster response times (2.7 s vs. 3.1 s) — demonstrating expertise-dependent differences in how explainability is experienced. [Domain: healthcare / engineering]
- Decision trees (88% preference) and attention heatmaps (82%) were preferred by participants; LRP heatmaps were found too complex (12% preference). [Domain: autonomous vehicles / healthcare]
- In healthcare, the model reduced treatment rejections by 25% and improved patient outcomes by 8%. [Domain: healthcare]
- In AV simulation, 95.8% safety score corresponded to an 18% reduction in simulated accident rates. [Domain: autonomous vehicles]
- The model maintained robustness under sensor noise up to 20% Gaussian perturbation (TCR declined by only 1.3% vs. 2.3% for DDQN). [Domain: autonomous vehicles]

## Transparency Constructs

The paper operationalizes transparency as **intrinsic, real-time explainability** — what the authors call "explainability-by-construction." This contrasts with post hoc methods (SHAP, LIME) that are applied after model training and introduce inference latency of 150–350 ms, exceeding the sub-50 ms requirement for real-time safety-critical control.

The three components map onto distinct forms of transparency:
- Symbolic reasoning → [[algorithmic-transparency]] (rule-based justifications)
- Attention heatmaps → [[process-transparency]] (highlighting which inputs drove decisions)
- LRP → [[traceability]] (end-to-end attribution of decision formation)

The framework is positioned as enabling [[causability]] (Holzinger et al., 2020) — allowing users to trace the causes of decisions at a human-interpretable level, going beyond technical saliency to clinically actionable reasoning.

## Trust Constructs

Trust is measured via a seven-point Likert scale (Trust Score), with pre/post measurements. The paper treats trust as primarily **cognitive trust** — based on comprehension and confidence in the system's reasoning — rather than affective or behavioural trust. The strong correlation between comprehension and trust (R²=0.94) supports a cognitive-trust model where understanding the system's reasoning is the proximal cause of trust.

The paper also observes that users who did not receive explanations (DQN/DDQN baselines) showed lower trust, higher cognitive load, and slower response times — consistent with the notion that opacity impedes [[cognitive-trust]] formation and increases task burden. See [[cognitive-trust]] and [[algorithmic-trust]].

## Relevance to Research Questions

**RQ1**: The paper operationalizes transparency as intrinsic, multi-component explainability (symbolic rules + attention + LRP) and trust via Likert-scale ratings in a controlled human-AI study. It contributes a formal "explainability-by-construction" framework that distinguishes between forms of explanation and their separate contributions to comprehension and trust. See [[rq1-conceptualizations]].

**RQ2**: The paper reports a large positive effect of embedded explainability on user trust (+19%) and comprehension (+25.6%) compared to non-explainable baselines. A strong positive correlation between comprehension and trust (R²=0.94) supports a mediated pathway: explainability → comprehension → trust. The 4% performance trade-off is positioned as acceptable given the safety and trust gains, suggesting a non-linear value function for explainability where modest accuracy loss yields large trust benefits. See [[rq2-relationships]].

**RQ3**: The study explicitly compares two user expertise groups (clinicians vs. engineers). Clinicians showed higher trust and comprehension gains; engineers showed lower cognitive load and faster response times. This suggests that the *form* of benefit from explainability varies by expertise: domain experts benefit more on trust/comprehension dimensions, while technical experts benefit on efficiency dimensions. Qualitative interviews also reveal that decision trees and attention heatmaps were more accessible than LRP for non-technical users — a clear interaction between explanation format and user expertise. See [[rq3-user-roles]].

## Related pages

- [[explainability]]
- [[causability]]
- [[traceability]]
- [[cognitive-trust]]
- [[user-expertise]]
- [[rq3-user-roles]]
