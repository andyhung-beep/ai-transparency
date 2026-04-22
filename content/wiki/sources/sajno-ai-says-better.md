# AI Says I'm Better: Evaluating the Effect of AI Defer on Users — A Study Protocol

**Source file**: [Original article](../../raw/Sajno et al._AI Says I'm Better.pdf)

**Summary**: This paper presents a pre-registered study protocol investigating how Learning to Defer (LtD) — an AI paradigm where the system delegates decisions to humans when the human is likely to outperform the model — combined with Explainable AI affects decision accuracy, cognitive processing style, and trust, with particular attention to individual psychological differences as moderators.

**Sources**: Sajno et al._AI Says I'm Better.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Sajno et al. (2025, *Annual Review of Cybertherapy and Telemedicine*) present a study protocol rather than completed empirical findings. The protocol proposes an experiment in which approximately 550 participants classify noisy images from ImageNet under three between-subjects conditions and two stakes-level framing conditions. The study's primary theoretical contribution is connecting the Learning to Defer (LtD) paradigm — where an AI recognizes its own limitations and actively returns decision authority to a human when the human is likely to be more accurate — with Explainable AI and cognitive dual-process theory.

The study is motivated by the problem of overreliance and distrust as opposing failure modes in human-AI interaction, and seeks to understand under what conditions AI interventions shift users from fast, automatic (System 1) to slow, deliberate (System 2) processing. The domain is general cognitive task performance (noisy image classification), with clinical decision-making identified as a primary intended application domain.

**Three experimental conditions:**
- **LtD (Defer)**: AI explicitly delegates the classification decision to the user, making clear that the system is uncertain and deferring.
- **LtD + XAI (Defer + Explanation)**: AI defers and also provides a GradCAM visual explanation of its processing.
- **Hidden Delegation**: AI has already processed the image but does not inform the participant; the participant is unaware of AI involvement.

**Two stakes conditions (crossed with conditions above):**
- **Neutral narrative**: Standard classification framing.
- **High-stakes narrative**: Emphasizes that failing to classify the object correctly could have severe consequences (dangerous objects framing).

## Key Findings

This is a study protocol — no empirical findings are reported. The authors provide the following hypotheses:

- LtD is expected to outperform Hidden Delegation in accuracy, because explicit delegation of responsibility activates System 2 (deliberate) processing. [Hypothesized domain: general cognitive tasks, with intended extension to clinical settings]
- LtD + XAI is expected to further improve accuracy and cognitive engagement relative to LtD alone, as the explanation provides additional grounding for deliberate reasoning. [Hypothesized]
- Hidden Delegation is expected to foster System 1 reliance and more errors because the absence of contextual cues and responsibility framing encourages habituation. [Hypothesized]
- High-stakes framing is expected to amplify cognitive engagement (longer response times, higher accuracy) across all conditions. [Hypothesized]
- Individual differences are expected to moderate all condition effects: analytic decision-making style and positive AI attitudes will increase engagement with LtD + XAI; high intolerance of uncertainty and suppressive emotion regulation will reduce trust and increase avoidant behavior when explanations are absent. [Hypothesized]

## Transparency Constructs

The paper addresses two distinct transparency mechanisms:

1. **Learning to Defer (LtD)**: A process-level transparency mechanism in which the AI communicates its own epistemic limits — specifically, when the human is expected to outperform the model — and explicitly transfers decision authority. This is a form of [[process-transparency]]: the system makes its uncertainty and decision delegation logic visible to the user.

2. **Explainable AI (GradCAM)**: A visual post-hoc explanation technique applied to the model's image classification, highlighting regions of the image that were most influential in the model's processing. This is a form of [[explainability]] via saliency visualization.

The study treats LtD as the primary novel transparency construct, and XAI as an additive enhancement. The theoretical framing is that both mechanisms serve as a "cognitive honk" — triggering users to re-engage analytically with a decision they might otherwise delegate mindlessly.

## Trust Constructs

The paper does not directly measure trust as its primary dependent variable but addresses it through the lens of overreliance and distrust as behavioral failure modes. The study's concern is with calibrated reliance: neither too much delegation to the AI (overreliance) nor too little adoption (distrust/algorithm aversion).

Trust is conceptualized as influenced by:
- **System design features**: Whether the AI is transparent about its limitations (LtD) and whether it provides explanations.
- **Individual differences**: Attitudes toward AI, intolerance of uncertainty, emotion regulation strategies, and decision-making style.
- **Contextual/emotional stakes**: High-stakes framing may increase vigilance and reduce over-trust.

The proposed measures capture aspects of [[behavioural-trust]] (accuracy, response time, agreement with AI) and include psychometric scales for AI attitudes (General Attitudes towards AI Scale, GAAIS) and intolerance of uncertainty (IUS-12). The hidden delegation condition operationalizes a baseline of trust without disclosed AI involvement — a naturalistic condition where trust cannot be consciously calibrated.

## Relevance to Research Questions

**RQ1**: The protocol introduces Learning to Defer as a novel transparency construct that has not been widely studied in the human-AI trust literature. LtD conceptualizes transparency not as disclosure of model internals but as epistemic humility — the AI transparently signals when it should not be trusted. This reframes transparency as a dynamic, contextual property of the system rather than a static interface feature. The study also proposes measuring System 1/System 2 activation as a cognitive process mediator linking transparency to trust and performance (source: Sajno et al._AI Says I'm Better.txt).

**RQ2**: The protocol is designed to test whether two transparency-enhancing mechanisms (LtD, LtD + XAI) improve decision accuracy over a Hidden Delegation baseline. The expected direction is positive (transparency improves accuracy), with XAI providing additive benefit. Emotional salience (high-stakes framing) is treated as a context moderator. These are hypotheses, not confirmed findings — but the design provides a rigorous structure for investigating conditional transparency effects (source: Sajno et al._AI Says I'm Better.txt).

**RQ3**: Individual psychological differences are the central moderating variables: decision-making style (analytic vs. intuitive), AI attitudes, intolerance of uncertainty, and emotion regulation strategies. The study explicitly argues that ignoring individual variability leads to oversimplified models of human-AI interaction. This is a strong theoretically-motivated contribution to understanding how user characteristics moderate transparency effects, though empirical confirmation is pending (source: Sajno et al._AI Says I'm Better.txt).

## Related pages

- [[explainability]]
- [[process-transparency]]
- [[trust-calibration]]
- [[algorithm-aversion]]
- [[appropriate-reliance]]
- [[behavioural-trust]]
- [[user-expertise]]
- [[perceived-risk]]
- [[rq2-relationships]]
- [[rq3-user-roles]]
