# Cognitive Trust

**Summary**: Cognitive trust is a judgment-based form of trust grounded in beliefs about an AI system's competence, reliability, and predictability; it is the most commonly measured trust dimension in this corpus and is distinguished from affective trust (emotion-based) and behavioural trust (reliance-based).

**Sources**: Multiple — see individual source pages.

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Definition

Cognitive trust is grounded in rational evaluation of an agent's characteristics — most commonly:
- **Competence/ability**: perceived capability to perform the task accurately
- **Reliability/predictability**: consistency of performance over time
- **Benevolence**: belief that the AI acts in the user's interest
- **Integrity**: alignment with accepted standards or values

In the AI context, cognitive trust is typically measured through self-report scales (e.g., Jian et al. 2000 trust scale, Madsen & Gregor scale, Körber TiA scale) asking users to rate their confidence in the system's competence and reliability.

## Distinction from Other Trust Constructs

Cognitive trust is one component in a broader trust taxonomy:
- **Affective trust** (see [[affective-trust]]): grounded in emotional bonds and feelings of security rather than rational evaluation
- **Behavioural trust** (see [[behavioural-trust]]): manifested in reliance, adoption, or advice-following behaviour
- **Institutional trust** (see [[institutional-trust]]): trust in the organization or regulatory system that deploys the AI

A recurring finding in this corpus is that cognitive trust (self-reported) dissociates from behavioural trust (reliance): users may rate an AI highly on trust scales while not relying on it (or vice versa). This dissociation is documented by Wang & Ding, Kornowicz & Thommes, Rezaeian et al., and Suffian et al.

## Key Findings

- Perceived understandability (a cognitive appraisal) varies significantly across XAI classes — example-based and counterfactual explanations rate higher than local and global explanations — but perceived reliability does not vary by explanation type (domain: healthcare; Naiseh et al., 2023).
- Cognitive trust (system reliability ratings) increased significantly with two-class example-based XAI compared to one-class or no explanation among domain experts (domain: industrial; Perlmutter et al., 2024).
- Tangibility features (avatar) increase cognitive trust in AI-assisted video interviews; transparency features also increase cognitive trust; immediacy (chatbot) does not (domain: HR; Suen & Hung, 2023).
- Self-reported cognitive trust correlates with but is not the same as calibrated trust: Lee & Chew show counterfactual explanations lower self-reported trust (73 → 45/100) while better calibrating users to actual AI accuracy (domain: healthcare; Lee & Chew, 2023).
- First-impression framing (describing AI as "advanced") increases behavioural alignment with AI outputs without increasing self-reported trust scores, demonstrating that cognitive trust measures may not capture all relevant attitude–behaviour relationships (domain: general/lab; Chu et al., 2023).

## Measurement Instruments

Key self-report instruments used across the corpus:
- **Jian et al. (2000)**: 12-item scale measuring trust and distrust in automation (used by Salehi et al., multiple others)
- **Madsen & Gregor (2000)**: 5-dimension scale (understandability, technical competence, reliability, faith, personal attachment) (used by Naiseh et al.)
- **Körber TiA scale**: trust in automation scale (used by Chu et al., Weitz et al.)
- **NASA-TLX**: often combined with trust measures as a cognitive load control

## Related pages

- [[affective-trust]]
- [[behavioural-trust]]
- [[algorithmic-trust]]
- [[trust-calibration]]
- [[explainability]]
- [[rq1-conceptualizations]]

## References

Chu, Z., Wang, J., & Cao, J. (2023). User judgement of an AI model: The effect of initial AI performance and explanation credibility on subsequent trust and reliance. *CHI Conference on Human Factors in Computing Systems* [details TBD].

Lee, J., & Chew, E. (2023). Understanding the effect of counterfactual explanations on trust and reliance on AI for human-AI collaborative clinical decision making. *Proceedings of the ACM on Human-Computer Interaction* (CSCW2), 7.

Naiseh, M., Al-Thani, D., Jiang, N., & Ali, R. (2023). How the different explanation classes impact trust calibration: The case of clinical decision support systems. *International Journal of Human-Computer Studies* [details TBD].

Perlmutter, S., Gifford, T., & Krening, S. (2024). Impact of example-based XAI for neural networks on trust, understanding, and performance. *International Journal of Human-Computer Studies* [details TBD].

Suen, H. Y., & Hung, K. E. (2023). Building trust in automatic video interviews through anthropomorphism and affective trust. *Technology, Mind, and Behavior* [details TBD].
