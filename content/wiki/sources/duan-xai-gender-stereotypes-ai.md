# Mitigating Gender Stereotypes Toward AI Agents Through an eXplainable AI (XAI) Approach

**Source file**: [Original article](../../raw/Duan et al._Mitigating gender stereotypes toward AI agents.pdf)

**Summary**: A factorial video-vignette online experiment (N = 350) showing that feature-contribution XAI explanations reduce participants' gender stereotyping of AI agents by increasing understanding of how AI works and decreasing perceived humanlikeness, with implications for both XAI design and social equity.

**Sources**: Duan et al._Mitigating gender stereotypes toward AI agents.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Duan, McNeese, Freeman, and Li (2024), published in the *Proceedings of the ACM on Human-Computer Interaction (CSCW2)*, examine whether XAI can mitigate gender stereotypes toward AI agents. The study addresses two research questions: whether people apply gender stereotypes to modern LLM-style AI agents (RQ0), and whether XAI can reduce those stereotypes (RQ1 in the paper).

The study used an 18-condition fully between-subjects design: 3 (agent gender: woman, man, gender-neutral) × 3 (task gender: feminine, masculine, gender-neutral) × 2 (XAI presence/absence). 350 Prolific participants from the US were exposed to video vignettes depicting a ChatGPT-style AI agent providing decision support via a comparative table. XAI conditions featured **feature-contribution explanations** (quantifying the weight of each parameter in the agent's final decision), explicitly chosen over counterfactual or example-based explanations because feature contribution highlights the difference between AI and human decision-making. The study also conducted 9 qualitative interviews.

Key dependent variables: understanding of how the agent works, cognitive effort, perceived humanlikeness, domain-specific trust in the agent, conformity to the agent's decision, and ratings of gender stereotypical traits (communion, agency, competence).

## Key Findings

- XAI significantly increased participants' self-reported understanding of how the agent works (F[1,332] = 50.32, p < .001, η² = .13; XAI M = 4.98 vs. non-XAI M = 3.81 on 7-point scale). (source: Duan et al._Mitigating gender stereotypes toward AI agents.txt; domain: human-computer interaction / social AI)
- XAI significantly reduced perceived humanlikeness of the agent (F[1,332] = 11.72, p < .001; XAI M = 3.29 vs. non-XAI M = 3.98), with partial mediation through increased understanding (Sobel z = 2.49, p = .013). (source: Duan et al._Mitigating gender stereotypes toward AI agents.txt; domain: human-computer interaction / social AI)
- In non-XAI conditions, participants were significantly more likely to conform to a woman agent's decision on a stereotypically feminine topic (OR = 0.05 vs. baseline, p = .002) and to a man agent on a masculine topic (OR = 0.162, p = .016)—demonstrating implicit gender stereotyping through conformity. (source: Duan et al._Mitigating gender stereotypes toward AI agents.txt; domain: human-computer interaction / social AI)
- XAI eliminated this gender-stereotyped conformity pattern; the interaction between agent gender and task gender was no longer a significant predictor of conformity in XAI conditions (p = .897). (source: Duan et al._Mitigating gender stereotypes toward AI agents.txt; domain: human-computer interaction / social AI)
- Domain-specific trust did not show gender-stereotyped patterns, suggesting participants corrected for explicit stereotypes when directly asked—but implicit stereotypes were visible in conformity and trait ratings. (source: Duan et al._Mitigating gender stereotypes toward AI agents.txt; domain: human-computer interaction / social AI)
- Non-XAI conditions produced significant gendered trait attribution: woman agents rated higher on communion traits (affectionate, compassionate, sensitive, emotional, tender, sympathetic) and man agents higher on agency traits (aggressive, courageous). XAI conditions showed no such differences (except "decisive"). (source: Duan et al._Mitigating gender stereotypes toward AI agents.txt; domain: human-computer interaction / social AI)
- XAI had a trend (non-significant) toward increasing domain-specific trust (p = .06; XAI M = 5.41 vs. non-XAI M = 5.06), suggesting explanations may slightly boost trust overall even while reducing anthropomorphism. (source: Duan et al._Mitigating gender stereotypes toward AI agents.txt; domain: human-computer interaction / social AI)
- Qualitative interviews revealed that XAI worked by drawing attention to impartial data-driven processes, reducing the salience of gender cues and positioning the agent as a calculator rather than a gendered social actor. (source: Duan et al._Mitigating gender stereotypes toward AI agents.txt; domain: human-computer interaction / social AI)
- Gender-neutral agent design (non-binary) did not eliminate gender stereotypes; participants still attributed gendered traits to the gender-neutral agent, indicating de-gendering alone is insufficient. (source: Duan et al._Mitigating gender stereotypes toward AI agents.txt; domain: human-computer interaction / social AI)

## Transparency Constructs

The study employs **feature-contribution XAI** (a quantitative transparency technique that shows how each input feature weighted the AI's decision), mapped onto [[explainability]] and [[algorithmic-transparency]]. The authors deliberately avoid example-based or counterfactual explanations because those styles mimic human reasoning and may reinforce rather than disrupt anthropomorphic heuristics. This finding has theoretical implications for [[causability]] (user understanding of causal mechanisms) and for how different transparency types can serve distinct social functions beyond prediction explanation.

## Trust Constructs

Trust is operationalised in two ways: (1) **domain-specific trust**—a 5-item scale measuring willingness to take the agent's advice on a given topic (α = .91), capturing a [[cognitive-trust]] / competence-related dimension; and (2) **conformity**—a behavioural measure of whether participants changed their decision to match the agent's, indexing [[behavioural-trust]]. The divergence between these two measures—explicit domain trust showed no stereotyping, but behavioural conformity did—illustrates the importance of multi-method trust assessment and the gap between self-reported and enacted trust relevant to [[trust-calibration]].

## Relevance to Research Questions

**RQ1**: The study introduces an underexplored operationalisation of XAI effects: not as accuracy-improving or uncertainty-reducing, but as a mechanism to disrupt social heuristics (gender stereotyping). Trust is split into explicit self-report and implicit conformity behaviour. This expands the conceptual landscape in [[rq1-conceptualizations]] by showing transparency constructs can be defined and measured with respect to social bias reduction.

**RQ2**: XAI's effect on trust is conditional on what aspect of trust is measured: it shows a non-significant trend toward higher domain trust while simultaneously reducing humanlikeness (which could decrease affective or social trust). The relationship is therefore non-simple and depends on the trust facet. The complete elimination of stereotyped conformity in XAI conditions represents a strong conditional effect, contributing to [[rq2-relationships]].

**RQ3**: The study explicitly examines how **need for cognition** and pre-existing **attitudes toward sex roles** moderate responses, and domain knowledge is a covariate. Women and gender non-binary participants were more likely to consciously articulate concerns about gendered AI; men showed more implicit stereotyping. These findings directly address how user characteristics (gender identity, cognitive style) moderate trust and XAI responses, contributing to [[rq3-user-roles]].

## Related pages

- [[explainability]]
- [[algorithmic-transparency]]
- [[cognitive-trust]]
- [[behavioural-trust]]
- [[trust-calibration]]
- [[user-expertise]]
