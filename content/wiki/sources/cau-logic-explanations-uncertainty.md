# Effects of AI and Logic-Style Explanations on Users' Decisions Under Different Levels of Uncertainty

**Source file**: [Original article](../../raw/Cau et al._Effects of AI and logic-style explanation on users_ decitions.pdf)

**Summary**: A large-scale two-study experiment (N ≈ 1,300) examining how explanation logic-style (inductive, abductive, deductive), user uncertainty, AI correctness, and AI uncertainty jointly influence decision-making in image and text classification tasks. Inductive explanations were found to be the most persuasive style, leading to overreliance on the AI even when predictions were incorrect.

**Sources**: Cau et al._Effects of AI and logic-style explanation on users_ decitions.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Cau et al. (2023) address a gap in XAI research by systematically studying four factors that influence the effectiveness of AI explanations in decision support: user uncertainty, AI correctness, AI uncertainty, and explanation style. Two crowdsourced studies were conducted via Prolific — one on handwritten digit recognition (MNIST) and one on sentiment analysis (Yelp Reviews) — with approximately 659 and 665 participants respectively, each assigned to one of four explanation conditions: no explanation, inductive, abductive, or deductive style.

Explanation styles were derived from Peirce's syllogistic theory and mapped to existing XAI techniques:
- **Inductive** (bottom-up): example-based explanations (k-NN nearest neighbours), where users must infer the rule from presented examples.
- **Abductive** (best-guess cause): saliency/highlight-based explanations (Grad-CAM, LIME), where users identify the most significant features from a highlighted rule.
- **Deductive** (top-down): explicit rule-to-conclusion explanations (natural language / LIME word weights), where the rule and cause are provided and users evaluate the AI's conclusion.

The paper is among the first to jointly evaluate all four factors across two distinct data domains (image and text).

## Key Findings

- In both domains, users primarily relied on the raw instance (image or text) as their first source of decision information, regardless of user uncertainty level. (Domain: general HCI, image and text classification)
- When the AI made correct predictions, users relied on the AI prediction as a secondary source; when the AI made incorrect predictions, explanations displaced the AI prediction as the second source. (Domain: general HCI)
- Users showed systematic overconfidence: only 34.5% of high-uncertainty image instances and 14.0% of high-uncertainty text instances were correctly self-identified as difficult by participants. (Domain: general HCI)
- Users had difficulty identifying high AI uncertainty: only ~22% of high-AI-uncertainty instances were correctly perceived as such in both domains, indicating that AI prediction and explanation alone are insufficient to expose model uncertainty. (Domain: general HCI)
- Low user uncertainty and correct AI predictions both significantly and positively predicted task performance in both domains. (Domain: image and text classification)
- In the image domain, inductive and deductive explanation styles significantly decreased task performance when AI uncertainty was low and the AI was wrong, indicating overreliance. Abductive explanations did not show this negative effect. (Domain: image classification)
- No significant interaction between explanation style and AI uncertainty was found for task performance in the text domain, suggesting domain-specific effects. (Domain: text classification)
- For agreement with the AI, inductive explanations produced the highest agreement in the image domain under low AI uncertainty — even when the AI was incorrect — confirming that inductive style is the most persuasive. Abductive explanations under low AI uncertainty reduced agreement relative to no explanation. (Domain: image classification)
- In the text domain, inductive explanations also led to higher agreement than no explanation, and this persisted regardless of AI uncertainty level. (Domain: text classification)

## Transparency Constructs

The paper operationalises [[explainability]] by classifying explanation techniques according to three logical reasoning styles:

- **Inductive explanations** (e.g., [[example-based-explanations]]): present similar training instances; users must infer the general rule. Mapped to k-NN neighbour presentations.
- **Abductive explanations** (e.g., [[uncertainty-visualization]], saliency maps): present the rule (feature weights/highlights) and the AI prediction; users must identify the best causal account. Mapped to Grad-CAM and LIME highlighting.
- **Deductive explanations** (e.g., [[natural-language-explanations]], LIME feature weights as explicit rules): present both cause and rule; users only evaluate whether the AI's conclusion follows. Mapped to encoder-decoder natural language rationales and LIME word-weight bar charts.

The paper also operationalises [[uncertainty-visualization]] indirectly by manipulating AI uncertainty (epistemic, via Monte Carlo dropout) and measuring whether users perceive it correctly.

## Trust Constructs

The paper focuses on [[behavioural-trust]] operationalised via two objective metrics:
- **Agreement**: whether the user's final classification matches the AI's prediction.
- **Reliance**: participant ranking of which information source (instance, AI prediction, explanation) most influenced their decision.

Task performance (correctness) serves as a downstream measure that reflects over- or under-reliance, capturing elements of [[appropriate-reliance]] and [[algorithm-aversion]] (the latter not the focus, but implicated when users reject correct AI advice).

[[trust-calibration]] is implicitly addressed: users are systematically overconfident relative to objectively measured uncertainty, and they fail to detect high AI uncertainty — a trust calibration failure.

## Relevance to Research Questions

**RQ1**: Operationalises explanations via a novel taxonomy based on logical reasoning styles (inductive/abductive/deductive), contributing a theoretically grounded framework for classifying XAI techniques. Also operationalises user and AI uncertainty as distinct constructs.

**RQ2**: Demonstrates that the relationship between explanations and user behaviour is strongly conditional on explanation style, domain (image vs. text), AI correctness, and AI uncertainty level. Inductive explanations are consistently more persuasive and lead to overreliance when the AI is wrong, representing a non-linear/conditional transparency–trust relationship. The confidence-boosting effect of explanations does not reliably translate to better decisions.

**RQ3**: Does not directly vary user expertise. However, the overconfidence findings imply that lay users (non-experts) miscalibrate their uncertainty. The authors note future work should examine expert vs. novice differences. Indirectly relevant to [[user-expertise]] as a moderator.

## Related pages

- [[explainability]]
- [[example-based-explanations]]
- [[uncertainty-visualization]]
- [[appropriate-reliance]]
- [[trust-calibration]]
- [[rq2-relationships]]
