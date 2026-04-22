# Hernandez-Bocanegra & Ziegler 2023 — Methods

**Summary**: A between-subjects user study (N=223) comparing two interface types (GUI navigation vs. natural language chatbot) and two levels of interactivity for conversational explanations in a hotel recommender system, using structural equation modeling to test a mediation model from explanation quality to trust.

**Sources**: Hernandez-Bocanegra & Ziegler_Explaining recommendations through conversations.pdf

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-19

---

## Study design
experimental (between-subjects, 2×2 design: interface type × degree of interactivity)

## Sample
- N: 223
- Population: general public (adult participants)
- Domain: e-commerce / hospitality (hotel recommender system)
- Country / region: not reported
- Recruitment method: not reported

## Transparency operationalization
- Type: algorithmic transparency and process transparency, operationalized as multi-dimensional transparency: information provision (how recommendations are generated), understanding input (what data the system uses), understanding output (why an item fits preferences), and interaction (what to change for a different prediction), following Hellmann et al.
- Manipulation or measure: between-subjects manipulation of (1) interface type — GUI-based navigation vs. natural language chatbot (ConvEx); and (2) degree of interactivity — lower interactivity (aggregated aspect ratings only) vs. higher interactivity (access to filtered customer comments supporting or rebutting ratings); perceived transparency measured as latent variable in SEM via multi-item scales for each sub-dimension
- Scale / instrument name: adapted from Hellmann et al. transparency scale (four sub-constructs); exact scale name not reported
- Number of items: not reported

## Trust operationalization
- Type: cognitive trust — trusting beliefs (honesty and competence) and trusting intentions (willingness to act on recommendations); trusting intentions dropped from final SEM due to insufficient discriminant validity from perceived effectiveness
- Measure: multi-item self-report Likert scales for trusting beliefs; perceived effectiveness measured separately (captures behavioural dimension)
- Scale / instrument name: not reported (adapted trust scale)
- Number of items: not reported
- Behavioural vs self-report: self-report (trusting beliefs via Likert; no behavioural reliance measure)

## Moderators and covariates tested
- Rational decision-making style: measured via questionnaire; moderated the effect of interactivity degree on explanation quality — more rational users in high-interactivity conditions rated explanation quality significantly higher; relevant to RQ3 as a user information-processing style moderator
- Intuitive decision-making style: measured; did not significantly moderate the interface-type effect
- Visualization familiarity: measured; did not significantly moderate the interface-type effect
- User expertise / AI literacy: not explicitly measured or manipulated

## Statistical approach
- Primary analysis method: Structural Equation Modeling (SEM); also multivariate comparison of means across conditions; moderation analysis for decision-making style
- Software: not reported
- Key model fit or effect size reported: SEM path coefficients reported; GUI vs. chatbot mean difference on explanation quality (M=3.87 vs. M=3.69); model fit indices not specified in source page

## Author-noted limitations
- GUI outperformed chatbot contrary to hypothesis, which may reflect limitations of the specific chatbot implementation rather than a fundamental advantage of GUI
- Trusting intentions could not be discriminated from perceived effectiveness, limiting the trust measurement model
- The study used a hospitality domain (hotel RS) which may limit generalisability to higher-stakes recommendation contexts
- General-public users asked primarily factoid and evaluation questions; system-level transparency questions were rare (24 of 1,806), suggesting the study may not capture expert-user information needs
- The dataset (ConvEx-DS) and dialog model are domain-specific

## Related pages
- [[hernandez-bocanegra-conversational-explanations]]
- [[process-transparency]]
- [[algorithmic-transparency]]
- [[natural-language-explanations]]
- [[cognitive-trust]]
- [[behavioural-trust]]
- [[user-expertise]]

## References
Hernandez-Bocanegra, D. C., & Ziegler, J. (2023). Explaining recommendations through conversations: Dialog model and the effects of interface type and degree of interactivity. *ACM Transactions on Interactive Intelligent Systems*.
