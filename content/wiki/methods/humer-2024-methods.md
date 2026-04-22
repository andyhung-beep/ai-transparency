# Humer et al. 2024 — Methods

**Summary**: A between-subjects experiment (N=501) in a gamified mushroom-identification task comparing three XAI methods (Grad-CAM, nearest-neighbor examples, network-dissection concept labels) against a no-explanation control on decision correctness and self-reported trust calibration.

**Sources**: Humer et al._Reassuring, misleading, debunking.pdf

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-19

---

## Study design
experimental (between-subjects, four conditions: no explanation / Grad-CAM / nearest-neighbor examples / network-dissection)

## Sample
- N: 501
- Population: general public (end-users; not AI experts or domain experts)
- Domain: nature identification / general public (gamified mushroom-hunting scenario designed to be relatable to general adults)
- Country / region: not reported
- Recruitment method: not reported (online study implied by "between subjects" design and comparison to prior online and festival studies)

## Transparency operationalization
- Type: three operationalizations of explainability for image classification:
  (E1) Grad-CAM — gradient-based attribution heatmap overlaid on input images highlighting prediction-relevant regions (outcome transparency at feature level);
  (E2) Nearest-neighbor examples — training images closest to the input per predicted class displayed for similarity comparison (example-based explanation);
  (E3) Network-dissection — semantic concept labels assigned to neural network units with highlighted image regions (concept-based, combining causability cues with visual attribution)
- Manipulation or measure: between-subjects manipulation; participants assigned to one of four conditions; each participant evaluated 10 task items
- Scale / instrument name: not applicable (visual explanation displays, not a scale)
- Number of items: not applicable

## Trust operationalization
- Type: trust calibration as primary outcome — operationalized both behaviourally (decision correctness on correct vs. incorrect AI items) and via self-report (Trust in Automation questionnaire, system evaluation, intention to use)
- Measure: behavioural — decision correctness on edibility assessment and take/leave decisions for 10 items; self-report — Trust in Automation questionnaire (propensity to trust, system-specific trust ratings), system evaluation, and intention to use
- Scale / instrument name: Trust in Automation questionnaire (exact citation not specified; consistent with Heerink et al. or Körber variants)
- Number of items: not reported
- Behavioural vs self-report: both (decision correctness is primary behavioural measure; TiA and system evaluation are self-report)

## Moderators and covariates tested
- Domain knowledge (mushroom knowledge): measured; did not differ significantly across groups; prior studies found no significant effect of domain knowledge on performance — relevant to RQ3 (non-expert user population)
- AI knowledge: measured; did not differ significantly across groups
- Propensity to trust automation: measured; correlation analysis showed E2 and E3 participants relied less on general propensity to trust when forming system-specific trust judgments
- Item-level helpfulness of explanation: post-hoc analysis distinguishing "helpful" explanations (accordant with AI reliability on a given item) from "misleading" explanations; helpful explanations produced larger positive effects
- User expertise / AI literacy: not varied as a moderator; sample explicitly designed to represent non-expert end-users

## Statistical approach
- Primary analysis method: ANOVA / between-groups comparison for primary outcomes; item-level subset analysis for helpful vs. misleading explanations; correlation analysis for propensity to trust vs. system-specific trust by condition
- Software: not reported
- Key model fit or effect size reported: not reported (statistical significance thresholds and p-values reported; effect sizes not specified in source page)

## Author-noted limitations
- Grad-CAM alone yielded inconclusive effects; positive effects in prior studies may have been driven by the nearest-neighbor component of a combined interface
- Explanation effects are not uniform across items: the same method can reassure, mislead, or debunk depending on item characteristics, limiting aggregate-level conclusions
- Self-reported trust, system evaluation, and intention-to-use showed no significant effects for any explanation method — replicating null subjective-trust results from a prior festival study
- The study used a gamified, naturalistic task that may not generalise to higher-stakes professional contexts
- The mushroom-identification domain is artificial; expert-user populations were not tested

## Related pages
- [[humer-xai-methods-effects-decisions]]
- [[explainability]]
- [[example-based-explanations]]
- [[trust-calibration]]
- [[appropriate-reliance]]
- [[behavioural-trust]]
- [[algorithm-aversion]]
- [[user-expertise]]

## References
Humer, E., et al. (2024). Reassuring, misleading, debunking: Comparing effects of XAI methods on human decisions. *ACM Transactions on Interactive Intelligent Systems*.
