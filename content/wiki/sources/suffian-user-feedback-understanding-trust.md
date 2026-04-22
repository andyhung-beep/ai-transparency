# The Role of User Feedback in Enhancing Understanding and Trust in Counterfactual Explanations for Explainable AI

**Source file**: [Original article](../../raw/Suffian et al._The role of user feedback in enhancing understanding and trust.pdf)

**Summary**: A user study with 70 participants comparing a user-feedback-based counterfactual explanation method (UFCE) against a standard diverse counterfactual approach (DiCE) and a control group, finding that UFCE significantly improves task performance, feature understanding, actionability, and reliance on AI suggestions.

**Sources**: Suffian et al._The role of user feedback in enhancing understanding and trust.pdf

**Research questions addressed**: RQ1, RQ2

**Last updated**: 2026-04-18

---

## Overview

Suffian et al. (2025), published in the *International Journal of Human-Computer Studies*, present an empirical user study that extends the FCE framework (see [[suffian-fce-counterfactual-feedback]]) by introducing and evaluating UFCE (User Feedback-based Counterfactual Explanation) against DiCE (Diverse Counterfactual Explanations) and a no-explanation control group. The study uses a game-inspired platform called "Alien Nutri-Solver" in which participants (N = 70 after quality assurance; N = 101 recruited) must learn which nutrients improve a fictional creature's fitness — an unfamiliar domain designed to prevent prior knowledge from confounding results. Three conditions: control (no explanations), UFCE (user-feedback-driven counterfactuals), DiCE (automated diverse counterfactuals). The platform is open-sourced with data shared for reproducibility.

UFCE improves upon DiCE by allowing users to specify which features they want to modify and the acceptable ranges, so counterfactuals are constrained to feasible and personally relevant modifications. DiCE generates diverse counterfactuals without such constraints. The study evaluates understanding, task performance, satisfaction, and trust as outcomes.

## Key Findings

- **Explanations improve feature understanding**: participants who received either UFCE or DiCE explanations correctly identified relevant and irrelevant input features significantly better than the control group (H(2) = 9.920, p = 0.007); no significant difference between UFCE and DiCE on this measure (domain: synthetic/game-based).
- **UFCE produces highest task performance**: significant differences in final fitness scores (H(2) = 24.729, p < 0.0001); post-hoc tests show UFCE > DiCE (p = 0.022) > control (p = 0.000002). UFCE users were also better at targeting the correct features (plants) in their changes (domain: synthetic/game-based).
- **UFCE explanations are more actionable than DiCE**: significant difference on actionability item (U = 367.5, p = 0.038, r = 0.298); UFCE users rated suggestions as more actionable (M = 3.85) than DiCE users (M = 3.39) (domain: synthetic/game-based).
- **UFCE users relied more on suggestions**: significant difference in explanation usage (U = 194.5, p = 0.026, r = -0.316), with UFCE users reporting lower non-usage of suggestions than DiCE users (domain: synthetic/game-based).
- **No significant differences between UFCE and DiCE on satisfaction or trust self-report items** individually (after multiple comparisons), though UFCE users consistently showed numerically higher means across satisfaction and trust items. The study was adequately powered for large effects (power = 0.91) but underpowered for medium effects (power = 0.65), so medium-sized differences may be genuine but undetected.
- Control group universally reported needing explanatory support and disagreed that they could understand the system without help, demonstrating the necessity of XAI in unfamiliar domains (domain: synthetic/game-based).
- The GDPR and EU AI Act are cited as regulatory drivers for user-centric XAI, underscoring the policy relevance of the findings.

## Transparency Constructs

The study evaluates two implementations of **[[counterfactual-explanations]]**:

- **UFCE** (User Feedback-based Counterfactual Explanation): User specifies features to modify and acceptable ranges; counterfactuals are searched within that user-defined feasibility space. Combines [[counterfactual-explanations]] with participatory design, yielding higher actionability and reliance than automated alternatives.
- **DiCE** (Diverse Counterfactual Explanations): Automated generation of diverse counterfactuals without user-defined constraints. A widely used baseline in the [[counterfactual-explanations]] literature.

Both methods operationalize **[[explainability]]** by showing how minimal input changes alter model outputs — a contrastive form of transparency. The user-feedback loop in UFCE also contributes to **[[process-transparency]]**: users actively participate in defining the explanation space, gaining insight into which features the model treats as influential. The game platform design provides **[[outcome-transparency]]** by showing the immediate fitness consequences of dietary changes fed back to the creature (Shub).

## Trust Constructs

Trust is assessed through post-game survey items (items 15–20):

- **Item 15** (asked of all groups): General trust in the Alien Nutri-Solver framework. Enables comparison across all three groups including control.
- **Items 16–20** (explanation groups only): Trust in explanations, confidence in explanations, perceived safety when following suggestions, and reliance behavior.

Trust constructs represented:
- **[[cognitive-trust]]**: Items addressing confidence in and perceived reliability of the counterfactual suggestions.
- **[[behavioural-trust]]** (reliance): Operationalized through actual suggestion usage during gameplay (objective) and self-reported non-usage (subjective). UFCE users showed significantly higher reliance than DiCE users.
- **[[appropriate-reliance]]**: The study's design — game-based task performance — enables a form of reliance calibration assessment: users following appropriate suggestions should achieve higher fitness scores.

The distinction between UFCE's superiority on *objective* reliance and task performance vs. the absence of significant *self-reported* trust differences is noteworthy: behavioural trust and self-reported trust may diverge (source: Suffian et al._The role of user feedback in enhancing understanding and trust.pdf).

## Relevance to Research Questions

**RQ1**: Extends the operationalization of counterfactual transparency by comparing two different instantiations — user-driven vs. automated — on multiple outcomes (understanding, performance, actionability, reliance, satisfaction, trust). The UFCE/DiCE comparison provides a rare controlled test of how the *generation process* of a counterfactual explanation affects user outcomes. The game-based platform is a novel measurement approach for XAI evaluation (source: Suffian et al._The role of user feedback in enhancing understanding and trust.pdf).

**RQ2**: Demonstrates a **positive effect of human-in-the-loop counterfactual explanations on behavioural trust** (reliance) and task performance, with UFCE outperforming DiCE. However, self-reported satisfaction and trust items show no significant UFCE vs. DiCE differences, suggesting the relationship between explanation quality and self-reported trust is weaker than the relationship with behavioural trust. This divergence between attitudinal and behavioural trust is an important conditional effect (domain: synthetic/game-based learning; source: Suffian et al._The role of user feedback in enhancing understanding and trust.pdf).

**RQ3**: Not directly addressed. The sample is primarily 18–24-year-old students; user expertise or AI literacy differences are not examined as moderators. The unfamiliar domain was specifically chosen to control for prior knowledge, but this means the study cannot speak to how expertise shapes the counterfactual explanation–trust relationship (source: Suffian et al._The role of user feedback in enhancing understanding and trust.pdf).

## Related pages

- [[counterfactual-explanations]]
- [[explainability]]
- [[behavioural-trust]]
- [[cognitive-trust]]
- [[appropriate-reliance]]
- [[rq2-relationships]]
