# Disclosure / Notification

**Summary**: Disclosure refers to informing users (or third parties) that AI was used in producing an output or decision; unlike explainability, disclosure concerns the fact of AI involvement rather than the logic behind it, and can paradoxically erode trust.

**Sources**: Schilke & Reimann_The transparency dilemma.pdf; Liu 2021_In AI we trust_.pdf; Sun et al._Understanding trust toward human versus AI-generated health information.pdf

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Definition

Disclosure is a form of transparency that operates at the level of *identifying* AI involvement, rather than *explaining* it. Disclosures can be:
- **Voluntary**: the AI user proactively reveals AI assistance (Schilke & Reimann)
- **Mandatory/regulatory**: required by policy or law
- **Source labeling**: content is tagged as AI-generated (Sun et al.)
- **Real vs. placebic**: genuine disclosure of AI logic vs. superficial or uninformative labels (Liu 2021)

Disclosure is distinct from [[explainability]] (which explains the AI's reasoning) and [[algorithmic-transparency]] (which concerns the overall transparency of the algorithmic process).

## Key Findings

### The Transparency Dilemma

Schilke & Reimann (2025) conducted 13 experiments showing that humans who disclose AI assistance in their work are trusted significantly less than those who do not, across diverse contexts (education, hiring, finance, legal, creative). The mechanism is legitimacy erosion: disclosure reduces perceived legitimacy of the actor, which reduces interpersonal trust. This effect is robust across different disclosure framings (qualified, intent-based, error-acknowledging) and is even stronger when AI use is discovered by a third party rather than voluntarily disclosed (domain: organizational/general; Schilke & Reimann, 2025).

This finding directly contradicts the intuition that transparency always promotes trust. It does not mean disclosure is wrong — it means the social context of disclosure matters enormously.

### Real vs. Placebic Transparency

Liu (2021) distinguishes between *real transparency* (genuine disclosure of how an AI system works) and *placebic transparency* (disclosure that feels informative but provides no actionable information). Real transparency reduces uncertainty and increases trust; placebic transparency increases use intention through heuristic processing but does not reduce uncertainty (domain: general/recommendation systems; Liu, 2021).

### Source vs. Label Dissociation

Sun et al. (2026) show that the source of health information (LLM vs. human) and the label attached to it (AI-generated vs. human-authored) affect trust independently and in opposite directions: LLM content is objectively trusted more, but content *labeled* as AI-generated is trusted less. This dissociation reveals that disclosure effects depend on what is disclosed and how it is framed, not just whether AI is mentioned (domain: healthcare/health information; Sun et al., 2026).

## Moderators

- **Technology attitudes**: Users with favorable attitudes toward technology show attenuated (but not eliminated) trust penalties from disclosure (Schilke & Reimann, 2025).
- **Perceived AI accuracy**: Higher perceived accuracy weakens the disclosure penalty (Schilke & Reimann, 2025).
- **Information type**: Effects of source labeling vary by health information category (general, symptom, treatment) but remain directionally consistent (Sun et al., 2026).

## Implications for Research Design

Many studies on [[explainability]] implicitly disclose AI involvement through the study design. The disclosure effect identified by Schilke & Reimann suggests that baseline trust in AI-disclosed conditions may already be lower than in non-disclosed conditions, potentially confounding findings about explanation effects.

## Related pages

- [[explainability]]
- [[algorithmic-transparency]]
- [[cognitive-trust]]
- [[institutional-trust]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]

## References

Liu, P. (2021). In AI we trust? Effects of agency locus and transparency on uncertainty reduction in human–AI interaction. *Journal of Computer-Mediated Communication*, 26(6), 384–402 [details TBD].

Schilke, O., & Reimann, M. (2025). The transparency dilemma: How AI disclosure erodes trust. *Organizational Behavior and Human Decision Processes* [details TBD].

Sun, Y., Zhou, Y., Shi, M., Lim, K. H., & Li, Y. (2026). Understanding trust toward human versus AI-generated health information through behavioral and physiological sensing. *International Journal of Human-Computer Studies* [details TBD].
