# A Neural Model to Jointly Predict and Explain Truthfulness of Statements

**Source file**: [Original article](../../raw/Brand et al._A neural model to jointly predict and explain truthfulness.pdf)

**Summary**: This paper introduces E-BART, a transformer-based model that jointly predicts the veracity of a claim and generates a natural language explanation for that prediction within a single architecture, and demonstrates through crowdsourced human evaluation that E-BART explanations increase human accuracy in detecting misinformation and make people more skeptical of claims.

**Sources**: Brand et al._A neural model to jointly predict and explain truthfulness.txt

**Research questions addressed**: RQ1, RQ2

**Last updated**: 2026-04-18

---

## Overview

Brand, Roitero, Soprano, Rahimi, and Demartini (2022, published 2023 in ACM Journal of Data and Information Quality) present E-BART, an architecture built on the BART transformer model that simultaneously produces a veracity classification and a human-readable abstractive explanation for automated fact-checking (AFC) of text claims. The core technical novelty is a "joint prediction head" that conditions both classification and explanation generation on the same decoder hidden states, ensuring the two outputs are internally coherent rather than produced by independent post hoc pipelines.

The paper evaluates E-BART on three datasets: FEVER (185,445 claims with evidence and veracity labels drawn from Wikipedia), e-FEVER (a FEVER extension by Stammbach and Ash augmented with generated explanations), and e-SNLI (570K sentence-pair entailment examples with human explanations). Evaluation combines automated metrics (classification accuracy, ROUGE scores for explanation quality, BLEU) and a crowdsourced human study using Amazon Mechanical Turk (four task variants comparing no explanation, E-BART explanation, ground truth explanation, and both explanations with explicit preference rating). The human study examined the impact of machine-generated explanations on truthfulness assessment accuracy among non-expert annotators.

## Key Findings

- E-BART achieved veracity prediction accuracy competitive with state-of-the-art models on FEVER (75.0–75.1), despite being trained on substantially fewer examples, suggesting that joint explanation generation encouraged better attention to relevant evidence (information quality/fact-checking domain). (source: Brand et al._A neural model to jointly predict and explain truthfulness.txt)
- The joint model (E-BART) and the separate pipeline (Separate-BART) achieved near-identical classification accuracy, confirming that generating explanations does not significantly impede veracity prediction performance (information quality/fact-checking domain). (source: Brand et al._A neural model to jointly predict and explain truthfulness.txt)
- Joint models showed higher internal consistency (veracity prediction and explanation were more coherent with each other) than separate pipeline models, as assessed by an independent "judge" model (information quality/fact-checking domain). (source: Brand et al._A neural model to jointly predict and explain truthfulness.txt)
- In the crowdsourced human study, showing E-BART explanations (Task 2, aggregated accuracy 0.90) was more effective than showing no explanation (Task 1, 0.83) and outperformed showing the ground truth explanation (Task 3, 0.65), in terms of improving human accuracy in spotting misinformation (information quality/general public domain). (source: Brand et al._A neural model to jointly predict and explain truthfulness.txt)
- E-BART explanations reduced false positives (claims incorrectly judged as true) from 122 to 93, making users more appropriately skeptical, without a comparable effect on false negatives; this is important because false positives are more harmful in misinformation contexts (information quality/general public domain). (source: Brand et al._A neural model to jointly predict and explain truthfulness.txt)
- After temperature scaling calibration, E-BART's confidence scores became well-calibrated (ECE reduced from 11.44% to 1.61%), enabling reliable communication of prediction uncertainty to end users (information quality/fact-checking domain). (source: Brand et al._A neural model to jointly predict and explain truthfulness.txt)

## Transparency Constructs

The primary transparency mechanism studied is **natural language explanation generation** — the automated production of abstractive, human-readable summaries justifying a veracity prediction. This is an instance of [[natural-language-explanations]] and [[explainability]] at the system level. The paper also implements [[uncertainty-visualization]] through calibrated confidence scores that communicate how certain the model is in its veracity prediction, addressing trust calibration for end users. The paper contrasts intrinsic (joint, truly reflecting the model's reasoning) versus post hoc (separate pipeline, explanations loosely attached to predictions) transparency, arguing that joint generation more faithfully represents the model's actual decision process and thus constitutes more genuine [[algorithmic-transparency]].

## Trust Constructs

The study does not measure trust using standard psychometric scales. Instead, trust is approached indirectly through behavioral and accuracy outcomes: the extent to which explanations increase human annotators' ability to correctly classify claims, reduce false positives, and increase skepticism. This maps to [[behavioural-trust]] (calibrated skepticism as a form of appropriate reliance on the AI-supported fact check) and [[trust-calibration]] (the desirability of neither blindly accepting nor blindly rejecting AI outputs). The paper cites Toreini et al. (2020) for the theoretical link between trustworthy machine learning and user trust, and frames the entire project as an effort to foster "a more trustworthy relationship between humans and deep learning models." [[Algorithmic-trust]] is implicitly discussed in the sense that the opacity of AFC systems (without explanations) previously deterred trust and adoption.

## Relevance to Research Questions

**RQ1**: The paper demonstrates an NLP-based operationalization of AI explainability — joint natural language explanation generation — that is novel relative to saliency or feature-attribution methods typical in the XAI literature. It also introduces calibrated confidence scores as a quantitative transparency mechanism. These operationalizations extend the conceptual toolkit available for transparency research.

**RQ2**: The human evaluation provides direct empirical evidence that natural language explanations generated by AI improve human decision accuracy in a fact-checking task. Crucially, the effect was conditional: E-BART explanations outperformed both no explanation and ground truth explanations in raising accuracy, suggesting a nuanced, non-obvious positive relationship between AI-generated transparency and user performance. The confidence calibration work also bears on the relationship between expressed uncertainty and user trust.

**RQ3**: The crowdsourced human study used general (non-expert) annotators on Amazon MTurk, with no manipulation or measurement of user expertise or domain knowledge. The paper does not address how expert fact-checkers (journalists, researchers) might respond differently to E-BART explanations; this remains a gap.

## Related pages

- [[natural-language-explanations]]
- [[explainability]]
- [[uncertainty-visualization]]
- [[trust-calibration]]
- [[algorithmic-trust]]
- [[rq1-conceptualizations]]
