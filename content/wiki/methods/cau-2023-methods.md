# Cau et al. (2023) — Methods

**Summary**: Two large-scale crowdsourced experiments (total N ≈ 1,324) via Prolific comparing four explanation conditions (no explanation, inductive/example-based, abductive/saliency, deductive/rule-based) in image classification (MNIST) and text sentiment classification (Yelp Reviews) tasks, examining how explanation logic-style, user uncertainty, AI correctness, and AI uncertainty jointly influence decision-making.

**Sources**: Cau et al._Effects of AI and logic-style explanation on users_ decitions.pdf

**Research questions addressed**: RQ1 / RQ2 / RQ3

**Last updated**: 2026-04-19

---

## Study design
experimental (two crowdsourced between-subjects online experiments conducted via Prolific)

## Sample
- N: approximately 1,324 (Study 1: N ≈ 659 handwritten digit recognition; Study 2: N ≈ 665 sentiment analysis)
- Population: general public (Prolific crowdworkers; no domain expertise required)
- Domain: general HCI / image classification (MNIST handwritten digits) and text sentiment classification (Yelp Reviews)
- Country / region: not reported (Prolific platform; international)
- Recruitment method: Prolific platform

## Transparency operationalization
- Type: explanation logic-style (inductive, abductive, deductive explanations derived from Peirce's syllogistic theory and mapped to existing XAI techniques)
- Manipulation or measure: between-subjects manipulation of explanation condition across four groups — (1) no explanation: AI prediction only; (2) inductive (example-based): k-NN nearest-neighbor training instances presented so users infer the decision rule from examples (bottom-up reasoning); (3) abductive (saliency-based): rule and AI prediction provided; users identify the most significant causal features — implemented as Grad-CAM (image study) and LIME feature highlighting (text study); (4) deductive (rule-based): cause and rule both provided; users evaluate whether AI conclusion follows — implemented as LIME word-weight bar charts and encoder-decoder natural language rationales. AI uncertainty was also manipulated via Monte Carlo dropout (low vs. high epistemic uncertainty per trial); participants were asked to indicate their perception of AI uncertainty per trial.
- Scale / instrument name: not applicable (experimental manipulation); AI uncertainty manipulation via Monte Carlo dropout
- Number of items: not applicable

## Trust operationalization
- Type: behavioural (agreement with AI prediction as proxy for trust; reliance ranking as secondary measure)
- Measure: (1) agreement — whether the user's final classification matched the AI's prediction (binary per trial); (2) reliance — participant ranking of which information source (raw instance, AI prediction, explanation) most influenced their decision; (3) task performance (classification correctness) as downstream outcome reflecting appropriate reliance. No psychometric trust scale administered.
- Scale / instrument name: not applicable (behavioral measures only)
- Number of items: not applicable
- Behavioural vs self-report: both (agreement and task accuracy as behavioral; reliance source ranking as self-report)

## Moderators and covariates tested
- User uncertainty (low vs. high): measured per trial (subjective confidence in own judgment before seeing AI output); significantly predicted task performance; users systematically overestimated their ability to identify high-uncertainty instances (only 34.5% of high-uncertainty image instances and 14.0% of text instances correctly self-identified)
- AI correctness (correct vs. incorrect AI prediction): covariate manipulated by trial composition; when AI was correct, users relied on AI prediction as secondary source; when AI was incorrect, explanations displaced AI prediction as secondary source
- AI uncertainty (low vs. high epistemic uncertainty via Monte Carlo dropout): within-subjects covariate; users could correctly identify high AI uncertainty only ~22% of the time — a calibration failure
- Domain (image vs. text): between-studies factor; inductive explanations were persuasive in both domains; abductive explanations reduced agreement in image domain under low AI uncertainty but had no significant effect in text domain
- Note: user expertise was NOT varied or measured as an independent variable. The authors note that lay users (non-experts) miscalibrate both their own and AI uncertainty, and call for future research with expert vs. novice comparisons (relevant to RQ3 as a gap).

## Statistical approach
- Primary analysis method: mixed-effects logistic regression (for binary agreement outcome) and ordinal regression (for reliance rankings), with participant as random effect; interaction terms for explanation style × AI correctness × AI uncertainty
- Software: not reported
- Key model fit or effect size reported: Log-Odds coefficients and p-values reported; significant interactions between explanation style and AI correctness/uncertainty reported (e.g., inductive style under low AI uncertainty when AI wrong decreased task performance significantly in image domain; abductive explanations under low AI uncertainty reduced agreement relative to no explanation in image domain)

## Author-noted limitations
- Crowdworker sample lacks domain expertise; results may not generalize to expert users (e.g., physicians for medical imaging tasks)
- Task paradigms (MNIST digits, Yelp sentiment) are relatively simple and artificial; effects may differ in high-stakes real-world tasks
- AI uncertainty manipulation (Monte Carlo dropout) produced uncertainty levels that users could not reliably perceive, limiting the ecological validity of the uncertainty manipulation
- The categorization of explanation styles as inductive/abductive/deductive is a theoretical proposal; mapping to specific XAI techniques (Grad-CAM, LIME, k-NN) may not be the only or best instantiation
- Only one type of explanation per logic-style was tested; results may not generalize to other implementations of the same logical style

## Related pages
- [[cau-logic-explanations-uncertainty]]
- [[explainability]]
- [[example-based-explanations]]
- [[uncertainty-visualization]]
- [[appropriate-reliance]]
- [[trust-calibration]]
- [[rq2-relationships]]

## References
Cau, F. M., et al. (2023). *Effects of AI and logic-style explanations on users' decisions under different levels of uncertainty*. [Journal not reported in source summary.]
