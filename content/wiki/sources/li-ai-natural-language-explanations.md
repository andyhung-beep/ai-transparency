# When AI Explains in Natural Language: Unveiling the Impact of Generative AI Explanations on Educators' Grading and Feedback Practices

**Source file**: [Original article](../../raw/Li et al._When AI explains in natural language.pdf)

**Summary**: A four-phase experiment with 60 human graders shows that GenAI-produced natural-language grading explanations significantly improved educators' feedback quality compared to no AI support or to traditional XAI-derived important-word highlights, and that educators perceived natural-language insights as more useful, comprehensible, and adoption-worthy.

**Sources**: Li et al._When AI explains in natural language.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Li, Shan, Rakovic, Guan, Gasevic, and Chen (2025) examine whether generative AI (GPT-4) natural-language grading explanations can support human educators in assessing secondary students' short-answer responses, with a focus on both current and future assessment practices. The study contrasts three conditions: (G1) no AI support, (G2) important-word highlights from a BERT-based automatic grader via integrated-gradients XAI, and (G3) chain-of-thought natural-language explanations from a GPT-4 grader. The study used a four-phase design (Pre-Training → Pre-Eval → Exp-1 → Exp-2) to examine both immediate effects of AI insights and transfer effects one week later. Sixty participants were recruited from Prolific; 56 completed all phases.

Grading tasks came from the ASAP-SAS dataset (KAGGLE), covering Q9 (English comprehension/summarisation) and Q10 (science reasoning). Human assessment quality was evaluated on grading correctness and learner-centred feedback quality (agency, sense-making, learning impact dimensions).

Domain: educational assessment / K-12 and secondary education.

## Key Findings

- GenAI natural-language insights (G3) significantly improved educators' feedback quality compared to no AI support (β = 0.190, p = 0.010); important-word highlights (G2) had negligible impact (β = 0.065, p = 0.366). [domain: education]
- Natural-language insights showed greater (though marginally non-significant) potential to improve grading accuracy than highlights (G3: β = 0.556, p = 0.093; G2: β = −0.060, p = 0.848). [domain: education]
- G3 participants perceived natural-language insights as significantly more informative, useful, comprehensible, and efficiency-enhancing than G2 participants perceived important-word highlights (all comparisons p < 0.05, effect sizes r ∈ [0.382, 0.664]). [domain: education]
- Providing natural-language insights slightly reduced educators' feedback efficiency (G3 spent ~20 s less than the ~40 s reduction achieved by G1 during Exp-1), suggesting a cognitive cost to processing and integrating AI explanations. [domain: education]
- Transfer effects (Exp-2, one week later, no AI support): G2 and G3 educators showed non-significant trends toward better feedback quality and G2 grading duration increased significantly, suggesting important-word highlights may have slowed graders' autonomous workflows. No strong evidence of lasting skill improvement from GenAI exposure was found within this timeframe.
- Grading tasks were relatively easy for the recruited experienced educators, limiting the ceiling for improvement in accuracy.
- Concerns about over-reliance on AI-powered insights are acknowledged: educators could uncritically align with AI-generated decisions even when incorrect (though this study used only correctly-graded answers in Exp-1 to control for this variable).

## Transparency Constructs

The study contrasts two distinct operationalisations of AI transparency in assessment support:

1. **Important-word highlights** (G2): derived via integrated-gradients XAI applied to BERT-based graders—a form of [[explainability]] that surfaces which words most influenced the machine's decision, analogous to local feature attribution. These require high cognitive effort from the human to interpret.
2. **Natural-language explanations** (G3): chain-of-thought reasoning from GPT-4 describing the assessment rationale step-by-step—an instance of [[natural-language-explanations]] that reduces interpretive burden by communicating reasoning in human-readable prose.

The comparison directly tests whether the modality of explanation (feature-level vs. natural-language) affects educator uptake and performance, operationalising [[process-transparency]] at the instance level.

## Trust Constructs

The study does not directly measure trust using validated psychometric scales. Instead, it assesses subjective acceptance and willingness to adopt AI insights (Q4 survey items: "I would be more willing to grade/compile feedback with the AI-powered insights"), which maps onto [[behavioural-trust]] (adoption intention) and elements of [[cognitive-trust]] (perceived usefulness, comprehensibility). The concern over over-reliance is framed as an inverse of [[appropriate-reliance]]: educators may anchor too heavily on AI outputs and reduce exercise of professional judgement.

## Relevance to Research Questions

**RQ1**: This paper provides evidence on how different types of AI explanation—feature-attribution (XAI highlights) vs. generative natural-language explanations—are conceptualised by end-users (educators) and how they operationalise transparency in practice. Natural-language explanations are perceived as more transparent and useful, suggesting that explanation modality is a critical dimension of how transparency is experienced rather than just provided.

**RQ2**: The paper reports a positive relationship between natural-language transparency and feedback quality (a behavioural-trust outcome), but the relationship is not uniform across outcome metrics: accuracy improvement was not statistically significant, and efficiency showed a trade-off (more time spent). This nuanced pattern suggests that transparency effects on trust-adjacent outcomes are outcome-specific and cannot be generalised without specifying the dependent variable.

**RQ3**: The study recruited exclusively experienced educators (K-12 teachers with teaching experience in relevant subjects), creating a sample of domain experts. The paper does not explicitly contrast expertise levels, but its findings raise questions about whether the benefits of natural-language explanations would differ for novice graders. The potential for over-reliance may be particularly relevant for less experienced graders who lack the professional reference points to critically evaluate AI explanations.

## Related pages

- [[natural-language-explanations]]
- [[explainability]]
- [[appropriate-reliance]]
- [[behavioural-trust]]
- [[user-expertise]]
- [[rq2-relationships]]
