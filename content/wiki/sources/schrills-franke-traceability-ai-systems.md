# How Do Users Experience Traceability of AI Systems? Examining Subjective Information Processing Awareness in Automated Insulin Delivery (AID) Systems

**Source file**: [Original article](../../raw/Schrills & Franke_How do users experience traceability of AI systems_.pdf)

**Summary**: Schrills and Franke introduce Subjective Information Processing Awareness (SIPA) as a construct for measuring users' experienced traceability of AI systems, finding that higher information disclosure affects SIPA only after repeated exposure and may create miscalibration between perceived and actual understanding.

**Sources**: Schrills & Franke_How do users experience traceability of AI systems_.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Published in *ACM Transactions on Interactive Intelligent Systems* (December 2023), this study examines how users experience *traceability*—the subjective sense of being able to follow and understand AI-system reasoning—in the context of automated insulin delivery (AID) systems for type 1 diabetes management. The authors develop and validate a new multi-faceted scale (SIPA) and test it in a controlled experiment (N = 80) with three levels of information disclosure: Low (LowID), Medium (MedID), and High (HighID).

Participants observed an AID simulation making insulin dosage calculations and predicted the system's outputs over 60+ trials. The dependent variables were SIPA (perceived transparency, predictability, controllability), trust, subjective workload (NASA-TLX), and prediction performance.

## Key Findings

- Higher information disclosure (HighID vs. LowID) did not immediately affect SIPA; a significant difference in perceived transparency emerged only after 45 observations, indicating that traceability experience develops over repeated interactions (domain: healthcare/diabetes management). (source: Schrills & Franke_How do users experience traceability of AI systems_.txt)
- Participants in the HighID condition spent more than twice as long on prediction tasks compared to LowID participants, confirming increased cognitive processing time with more information (domain: healthcare). (source: Schrills & Franke_How do users experience traceability of AI systems_.txt)
- Contrary to expectations, SIPA ratings generally *decreased* over time across conditions, suggesting that extended interaction with complex AI systems may erode rather than build subjective processing awareness (domain: healthcare). (source: Schrills & Franke_How do users experience traceability of AI systems_.txt)
- SIPA was strongly correlated with trust and satisfaction with explanations, supporting the construct validity of the scale (domain: healthcare). (source: Schrills & Franke_How do users experience traceability of AI systems_.txt)
- Despite more information available in MedID and HighID conditions, prediction *performance* did not differ significantly between conditions, indicating information overload may negate the performance benefit of additional disclosures (domain: healthcare). (source: Schrills & Franke_How do users experience traceability of AI systems_.txt)
- High information disclosure can produce miscalibration: users in HighID felt more transparent understanding but did not perform better, raising concerns about over-trust driven by information richness (domain: healthcare). (source: Schrills & Franke_How do users experience traceability of AI systems_.txt)
- A performance/prediction task (asking users to actively predict outputs) triggered a readjustment of trust and SIPA, suggesting task design can be used to calibrate experienced traceability (domain: healthcare). (source: Schrills & Franke_How do users experience traceability of AI systems_.txt)
- Attitudes toward AI (AIA) were significantly related to SIPA at initial observation and after the performance block, indicating individual user attitudes moderate traceability experience (domain: healthcare). (source: Schrills & Franke_How do users experience traceability of AI systems_.txt)

## Transparency Constructs

This paper offers one of the most detailed operationalizations of [[traceability]] in the XAI literature, defining it as a multi-faceted subjective construct (SIPA) comprising:
- *Transparency* facet: perceived ability to understand what information the AI uses
- *Predictability* facet: perceived ability to anticipate system outputs
- *Controllability* facet: perceived ability to influence system behavior

SIPA is explicitly distinguished from objective accuracy or comprehension: it measures *experienced* traceability, not actual knowledge. The three levels of [[disclosure]] correspond to showing 2, 4, or 6 attributes used in the insulin calculation algorithm. This is a form of [[process-transparency]] focused on input-feature visibility.

## Trust Constructs

Trust is measured as a dependent variable and shows strong convergent validity with SIPA facets, supporting the idea that experienced traceability is a key antecedent of [[cognitive-trust]] in AI systems. The study observes a trust development trajectory across three phases (learning, adjustment, fine-tuning), with performance prediction tasks triggering trust readjustment—consistent with [[trust-calibration]] processes. The miscalibration finding (high information → inflated SIPA without performance gain) relates directly to concerns about [[appropriate-reliance]].

## Relevance to Research Questions

**RQ1**: Introduces SIPA as a new operationalization of experienced traceability, a user-side transparency construct distinct from objective explainability or comprehension accuracy. Demonstrates strong correlation between SIPA and trust, supporting traceability as a theoretically coherent antecedent of trust.

**RQ2**: Documents a delayed and non-linear relationship between information disclosure and experienced transparency: more information does not linearly increase SIPA, and initial disclosure level differences only emerge after many repetitions. The miscalibration effect—more information increases perceived understanding without improving actual performance—points to a potential negative effect of high transparency on appropriate reliance.

**RQ3**: Notes that user expertise (e.g., familiarity with AID therapy, education level) may moderate the relationship between information disclosure and traceability experience, but does not directly test this. Flags that less engaged or less experienced users may be particularly vulnerable to misleading SIPA inflation under high information disclosure conditions—an important consideration for inclusive XAI design.

## Related pages

- [[traceability]]
- [[trust-calibration]]
- [[appropriate-reliance]]
- [[cognitive-trust]]
- [[user-expertise]]
- [[rq2-relationships]]
