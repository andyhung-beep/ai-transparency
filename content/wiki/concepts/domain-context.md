# Domain Context

**Summary**: The domain in which AI is deployed — healthcare, e-commerce, government, defense, HR, and others — shapes both the operationalization of transparency and trust and the magnitude and direction of their relationship; findings from one domain frequently do not generalise to others.

**Sources**: Multiple — see individual source pages.

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Domain context is a fundamental moderator of transparency–trust relationships. The same XAI intervention may increase trust in one domain and have null or negative effects in another. Understanding domain-specific findings is essential before drawing general conclusions.

## Domain Distribution in the Corpus

The 86 sources are distributed across the following domains:

| Domain | Approximate count | Representative sources |
|---|---|---|
| Healthcare / medical | ~25 | Calisto, Diprose, Rezaeian, Naiseh, Hassan, Panigutti, Okolo, Larasati, Xian, Ihongbe, Karagoz, Esmaeilzadeh, Guo & Chen, Yu, Woodcock |
| General/lab (no specific domain) | ~20 | Cau et al., Humer, Spitzer, Leichtmann, Wang & Ding, Conati, Weitz, Bernardo & Seva, Zhang |
| Recommender systems / e-commerce | ~10 | Cramer, Dominguez, Bigras, Musick, Hernandez-Bocanegra, Tintarev & Masthoff, Mourali, Sun (dating) |
| Unmanned vehicles / aviation | ~8 | Bhaskara, Tatasciore (×3), Du, Jansen (×2), Vered |
| HR / recruitment | ~6 | Fleiß, Kornowicz, Zhao, Shulner, Suen & Hung, Duan |
| Government / public services | ~5 | Aoki, Kleizen, Schmager, Salehi, Park |
| Finance / mortgage / e-commerce | ~4 | van Zetten, Cau & Spano, Suffian (×2), Kornowicz |
| Education | ~4 | Conati, Conijn, Li, Nelekar |
| Other (cybersecurity, IP, NLP) | ~4 | Lundberg, Jang & Yoon, Brand, La Gatta |

## Domain-Specific Patterns

### Healthcare

Healthcare is by far the dominant domain. Key patterns:
- [[User-expertise]] (clinical training) is a critical moderator — lay users and clinicians respond very differently to the same explanations.
- Trust thresholds are high: patients often prefer human physicians even when AI performs equivalently (Guo & Chen, 2025).
- Visual explanations (Grad-CAM, saliency maps) are preferred by imaging specialists (Xian et al., 2026).
- More transparency is not always better — Rezaeian et al. document degraded performance with the most detailed explanation level (Rezaeian et al., 2025).

### Government / Citizen AI

- Institutional trust in government strongly dominates transparency effects — ethical AI messaging has near-null impact when institutional trust is absent (Kleizen et al., 2023).
- Process and data transparency serve as micro-level reassurers within a social contract framing (Schmager et al., 2024).

### Human Resources / Recruitment

- Decisions with personal stakes (hiring) elicit strong algorithm aversion that explanations can partially mitigate (Fleiß et al., 2024; Zhao et al., 2024).
- Fairness perceptions are primarily driven by decision outcome (hired/rejected) rather than explanation type (Shulner, 2022).

### Unmanned Vehicles / Aviation

- Automation transparency effects are well-studied through the SAT model with clear level-specific effects.
- Cognitive load and time pressure are particularly salient in this domain.
- Non-linear effects (Level 3 transparency harmful) documented here do not generalise to other domains without empirical testing.

### Recommender Systems

- Foundational work on transparency (Cramer 2008) established the distinction between recommendation acceptance and system trust.
- Explanation effectiveness–satisfaction trade-offs (Tintarev & Masthoff) are well-documented in this domain.

## Non-Generalisability Warning

The corpus strongly supports the conclusion that domain context is not a nuisance variable but a core boundary condition for all transparency–trust claims. Researchers and practitioners should exercise caution when applying findings from one domain to another without empirical validation.

## Related pages

- [[user-expertise]]
- [[perceived-risk]]
- [[institutional-trust]]
- [[algorithmic-transparency]]
- [[rq2-relationships]]
- [[rq3-user-roles]]

## References

Fleiß, J., Hiebl, J., & Müller, S. (2024). Mitigating algorithm aversion in recruiting. *Journal of Business and Psychology* [details TBD].

Guo, B., & Chen, Z. (2025). Investigating whether AI will replace human physicians and understanding the interplay of the source of consultation, health-related stigma, and explanations of diagnoses on patients' evaluations of medical consultations. *Journal of Medical Internet Research*, 27, e66760. https://doi.org/10.2196/66760

Kleizen, B., Van Dooren, W., Verhoest, K., & Tan, J. (2023). Do citizens trust trustworthy artificial intelligence? Experimental evidence on the limits of ethical AI measures in government. *Government Information Quarterly* [details TBD].

Rezaeian, A., Asan, O., & Bayrak, A. E. (2025). The impact of AI explanations on clinicians' trust and diagnostic accuracy in breast cancer. *Applied Ergonomics* [details TBD].

Schmager, S., Osmundsen, K., & Thapa, D. (2024). Exploring citizens' stances on AI in public services: A social contract perspective. *Data & Policy* [details TBD].

Shulner, T. (2022). Fairness, explainability and in-between: Understanding the impact of different explanation methods on non-expert users' perceptions of fairness. *Ethics and Information Technology* [details TBD].

Xian, Y., Mehandjiev, N., Constantinides, M., Chen, Y., Quboa, Q., & Kitchen, G. (2026). Clinician preferences for explainable AI in critical care. *International Journal of Medical Informatics*, 210 [details TBD].

Zhao, Y., Xu, L., Yu, F., & Jin, W. (2024). Perceived opacity leads to algorithm aversion in the workplace. *Acta Psychologica Sinica*, 56(4), 497–514.
