# Impact of Example-Based XAI for Neural Networks on Trust, Understanding, and Performance

**Source file**: [Original article](../../raw/Perlmutter et al._Impact of example-based XAI for neural networks on trust, understanding, and performance.pdf)

**Summary**: This within-subjects study with 24 expert oil-and-gas pipeline data analysts finds that providing example-based XAI explanations from two classes significantly increases trust and understanding without degrading objective decision performance, and that trust and understanding are tightly correlated in highly-technical populations.

**Sources**: Perlmutter et al._Impact of example-based XAI for neural networks on trust, understanding, and performance.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Perlmutter, Gifford, and Krening (2024, *International Journal of Human–Computer Studies*) investigate example-based XAI for a convolutional neural network (CNN) that classifies oil-and-gas pipeline sections as normal or anomalous. The study targets a gap in the literature: most XAI research uses general populations in low-stakes domains, and prior example-based XAI work had not varied the number of classes shown in explanations, nor examined effects on technical domain experts.

Twenty-four data analysts from a single pipeline inspection company participated in a within-subjects design across three interfaces:
- **Baseline**: no explanation, only the ML classification.
- **XAI-1**: three closest training examples from the predicted class only (one-class explanation).
- **XAI-2**: three closest training examples from both classes (two-class explanation).

Analysts classified pipeline images as "normal" or "anomaly," with the CNN's classification shown alongside. Measures included self-reported trust in the ML, trust in the human-machine team, understanding, perceived agreement, helpfulness, and objective performance (correct/incorrect decisions).

The domain is industrial safety / oil-and-gas infrastructure inspection, a high-risk context where misclassification has either environmental disaster or large monetary consequences.

## Key Findings

- Participants ranked XAI-2 as the most trusted interface, followed by XAI-1, then Baseline (Kruskal-Wallis, p = 0.003, η² = 0.18). Showing examples from two classes increased trust more than one class. [Domain: oil-and-gas pipeline inspection]
- Similarly, participants ranked XAI-2 as the most easily understood, followed by XAI-1, then Baseline (p = 0.009, η² = 0.15). [Domain: oil-and-gas pipeline inspection]
- There was a perfect Spearman correlation between trust and understanding rankings for XAI-2 (r = 1.00, p < 0.001), and strong correlations for XAI-1 (r = 0.818) and Baseline (r = 0.904). Trust and understanding are not independent in technical populations. [Domain: oil-and-gas pipeline inspection]
- Objective performance (accuracy of human-ML team decisions) did not differ significantly across the three interfaces (Chi-square, p = 0.075). Adding XAI improved the human experience without harming performance — contradicting the common belief in a performance–explainability tradeoff. [Domain: oil-and-gas pipeline inspection]
- Participants trusted the human-machine team more than the ML alone, regardless of interface (Wilcoxon, Z = -6.186, p < 0.001, d = 0.73). The ability to override AI is a more important trust factor than the presence of examples. [Domain: oil-and-gas pipeline inspection]
- Trust in the human-machine team decreased with years of experience (Kruskal-Wallis, p = 0.001, η² = 0.22); the most experienced analysts (10+ years) trusted the team least. Experience was not significant for trust in the ML alone. [Domain: oil-and-gas pipeline inspection]
- For XAI interfaces, the most important predictor of trust in the human-machine team (from Random Forest RFE) was understanding of the ML classification. For the Baseline interface, the most important predictor was AI anxiety ("I feel that if I depend on robots or AI too much, something bad might happen"). Adding explanations shifts participants from emotional to logical processing. [Domain: oil-and-gas pipeline inspection]
- Analysts did not treat the two classes equally: they were more likely to agree with an anomaly prediction and more likely to override a non-anomaly prediction, consistent with risk-averse behavior. [Domain: oil-and-gas pipeline inspection]
- Participants with moderate experience (2-10 years) found the XAI interfaces most helpful and reported highest understanding; least and most experienced groups reported lower understanding. A non-linear experience effect on XAI benefit was observed. [Domain: oil-and-gas pipeline inspection]
- Free-response analysis identified five key themes affecting trust and understanding: (1) priming/job threat fears, (2) training and education, (3) one vs. two classes in explanation, (4) interface presentation, and (5) machine errors.

## Transparency Constructs

The study uses [[example-based-explanations]] (prototype XAI) as its sole transparency intervention. The explanation format shows the k-nearest training instances, retrieved by comparing activation-graph fingerprints (keypoints from neural network hidden layers) of the test image with training images.

The study distinguishes between:
- **One-class explanation (XAI-1)**: Shows closest instances from the predicted class — normative explanation revealing why the system chose this class.
- **Two-class explanation (XAI-2)**: Shows closest instances from both classes — contrastive explanation enabling the user to compare and contrast, communicating boundary uncertainty when classes look similar.

The two-class format functions as a form of [[uncertainty-visualization]]: when class boundaries are ambiguous, the overlapping examples signal to the analyst that this is a difficult case. This is framed as more nuanced than a simple confidence percentage, and more honest about ML limitations.

## Trust Constructs

The study distinguishes two trust targets:
1. **Trust in the ML classification** — analogous to [[cognitive-trust]] in the automated agent's outputs, measured by self-report after each interface.
2. **Trust in the human-machine team** — a broader construct encompassing the analyst's confidence in the combined system including their own judgment, analogous to [[behavioural-trust]] or reliance on the overall system.

Participants systematically trusted the human-machine team more than the ML alone (moderate effect, d = 0.73). This finding implies that preserving human agency and control is a trust-critical design factor in high-stakes, expert-populated domains. The study also finds that experience modulates team trust but not ML trust, suggesting that expert analysts are more skeptical of collaborative arrangements.

Trust operationalization uses continuous 0-10 Likert scales consistent with (Wang et al., 2023; Zhou et al., 2019).

## Relevance to Research Questions

**RQ1**: The study contributes to the operationalization of trust in XAI by distinguishing trust in the ML agent from trust in the human-machine team and showing these are empirically separable. It also demonstrates that understanding and trust are highly correlated in technical populations — possibly more so than in general populations — raising the question of whether these should be treated as distinct constructs in expert domains (source: Perlmutter et al._Impact of example-based XAI for neural networks on trust, understanding, and performance.txt).

**RQ2**: Strong positive effect of two-class example-based XAI on ranked trust (p = 0.003) and understanding (p = 0.009). Notably, the effect does not appear in immediate within-interface trust ratings (p = 0.491), only when participants directly compare interfaces at study end — suggesting that XAI effects on trust may require comparative reference points to emerge. The finding that XAI shifts trust predictors from emotional (AI anxiety) to logical (understanding) is a novel mechanism. No performance cost is observed (source: Perlmutter et al._Impact of example-based XAI for neural networks on trust, understanding, and performance.txt).

**RQ3**: Experience has a non-linear relationship with XAI benefit: moderate-experience analysts benefit most; the most experienced analysts show lower team trust and may resist the human-AI collaborative model. Priming (clarifying that the AI will not replace workers) is identified as essential for reducing resistance in technical populations. The study is one of few to focus specifically on domain experts rather than novices (source: Perlmutter et al._Impact of example-based XAI for neural networks on trust, understanding, and performance.txt).

## Related pages

- [[example-based-explanations]]
- [[uncertainty-visualization]]
- [[cognitive-trust]]
- [[behavioural-trust]]
- [[appropriate-reliance]]
- [[user-expertise]]
- [[rq2-relationships]]
- [[rq3-user-roles]]
