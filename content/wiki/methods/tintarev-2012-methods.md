# Tintarev & Masthoff (2012) — Methods

**Summary**: A methodological paper and series of four empirical studies (total N ≈ 174 across studies) in movie and camera recommendation domains comparing baseline, non-personalized feature-based, and personalized feature-based explanations on decision effectiveness and user satisfaction, finding that personalization improves satisfaction but consistently harms decision effectiveness.

**Sources**: Tintarev & Masthoff_Evaluating_the_effectiveness_o.pdf

**Research questions addressed**: RQ1 / RQ2 / RQ3

**Last updated**: 2026-04-19

---

## Study design
mixed-methods (conceptual framework paper plus four empirical user studies; Study 1: N = 46; Study 2: N = 33; Study 3: N = 47; Study 4: N = 48)

## Sample
- N: approximately 174 across four studies (46 + 33 + 47 + 48)
- Population: general public / volunteer participants; Study 3 screened to include only participants likely to purchase a camera (domain involvement criterion)
- Domain: e-commerce / recommender systems (movies in Studies 1, 2, 4; cameras in Study 3)
- Country / region: not reported
- Recruitment method: not reported (volunteer / convenience)

## Transparency operationalization
- Type: process transparency (personalized feature-based explanations revealing user-model attributes) and outcome transparency (non-personalized feature-based explanations describing item features without revealing personalization logic)
- Manipulation or measure: within-subjects or between-subjects (varies by study) manipulation of explanation type: (1) Baseline explanation — brief external validation cue (e.g., "This movie is in the top 100 on IMDB"); (2) Non-personalized feature-based explanation — item features without reference to user model (e.g., "This movie is a Drama directed by X"); (3) Personalized feature-based explanation — features tailored to user preferences inferred from user model (e.g., "This movie stars your favourite actor")
- Scale / instrument name: not applicable (explanation type was a condition manipulation)
- Number of items: not applicable

## Trust operationalization
- Type: cognitive trust (one of seven defined explanation aims); behavioural trust (decision quality / effectiveness)
- Measure: primary effectiveness measure — discrepancy between pre-consumption rating (after reading explanation) and post-consumption rating (after watching movie or using camera), following Bilgic & Mooney (2005); secondary measures — satisfaction ratings, opt-out rate (proportion of items where participants could not form an opinion); trust as explicit aim is discussed conceptually but not measured as a separate self-report scale in the empirical studies
- Scale / instrument name: Bilgic & Mooney (2005) effectiveness metric; custom satisfaction rating scales
- Number of items: not reported (satisfaction items not specified)
- Behavioural vs self-report: both (pre/post-consumption rating discrepancy as behavioral proxy for decision quality; satisfaction ratings as self-report)

## Moderators and covariates tested
- Domain involvement / item familiarity: Study 3 screened for camera purchase likelihood; discussion notes that user familiarity with named actors and directors moderated the benefit of personalized explanations in movie studies — users unfamiliar with named actors could not utilise personalization effectively (implicit moderator relevant to RQ3)
- Recommendation domain (movies vs. cameras): tested implicitly via cross-experiment comparison; camera domain showed stronger effectiveness differences between personalized and non-personalized explanations
- Note: formal user expertise as a moderator was not included; AI literacy not measured

## Statistical approach
- Primary analysis method: t-tests and non-parametric equivalents (Wilcoxon) for pairwise comparisons of explanation conditions on effectiveness (rating discrepancy) and satisfaction; chi-square or Fisher's exact for opt-out rate comparisons
- Software: not reported
- Key model fit or effect size reported: Study 3 (cameras) — non-personalized significantly better effectiveness than personalized p < .01; personalized significantly higher satisfaction p < .01 (M = 3.27 vs. 2.38); Study 4 — opt-out rate dropped from 35.6% (title only) to 15.9% (explanation) p < .001; exact effect sizes (d or η²) not reported in source summary

## Author-noted limitations
- Sample sizes per study are small (33–48 participants), limiting statistical power to detect smaller effects
- Explanation quality and relevance may vary with recommender system accuracy, which was not independently controlled
- The effectiveness metric (pre/post-consumption rating discrepancy) captures over-estimation/under-estimation but may not fully capture all relevant dimensions of decision quality
- The movie domain relies on subjective enjoyment ratings, which may be less sensitive to explanation quality than more objective product domains
- Participant familiarity with named actors/directors was not formally measured but informally observed to moderate personalization benefit
- The paper's seven-aims taxonomy was developed prior to widespread LLM-based or XAI explanation methods; its mapping onto contemporary post-hoc explanation methods warrants re-evaluation

## Related pages
- [[tintarev-masthoff-explanation-effectiveness]]
- [[explainability]]
- [[outcome-transparency]]
- [[process-transparency]]
- [[trust-calibration]]
- [[cognitive-trust]]
- [[behavioural-trust]]
- [[user-expertise]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]
- [[rq3-user-roles]]

## References
Tintarev, N., & Masthoff, J. (2012). Evaluating the effectiveness of explanations for recommender systems: Methodological issues and empirical studies on the impact of personalization. *User Modeling and User-Adapted Interaction, 22*, 399–439.

Bilgic, M., & Mooney, R. J. (2005). Explaining recommendations: Satisfaction vs. promotion. In *Proceedings of the Beyond Personalization Workshop, IUI*, 13–18.
