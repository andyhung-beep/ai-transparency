# The Effects of Explanations in Automated Essay Scoring Systems on Student Trust and Motivation

**Source file**: [Original article](../../raw/Conijn et al._The effects of explanations in automated essay scoring systems.pdf)

**Summary**: A between-subjects experiment (N = 150 university students) comparing no explanation, an accuracy statement, and a full-text global explanation in an automated essay scoring (AES) context, finding that neither explanation type increased student trust or motivation compared to no explanation, while the difference between the system grade and students' self-estimated grade had a large non-linear effect on both outcomes.

**Sources**: Conijn et al._The effects of explanations in automated essay scoring systems.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Conijn, Kahr, and Snijders (2023) report one of the first experimental studies on the use of XAI in an automated essay scoring (AES) system. Motivated by the ethical imperative for transparency in learning analytics, the authors designed a user-centred study where students wrote a short argumentative essay, received an automated grade (from a Wizard-of-Oz system), and then self-estimated their grade before and after seeing the system grade. Participants were randomly assigned to one of three conditions:

1. **Control**: No explanation — only the system grade was shown.
2. **Accuracy statement**: A brief confidence statement noting the system is accurate approximately 90% of the time.
3. **Full-text explanation**: A detailed global explanation describing the features the system uses (content, structure, cohesiveness, plagiarism, basic writing features) and how it was trained, including worked examples.

The explanations were designed using a needs-elicitation study with students (two focus groups, N = 11) combined with existing XAI guidelines (Kulesza et al., 2015; Lim & Dey, 2010; Mueller et al., 2021). Trust was measured via the Trust in Automation (TiA) scale (subjective) and the Weight of Advice (WoA) metric (behavioural, measuring grade adaptation). Motivation was measured via the Intrinsic Motivation Inventory interest/enjoyment subscale and willingness to continue writing.

## Key Findings

- Neither the accuracy statement nor the full-text explanation increased subjective trust (TiA) compared to the control condition (F(2,147) = 2.14, p = .12). (Domain: higher education / essay assessment)
- Neither explanation type increased behavioural trust (willingness to adapt self-estimated grade toward the system grade) compared to the control condition. (Domain: education)
- Neither explanation type increased overall intrinsic motivation; however, the accuracy statement showed a small positive effect on motivation compared to no explanation when controlling for other variables (B = 2.85, SE = 1.29, p = .03), but this effect was reduced for students with higher Need for Cognition. (Domain: education)
- The difference between the system-assigned grade and the student's self-estimated grade had a large, non-linear (quadratic) effect on trust: trust was lower when the system gave a lower grade than the student expected; this effect diminished when the system grade was much higher than expected. (Domain: education)
- Students adapted their grade more often (higher behavioural trust) when the absolute discrepancy between their estimate and the system grade was larger, but this effect was also non-linear (diminishing for very large discrepancies). (Domain: education)
- Students with higher propensity to trust technology showed higher subjective trust (B = 0.25, p = .020), replicating the role of dispositional trust. (Domain: education)
- Students spent approximately 2 minutes 40 seconds on the full explanation and 61 seconds on the accuracy statement, indicating reasonable engagement with the materials.
- The full explanations were rated as somewhat overwhelming by students (despite being designed with user input), while the accuracy statement was considered clearer.
- Contrary to findings from Conati et al. (2021) and Ooge et al. (2022) in ITS contexts, global explanations did not increase trust, suggesting context dependency. The difference in local versus global explanation type is highlighted as a key factor.

## Transparency Constructs

The study compares two forms of [[algorithmic-transparency]]:

- **Accuracy statement**: A confidence/accuracy claim (the system is accurate 90% of the time) — a minimal form of [[outcome-transparency]] or [[uncertainty-visualization]] without process detail.
- **Full-text global explanation**: A [[process-transparency]] intervention describing the system's features, training methodology, and example feature-grade relationships. Covers "What", "What If", "Inputs", and "Outputs" in Lim & Dey's (2010) Intelligibility Toolkit framework, reaching level 4 on Mueller et al.'s (2021) Self-Explanation Scorecard.

A key limitation acknowledged is the absence of **local** [[explainability]] (essay-specific explanations) and [[counterfactual-explanations]] ("Your grade would have been higher if..."), which the authors argue may be more relevant to students and more effective at building trust.

## Trust Constructs

The study employs a dual-operationalisation of trust:

- **Subjective [[cognitive-trust]]**: Trust in Automation (TiA) scale (Jian et al., 2010), 12 items on a 1–7 scale (α = .88).
- **[[behavioural-trust]]**: Weight of Advice (WoA) — the degree to which students adjusted their self-estimated grade in the direction of the system grade after seeing it.

The paper finds these two measures are not significantly correlated (B = 0.12, p = .44), reinforcing the finding from [[chu-user-judgement-ai-model]] that self-reported trust and trust-as-behaviour can dissociate. Both measures are used as dependent variables independently.

The study also measures [[dispositional trust]] (Propensity to Trust Technology, PTT scale, Jessup et al., 2019) as a covariate, finding a significant positive effect on subjective trust.

## Relevance to Research Questions

**RQ1**: Operationalises transparency as both an accuracy statement and a full-text global explanation in an educational AES context. Operationalises trust via TiA (subjective) and WoA (behavioural). Distinguishes between dispositional trust (PTT) and situational/contextual trust (TiA). Explicitly notes that transparency means different things in different ethical frameworks (informed consent vs. algorithmic accountability).

**RQ2**: The null finding is itself a significant contribution to RQ2: neither global explanation type reliably increased trust or motivation compared to no explanation. The dominant predictor of trust was the grade discrepancy (a system outcome variable), not the explanatory information provided. This represents a conditional/moderating effect where the outcome quality overwhelms any transparency effect — a pattern that may be domain-specific to high-stakes grading contexts where students have strong prior beliefs about their own grade. The non-linear grade-discrepancy effect on trust is an important finding about when transparency might and might not work.

**RQ3**: The study focused on students as a single stakeholder group and found no significant moderating effect of Need for Cognition on trust (though an interaction with the accuracy statement on motivation was found). The authors explicitly call for future work examining teachers as a different stakeholder group, whose response to explanations may differ substantially. This points to a gap in the literature regarding [[user-expertise]] and role as moderators in educational AI contexts.

## Related pages

- [[algorithmic-transparency]]
- [[outcome-transparency]]
- [[counterfactual-explanations]]
- [[cognitive-trust]]
- [[behavioural-trust]]
- [[dispositional trust]]
- [[domain-context]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]
- [[rq3-user-roles]]
