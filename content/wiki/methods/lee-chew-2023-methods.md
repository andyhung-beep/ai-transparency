# Lee & Chew 2023 — Methods

**Summary**: A within-subject experiment with 17 participants (7 therapists, 10 laypersons) comparing salient feature (SHAP) explanations to counterfactual (DiCE) explanations in a clinical stroke rehabilitation assessment task, finding that counterfactual explanations reduce overreliance on wrong AI outputs by 21% while producing lower subjective trust scores.

**Sources**: Lee & Chew_Understanding the effect of counterfactual explanations on trust.pdf

**Research questions addressed**: RQ1 / RQ2 / RQ3

**Last updated**: 2026-04-19

---

## Study design
experimental (within-subject counterbalanced; two conditions)

## Sample
- N: 17 (7 therapists with average 12.85 years of experience; 10 laypersons / students with no rehabilitation experience)
- Population: domain professionals (therapists) and laypersons (students)
- Domain: healthcare / clinical decision support (stroke rehabilitation assessment — Range of Motion and Compensation rating)
- Country / region: not reported
- Recruitment method: not reported

## Transparency operationalization
- Type: (A) salient feature explanation (SHAP-based attribution); (B) counterfactual explanation (DiCE-generated)
- Manipulation or measure: within-subject counterbalanced manipulation of two explanation conditions — (A) Condition Features: AI prediction score + top-3 SHAP features as radar chart comparing unaffected and affected sides; (B) Condition Counterfacts: Condition A + textual counterfactual explanations (which feature values would need to change to flip the AI's prediction, generated via DiCE); each condition included 8 cases (3 correct AI outputs, 5 incorrect); cognitive forcing functions applied equally to both conditions (hidden AI output until requested, brief loading delay); feed-forward neural network trained on kinematic sensor data from 15 post-stroke survivors
- Scale / instrument name: not applicable
- Number of items: not applicable

## Trust operationalization
- Type: cognitive (self-reported); behavioural (reliance/overreliance)
- Measure: (1) Self-reported trust — single 100-point Likert item; (2) Reliance — agreement with AI outputs (counts of right/wrong decisions per AI correctness condition); (3) Overreliance — agreeing with a wrong AI output; (4) Agreement level — degree of concurrence with AI; (5) Usability questionnaire items including trust, transparency, perceived usefulness, and frustration; (6) Decision duration
- Scale / instrument name: not reported (custom 100-point single item for trust; custom usability questionnaire)
- Number of items: 1 (primary trust item); not reported (usability questionnaire)
- Behavioural vs self-report: both (behavioural reliance and overreliance measures; self-report trust and usability)

## Moderators and covariates tested
- User expertise (therapist vs. layperson): key moderator — therapists showed lower overreliance and lower performance degradation on wrong AI outputs than laypersons across both conditions; counterfactual benefit on overreliance reduction was larger for laypersons (30%) than therapists (8%) (highly relevant to RQ3)
- AI output correctness (right vs. wrong AI output): manipulated within cases — analyses separately reported for correct and incorrect AI output conditions
- Explanation order (counterbalanced): controlled via within-subject counterbalancing

## Statistical approach
- Primary analysis method: Wilcoxon signed-rank test (within-subject comparisons of decision counts, trust, duration between conditions); descriptive analysis of F1 scores and agreement levels by expertise and AI correctness
- Software: not reported
- Key model fit or effect size reported: counterfactual explanations reduced overreliance by 21% overall (29/136 decisions); therapist overreliance reduction 8% (5/56), layperson 30% (24/80); self-reported trust: Features M = 73.78/100 vs. Counterfacts M = 45.20/100; decision duration: Features 57 s vs. Counterfacts 75 s (18 s longer)

## Author-noted limitations
- Very small sample (N = 17); insufficient statistical power for many comparisons; findings are exploratory
- Only 5 incorrect AI outputs per condition limits measurement of overreliance
- Within-subject design introduces order/learning effects despite counterbalancing
- Single task domain (stroke rehabilitation ROM and Compensation assessment); generalizability limited
- Self-reported trust (single item) diverges from behavioural reliance; both needed to characterize the trust–reliance relationship

## Related pages
- [[lee-chew-counterfactual-explanations-trust]]
- [[counterfactual-explanations]]
- [[explainability]]
- [[trust-calibration]]
- [[appropriate-reliance]]
- [[behavioural-trust]]
- [[user-expertise]]
