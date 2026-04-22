# Suffian et al. (2025) — Methods

**Summary**: A three-group between-subjects user study (N = 70 after quality assurance) comparing a user-feedback-based counterfactual explanation method (UFCE) against automated diverse counterfactuals (DiCE) and a no-explanation control on task performance, feature understanding, actionability, and reliance in a game-based unfamiliar domain.

**Sources**: Suffian et al._The role of user feedback in enhancing understanding and trust.pdf

**Research questions addressed**: RQ1 / RQ2

**Last updated**: 2026-04-19

---

## Study design
experimental (three-group between-subjects online experiment)

## Sample
- N: 70 (after quality assurance screening; 101 recruited initially)
- Population: primarily university students aged 18–24
- Domain: synthetic / game-based learning environment ("Alien Nutri-Solver" — a fictional creature nutrition task designed to prevent prior knowledge confounds)
- Country / region: not reported
- Recruitment method: not reported (university student sample; convenience)

## Transparency operationalization
- Type: counterfactual explanation — two active conditions: (1) UFCE (User Feedback-based Counterfactual Explanation), where users specify features to modify and acceptable ranges before counterfactual generation; (2) DiCE (Diverse Counterfactual Explanations), automated generation of diverse counterfactuals without user constraints; (3) control group receives no explanations
- Manipulation or measure: between-subjects manipulation of explanation condition (UFCE vs. DiCE vs. control); counterfactual explanations shown after each game round; UFCE additionally elicits user feedback on preferred feature modifications before generating suggestions
- Scale / instrument name: not applicable (explanation type was a condition assignment)
- Number of items: not applicable

## Trust operationalization
- Type: cognitive trust (self-report) and behavioural trust (reliance)
- Measure: post-game survey with trust-related items (items 15–20); item 15 (general trust in the Alien Nutri-Solver framework) administered to all groups; items 16–20 (trust in explanations, confidence in explanations, perceived safety following suggestions, reliance behaviour) administered to explanation groups only; behavioural trust operationalized as objective suggestion usage during gameplay and self-reported non-usage of suggestions
- Scale / instrument name: custom survey items (not a validated named scale)
- Number of items: 6 items (items 15–20); item 15 asked of all three groups
- Behavioural vs self-report: both (objective suggestion usage logs + self-report survey items)

## Moderators and covariates tested
- None tested as formal moderators; prior knowledge was controlled by design (unfamiliar domain)
- User expertise and AI literacy were not measured or examined as moderators — relevant to RQ3 as a gap
- Sample was predominantly young students, limiting generalisability to other user populations

## Statistical approach
- Primary analysis method: Kruskal–Wallis H test for non-parametric between-group comparisons on primary outcomes; Mann–Whitney U test for pairwise post-hoc comparisons; effect sizes reported as r
- Software: not reported
- Key model fit or effect size reported: feature understanding H(2) = 9.920, p = 0.007; task performance H(2) = 24.729, p < 0.0001; actionability UFCE vs. DiCE: U = 367.5, p = 0.038, r = 0.298; suggestion usage U = 194.5, p = 0.026, r = -0.316; study power = 0.91 for large effects, 0.65 for medium effects

## Author-noted limitations
- Sample is predominantly 18–24-year-old students; findings may not generalise to other age groups or professional users
- The unfamiliar synthetic domain precludes assessment of how prior expertise moderates explanation effectiveness
- Statistical power is insufficient to detect medium-sized differences, so some null findings between UFCE and DiCE may reflect Type II error rather than genuine equivalence
- No formal validated trust scale was used, limiting comparability with the broader XAI–trust literature
- The game platform's engaging design may have introduced motivational confounds independent of explanation type

## Related pages
- [[suffian-user-feedback-understanding-trust]]
- [[counterfactual-explanations]]
- [[explainability]]
- [[behavioural-trust]]
- [[cognitive-trust]]
- [[appropriate-reliance]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]

## References
Suffian, M., et al. (2025). The role of user feedback in enhancing understanding and trust in counterfactual explanations for explainable AI. *International Journal of Human-Computer Studies*, 193, 103380.

Mothilal, R. K., Sharma, A., & Tan, C. (2020). Explaining machine learning classifiers through diverse counterfactual explanations. *Proceedings of the 2020 Conference on Fairness, Accountability, and Transparency*, 607–617.
