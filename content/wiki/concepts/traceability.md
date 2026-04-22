# Traceability

**Summary**: Traceability (operationalized as Subjective Information Processing Awareness, or SIPA) is the user's experienced ability to follow and understand an AI system's processing over time; it is distinct from objective transparency and can diverge significantly from actual comprehension.

**Sources**: Schrills & Franke_How do users experience traceability of AI systems_.pdf

**Research questions addressed**: RQ1, RQ2

**Last updated**: 2026-04-18

---

## Definition

Traceability, as introduced by Schrills & Franke (2023), refers to the subjective experience of being able to follow the AI system's reasoning or processing. It is operationalized through the **SIPA** (Subjective Information Processing Awareness) scale, measuring the user's sense of:
- Knowing what information the AI is using
- Being able to follow how the system arrives at its decisions
- Feeling aware of the system's processing in real time

This is distinct from:
- [[explainability]] (what the system provides)
- [[causability]] (the user's capacity to reach causal understanding)
- Objective comprehension (whether the user can actually predict system behavior)

## Key Findings

Studied in the context of automated insulin delivery (AID) systems for diabetes management:

- SIPA (experienced traceability) develops non-linearly over time — it does not appear immediately upon receiving disclosure information but emerges after approximately 45+ interactions (domain: healthcare/medical devices; Schrills & Franke, 2023).
- High disclosure can produce a **miscalibration** effect: users may develop an inflated sense of traceability (high SIPA) without corresponding gains in objective understanding or system performance.
- Low traceability experience correlates with automation anxiety and lower trust in safety-critical medical contexts (domain: healthcare; Schrills & Franke, 2023).
- The delayed onset of SIPA suggests that transparency information takes time to be integrated into user mental models — a point with implications for longitudinal trust dynamics (see [[rq2-relationships]]).

## Relation to Other Constructs

SIPA can be understood as the phenomenological counterpart to objective explainability. The gap between SIPA and actual comprehension represents a vulnerability: users who feel they can trace system behaviour may over-rely on it even when they cannot predict its failures.

This construct connects to the broader theme of **subjective vs. objective transparency** in this corpus — a recurring finding that self-reported understanding and behavioral trust often dissociate (see also Rezaeian et al.; Wang & Ding).

## Methodological Note

SIPA is measured as a longitudinal construct, not a one-shot self-report. This makes it one of the few transparency constructs in the corpus explicitly designed to capture change over time, aligning with the temporal dynamics highlighted in [[rq2-relationships]].

## Related pages

- [[explainability]]
- [[causability]]
- [[cognitive-trust]]
- [[trust-calibration]]
- [[behavioural-trust]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]

## References

Schrills, T., & Franke, T. (2023). How do users experience traceability of AI systems? *International Journal of Human-Computer Studies* [details TBD].
