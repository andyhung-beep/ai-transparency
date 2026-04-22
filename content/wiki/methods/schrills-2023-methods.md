# Schrills 2023 — Methods

**Summary**: A controlled laboratory experiment (N = 80) with three levels of information disclosure in an automated insulin delivery (AID) simulation, introducing and validating the Subjective Information Processing Awareness (SIPA) scale to measure users' experienced traceability of AI systems over time.

**Sources**: Schrills & Franke_How do users experience traceability of AI systems_.pdf

**Research questions addressed**: RQ1 / RQ2 / RQ3

**Last updated**: 2026-04-19

---

## Study design
experimental (between-subjects, three-condition; longitudinal observation across 60+ trials)

## Sample
- N: 80
- Population: general public (non-expert participants; diabetes domain familiarity not specified)
- Domain: healthcare / diabetes management (automated insulin delivery systems)
- Country / region: not reported
- Recruitment method: not reported

## Transparency operationalization
- Type: process transparency / information disclosure (input-feature visibility)
- Manipulation or measure: Between-subjects manipulation across three levels of information disclosure: (1) LowID — 2 attributes of the AID insulin calculation algorithm shown; (2) MedID — 4 attributes shown; (3) HighID — 6 attributes shown. Participants observed AID simulation making insulin dosage calculations and predicted system outputs over 60+ trials. Time-on-task recorded as an objective measure of information processing effort.
- Scale / instrument name: not applicable (experimental manipulation)
- Number of items: not applicable

## Trust operationalization
- Type: cognitive (self-reported traceability and trust)
- Measure: (1) SIPA (Subjective Information Processing Awareness) — a multi-faceted scale developed and validated in this study, comprising three facets: perceived transparency (ability to understand what information the AI uses), perceived predictability (ability to anticipate system outputs), and perceived controllability (ability to influence system behavior); (2) Trust — measured as a self-report scale showing strong convergent validity with SIPA; (3) Subjective workload — NASA-TLX; (4) Prediction performance — objective accuracy of participants' predictions of AID outputs. Note: SIPA is explicitly distinguished from objective accuracy/comprehension — it measures experienced traceability, not actual knowledge.
- Scale / instrument name: SIPA (Subjective Information Processing Awareness; developed by authors); NASA-TLX (workload)
- Number of items: not reported (SIPA item count not specified in source)
- Behavioural vs self-report: both used (SIPA and trust = self-report; prediction performance = behavioural)

## Moderators and covariates tested
- Attitudes toward AI (AIA scale): measured; significantly related to SIPA at initial observation and after the performance block — relevant to RQ3
- Time / trial block: within-subjects repeated measurement; SIPA generally decreased over time across conditions, suggesting extended interaction erodes rather than builds experienced traceability
- User expertise / familiarity with AID therapy: noted as a potential moderator in discussion but not directly tested — relevant to RQ3

## Statistical approach
- Primary analysis method: mixed-effects models / repeated-measures analysis (for SIPA and trust trajectories over time); scale validation via factor analysis (SIPA development); correlation analyses (SIPA–trust convergent validity)
- Software: not reported
- Key model fit or effect size reported: SIPA–trust correlation reported as strong (specific r not provided in source); time-on-task comparison (HighID > 2× LowID); significance thresholds reported for condition × time interactions

## Author-noted limitations
- Participants were not diabetes patients or AID users; ecological validity limited
- No direct measure of objective understanding (only subjective SIPA); miscalibration between perceived and actual understanding cannot be fully disentangled
- Short-term laboratory study; long-term traceability development not captured
- SIPA scale requires further validation across domains beyond AID systems
- Less experienced or less engaged users particularly vulnerable to misleading SIPA inflation under high information disclosure — subgroup effects not formally tested

## Related pages
- [[schrills-franke-traceability-ai-systems]]
- [[traceability]]
- [[trust-calibration]]
- [[appropriate-reliance]]
- [[cognitive-trust]]
- [[user-expertise]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]
