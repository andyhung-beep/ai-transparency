# User Expertise / AI Literacy

**Summary**: User expertise — including domain knowledge, AI literacy, and professional role — is the most consistently identified moderator of transparency–trust relationships in this corpus, affecting what explanation types are effective, how reliance patterns manifest, and whether transparency interventions are beneficial or harmful.

**Sources**: Multiple — see individual source pages.

**Research questions addressed**: RQ1, RQ3

**Last updated**: 2026-04-18

---

## Definition and Dimensions

User expertise in AI transparency research encompasses multiple interrelated dimensions:

1. **Domain expertise**: knowledge of the subject matter of AI decisions (e.g., clinical knowledge for medical AI, radiology training for imaging AI).
2. **AI/ML literacy**: understanding of how AI systems work, their limitations, and common error types.
3. **Professional role**: formal occupational roles that structure how users interact with AI (clinician, analyst, operator, citizen).
4. **Task experience**: accumulated experience with a specific AI system or task type.
5. **Novice vs. expert user**: a binary distinction often used to group users in experimental designs.

## Key Moderation Findings

### Expertise Changes Optimal Explanation Format

- Clinical seniority reverses the effect of explanation assertiveness: junior clinicians benefit from assertive (directive) AI communication (39.2% diagnostic error reduction); senior clinicians benefit more from non-assertive (suggestive) communication (domain: healthcare; Calisto et al., 2025).
- Analogies designed for laypeople improve non-expert decision accuracy in skin cancer detection but are unnecessary and potentially distracting for experts (domain: general/lab; He et al., 2024).
- Clinicians prefer the visualization format that best matches their existing cognitive workflow (dual-encoded SHAP heatmap preferred for ICU decision-making due to temporal reasoning alignment), demonstrating that explanation effectiveness is mediated by cognitive fit with domain expertise (domain: healthcare; Xian et al., 2026).
- Non-expert community health workers (CHWs) in India prefer having SHAP/LIME explanations present even when they cannot interpret them — desire for explanations decouples from comprehension (domain: healthcare/Global South; Okolo et al., 2024).

### Expertise Changes Reliance Patterns

- Domain experts (therapists) show substantially lower overreliance on incorrect AI recommendations than laypeople with identical information — suggesting expertise provides an independent check on AI errors (domain: healthcare; Lee & Chew, 2023).
- Technical experts in oil-and-gas inspection show asymmetric risk preferences (preferring to classify anomalies conservatively) that are not captured by standard trust scales, demonstrating domain-specific behavioural patterns invisible to generic measures (domain: industrial; Perlmutter et al., 2024).
- Experienced clinicians trust AI significantly more than less experienced clinicians (β = 0.28, p = 0.015), with a feedback loop where transparency amplifies trust when AI is correct but accelerates trust erosion when AI errs (domain: healthcare; Yu et al., 2025).
- AI literacy training has no significant effect on appropriate reliance in high-risk decisions when given as a short intervention without accompanying XAI (domain: general/lab; Leichtmann et al., 2023).

### Expertise Determines Who Benefits from XAI

- Experts are better at discriminating correct from incorrect XAI explanations; novices are more deceived by imperfect (incorrect) explanations (domain: general/lab; Spitzer et al., 2025).
- Low task-capacity users benefit from explanations via a "placebo effect" — even irrational (randomly permuted) SHAP explanations improve their decisions, suggesting heuristic rather than analytical processing (domain: e-commerce; Wang & Ding, 2024).
- Experts in cybersecurity/automotive domains benefit more from visual SHAP explanations than secondary experts or novices (domain: automotive security; Lundberg et al., 2022).

## Cultural and Institutional Moderators

- Indian university students show significantly higher dispositional trust toward AI conversational agents than Western comparison groups — baseline trust propensity is culturally mediated (domain: education; Nelekar et al., 2021).
- Domain expertise (medical vs. sports) moderates advice reliance independently of explanation type — participants rely more on AI in domains where the AI's knowledge advantage is perceived as greater (domain: general/lab; Kornowicz & Thommes, 2025).

## Measurement Approaches

Expertise is operationalized across the corpus as:
- Professional role (physician, radiologist, therapist, CHW, pilot)
- Years of experience (continuous)
- Domain knowledge test score (post-task)
- Self-reported AI familiarity / AI anxiety (validated scales)
- Task-related capacity (post-task quiz; Wang & Ding)
- Need for Cognition (NFC) scale (trait-level cognitive engagement)

## Related pages

- [[domain-context]]
- [[trust-calibration]]
- [[appropriate-reliance]]
- [[explainability]]
- [[counterfactual-explanations]]
- [[rq3-user-roles]]

## References

Calisto, F. M., Nunes, N., & Nascimento, J. C. (2025). Personalized explanations for clinician-AI interaction in breast imaging. *International Journal of Human-Computer Studies* [details TBD].

He, G., Bhatt, U., & Weller, A. (2024). Opening the analogical portal to explainability: How analogies shape AI explanations for different expertise levels. *CHI Conference on Human Factors in Computing Systems* [details TBD].

Kornowicz, J., & Thommes, K. (2025). Algorithm, expert, or both? Determinants of algorithm adoption in managerial decision-making. *Journal of Behavioral Decision Making* [details TBD].

Lee, J., & Chew, E. (2023). Understanding the effect of counterfactual explanations on trust and reliance on AI for human-AI collaborative clinical decision making. *Proceedings of the ACM on Human-Computer Interaction* (CSCW2), 7.

Leichtmann, B., Humer, C., Hinterreiter, A., Streit, M., & Mara, M. (2023). Effects of explainable artificial intelligence on trust and human behavior in a high-risk decision task. *Computers in Human Behavior* [details TBD].

Lundberg, J., Riveiro, M., & Bång, M. (2022). Experimental analysis of trustworthy in-vehicle intrusion detection system using eXplainable artificial intelligence (XAI). *IEEE Access* [details TBD].

Nelekar, P., Kulkarni, A., & Krishnaswamy, N. (2021). Effectiveness of embodied conversational agents for managing academic stress. *ACM International Conference on Intelligent Virtual Agents* [details TBD].

Okolo, C. T., Agarwal, Y., Dell, N., & Vashistha, A. (2024). "If it is easy to understand then it will have value": Examining perceptions of explainable AI with community health workers in rural India. *Proceedings of the ACM on Human-Computer Interaction* (CSCW), 8.

Perlmutter, S., Gifford, T., & Krening, S. (2024). Impact of example-based XAI for neural networks on trust, understanding, and performance. *International Journal of Human-Computer Studies* [details TBD].

Spitzer, M., Schlegel, U., & Keim, D. A. (2025). Imperfections of XAI: Phenomena influencing AI-assisted decision-making. *ACM Transactions on Interactive Intelligent Systems* [details TBD].

Wang, D., & Ding, Y. (2024). The rationality of explanation or human capacity? A study of human-AI collaboration in clinical decision support. *Journal of the American Medical Informatics Association* [details TBD].

Xian, Y., Mehandjiev, N., Constantinides, M., Chen, Y., Quboa, Q., & Kitchen, G. (2026). Clinician preferences for explainable AI in critical care. *International Journal of Medical Informatics*, 210 [details TBD].

Yu, K., Guo, J., Shen, Y., & Martens, H. (2025). Research and analysis of trust and control in human–AI collaboration in healthcare. *Frontiers in Psychology* [details TBD].
