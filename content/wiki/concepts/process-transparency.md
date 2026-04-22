# Process Transparency

**Summary**: Process transparency refers to providing users with information about how an AI system works, what data it uses, and how it reaches decisions — as opposed to just communicating the decision outcome; user-controlled (demand-driven) access to process information consistently outperforms sequential disclosure.

**Sources**: Multiple — see individual source pages.

**Research questions addressed**: RQ1, RQ2

**Last updated**: 2026-04-18

---

## Definition

Process transparency discloses the *mechanisms* by which an AI system operates: its inputs, processing steps, decision logic, and constraints. It is distinct from:
- [[outcome-transparency]] (what the decision was)
- [[explainability]] (why a particular decision was made for a particular case)
- [[disclosure]] (that AI was involved)

Process transparency can be passive (always displayed) or demand-driven (accessible on request).

## Key Finding: Demand-Driven vs. Sequential Transparency

Vered et al. (2020) compare two interface designs for a military multi-vehicle management system:
- **Sequential transparency (ST)**: users step through explanation layers in a fixed order
- **Demand-driven transparency (DDT)**: users access transparency information when and as needed

DDT significantly improved operator trust and maintained or improved task performance without increasing workload, relative to ST. The key insight is that *user control over information access* — not just the availability of information — is critical to transparency benefits. Forcing users through sequential disclosure overwhelms them; letting them pull information when needed allows better self-regulation (domain: defense/unmanned vehicles; Vered et al., 2020).

## Timing of Process Transparency

Du et al. (2019) show that for autonomous vehicles, *when* process information is provided matters as much as *what* is provided:
- Explanations provided **before** an AV action significantly increased trust and preference
- Explanations provided **after** an action had no significant benefit over no explanation

This suggests process transparency is most effective when it helps users anticipate and prepare for AI behavior, not when it retrospectively justifies decisions already made (domain: autonomous vehicles; Du et al., 2019).

## Automation Transparency Levels

In the automation literature, process transparency is structured hierarchically (the SAT model):
- **Level 1**: What the automation perceives
- **Level 2**: What the automation will do
- **Level 3**: Projected outcomes

Intermediate levels (1+2) improve reliance accuracy; the highest level (1+2+3) introduces automation bias — an inverted-U effect (domain: defense/unmanned vehicles; Bhaskara et al., 2021).

## Social Contract Framing

Schmager et al. apply a social contract lens to process transparency in public services, identifying it as a micro-level reassurance mechanism: citizens accept AI in government services more readily when they can see how their data is used and how decisions are made, particularly when institutional trust is already present (domain: government/public services; Schmager et al., 2024).

## Related pages

- [[algorithmic-transparency]]
- [[outcome-transparency]]
- [[uncertainty-visualization]]
- [[disclosure]]
- [[trust-calibration]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]

## References

Bhaskara, A., Skinner, M., & Loft, S. (2021). Effect of automation transparency in the management of multiple unmanned vehicles. *Human Factors*, 63(2), 173–189 [details TBD].

Du, N., Haspiel, J., Zhang, Q., Tilbury, D., Pradhan, A. K., Yang, X. J., & Robert, L. P. (2019). Look who's talking now: Implications of AV's explanations on driver's trust, AV preference, anxiety and mental workload. *Transportation Research Part C: Emerging Technologies*, 104, 428–442.

Schmager, S., Osmundsen, K., & Thapa, D. (2024). Exploring citizens' stances on AI in public services: A social contract perspective. *Data & Policy* [details TBD].

Vered, M., Shani, G., & Karpas, E. (2020). Demand-driven transparency for monitoring intelligent agents. *AAAI Conference on Artificial Intelligence* [details TBD].
