# RQ3: How User Expertise and Role Are Accounted For

**Summary**: This page synthesizes evidence on how user expertise, professional role, AI literacy, and related user characteristics moderate the transparency–trust relationship across the 86 sources in this corpus.

**Sources**: All 86 source documents.

**Research questions addressed**: RQ3

**Last updated**: 2026-04-18

---

## Overview

Research Question 3 asks: *How do studies account for user roles or expertise when examining transparency–trust relationships?*

Expertise is the most consistently identified moderator of the transparency–trust relationship in this corpus. However, it is operationalized inconsistently, treated as a between-subjects variable in some studies and ignored entirely in others. This page documents what is known and what remains understudied.

---

## How Expertise Is Operationalized

Expertise is measured in heterogeneous ways across the corpus:

| Operationalization | Examples |
|---|---|
| Professional role (binary) | Clinician vs. patient; therapist vs. layperson; radiologist vs. oncologist |
| Years of experience (continuous) | Perlmutter (2–31 years pipeline experience); Yu et al. (clinician seniority) |
| Seniority strata | Calisto (intern / junior / middle / senior clinician) |
| Domain knowledge test | Post-task quiz (Wang & Ding); comprehension check |
| Self-reported AI familiarity | Rezaeian et al.; many others |
| AI anxiety scale | Bernardo & Seva; Lee et al. (LIMEADE) |
| Need for Cognition (NFC) | Cau & Spano; Conati et al. |
| Task-related capacity | Wang & Ding (post-task quiz of domain knowledge) |
| AI literacy (categorical) | Novice vs. expert distinction; Leichtmann intervention |

---

## Core Finding: Expertise Changes What Works

The overarching conclusion from studies that test expertise as a moderator is that **the same transparency intervention can be effective for one expertise level and ineffective or harmful for another**.

### Expertise Changes Optimal Explanation Format

- **Clinical seniority reverses communication preferences**: In breast cancer diagnosis, assertive (directive) AI communication reduces diagnostic errors by 39.2% for junior clinicians; suggestive (non-directive) communication is preferred by senior clinicians who integrate AI suggestions into their own clinical reasoning (domain: healthcare; Calisto et al., 2025).
- **Analogies help laypeople, not experts**: Analogy-based XAI explanations improve decision accuracy for non-experts in skin cancer detection; for experts, concept-level explanations without analogies are more effective (domain: general/lab; He et al., 2024).
- **Visual format alignment with clinical workflow**: Clinicians in ICU settings prefer explanation visualizations that match their temporal reasoning patterns; format effectiveness is mediated by cognitive fit with professional practice, not generic usability (domain: healthcare; Xian et al., 2026).
- **Lay users prefer explanations they cannot interpret**: Community health workers (CHWs) in rural India want SHAP/LIME explanations despite being unable to interpret the color coding correctly; desired understanding decouples from actual comprehension (domain: healthcare/Global South; Okolo et al., 2024).
- **Expert vs. novice response to two-class examples**: Technical experts benefit from two-class example XAI (showing both similar-positive and similar-negative cases) for trust and understanding; the distinction between case types requires domain knowledge to evaluate (domain: industrial; Perlmutter et al., 2024).

### Expertise Changes Reliance Patterns

- **Experts resist wrong AI recommendations better**: Therapists in clinical decision-making override incorrect AI recommendations more frequently than laypersons under both feature-based and counterfactual explanation conditions (domain: healthcare; Lee & Chew, 2023).
- **Domain expertise moderates advice reliance across domains**: Participants rely significantly more on AI advice in medical domains than sports domains (+18 percentage points), suggesting expertise confers both trust and capacity to evaluate AI quality (domain: general/lab; Kornowicz & Thommes, 2025).
- **Experienced clinicians trust AI more but are more vulnerable to trust erosion**: Experience (β = 0.28) predicts higher AI trust, but experienced users show stronger trust decay when AI makes errors (domain: healthcare; Yu et al., 2025).
- **Technical expertise predicts asymmetric risk preferences**: Oil-and-gas pipeline analysts deliberately classify ambiguous cases as anomalies due to the cost asymmetry of false negatives — a pattern not captured by generic trust scales and only observable with domain-expert samples (domain: industrial; Perlmutter et al., 2024).

### Expertise Determines Vulnerability to Misleading XAI

- **Novices are more deceived by imperfect explanations**: Experts can detect when an explanation is incorrect or implausible; novices take it at face value, showing higher Deception of Reliance (DoR) scores (domain: general/lab; Spitzer et al., 2025).
- **Low task-capacity users show explanation placebo effects**: Even irrational (randomly permuted) SHAP explanations improve decision accuracy for low-capacity users, suggesting heuristic processing that does not require explanation validity (domain: e-commerce; Wang & Ding, 2024).
- **AI literacy training alone is insufficient**: A short AI literacy educational intervention has no significant effect on appropriate reliance in high-risk decisions without accompanying XAI (domain: general/lab; Leichtmann et al., 2023).

---

## Studies That Account for Expertise Well

The following studies make expertise a central moderator and test its effects empirically:

| Source | Domain | Expertise operationalization | Key moderating finding |
|---|---|---|---|
| Calisto et al. (2025) | Healthcare | 4-seniority strata | Format preference and error rate reversal by seniority |
| He et al. (2024) | General/lab | Laypeople vs. experts | Analogies improve lay users; not experts |
| Lee & Chew (2023) | Healthcare | Therapist vs. layperson | Therapists override wrong AI more; counterfactuals benefit experts more |
| Conati et al. (2021) | Education | Perceptual speed, WM, NFC, personality | Multiple individual differences moderate explanation benefit |
| Perlmutter et al. (2024) | Industrial | 2–31 years domain experience | Expertise changes XAI format preference and reliance asymmetry |
| Spitzer et al. (2025) | General/lab | Novice vs. expert | Experts detect incorrect XAI; novices are deceived |
| Wang & Ding (2024) | E-commerce | Task-related capacity (post-task quiz) | Low-capacity users: placebo effect; high-capacity: need valid XAI |
| Okolo et al. (2024) | Healthcare/Global South | CHW novice users | Preference for XAI decouples from comprehension |
| Rezaeian et al. (2025) | Healthcare | Years of experience, specialty | Demographics predict self-report not behavioural trust |
| Yu et al. (2025) | Healthcare | Clinician experience (β = 0.28) | Experience increases trust but amplifies erosion |

---

## Studies That Under-specify Expertise

A substantial proportion of the corpus treats samples as homogeneous with respect to expertise, typically using MTurk or Prolific crowdsourced general-population samples. This limits generalizability to real-world expert contexts where the stakes are highest.

**Studies using general/student samples without expertise moderation**: Chu et al.; Cau et al.; Conijn et al.; Du et al.; Fleiß et al. (quota-representative but no expertise analysis); Kleizen et al.; Liu (2021); Nelekar et al. (student sample); Shulner et al.; Knapic et al. (2021) — STEM-background lay users tested in a medical imaging domain; authors explicitly flag the absence of domain experts as the primary limitation and call for application-grounded evaluation with physicians.

This represents a systematic gap: the majority of XAI trust research is conducted with non-experts, while the most consequential AI deployments involve domain experts (clinicians, analysts, operators).

---

## Cultural and Institutional Expertise Effects

Beyond domain expertise, cultural context shapes baseline trust propensity and the interpretation of transparency:

- **Indian students show higher propensity to trust** AI conversational agents (M > 4.5/5) than Western comparison groups, suggesting that cultural-institutional factors modulate transparency effects independently of domain expertise (domain: education/mental health; Nelekar et al., 2021).
- **Prior institutional trust dominates transparency effects** in government contexts, suggesting that civic expertise (familiarity with government processes) moderates citizen responses to ethical AI messaging (domain: government; Kleizen et al., 2023).
- **Chinese workplace contexts** show strong algorithm aversion driven by opacity, with anthropomorphism as an additional mitigating factor — suggesting cultural norms around human judgment may shape baseline algorithm aversion (domain: HR/China; Zhao et al., 2024).

---

## The Personalization Challenge

A recurrent recommendation across multiple papers is that transparency should be personalized to the user. Frameworks proposing this:

- **C-XAI** (Naiseh et al. 2024): A participatory design framework explicitly requiring user expertise assessment as an input to XAI interface design.
- **XIMED** (Karagoz et al. 2025): Dual-loop evaluation requiring human-centered assessment by specific expert user types.
- **Conati et al. (2021)**: Demonstrates that multiple individual difference dimensions (perceptual speed, working memory, NFC, personality) predict who benefits from explanations and how.

However, personalizing explanations at scale remains technically challenging. Calisto et al. demonstrate personalization by expertise stratum for a defined clinical task; generalizing this to arbitrary expertise dimensions is an open research problem.

---

## Gaps and Contradictions

1. **Expert user samples are underrepresented**: ~70% of studies use general/lay user samples. Expert findings may not generalise to novices, and vice versa.
2. **Expertise is often treated as categorical**: Most studies use binary expert/novice distinctions; continuous operationalizations (years of experience, domain knowledge test scores) are more informative but rarer.
3. **AI literacy as a separate dimension**: AI familiarity or literacy is rarely measured alongside domain expertise, making it impossible to disentangle their separate contributions.
4. **Cultural expertise is understudied**: Only Nelekar et al. directly examine cultural moderators; many other studies use convenience samples without reporting cultural context.
5. **Contradiction on experience effects**: Calisto et al. find seniority changes what works (not just how much); Yu et al. find seniority increases baseline trust. These findings are compatible but the mechanisms differ — further work is needed to reconcile them.

---

## Related pages

- [[user-expertise]]
- [[domain-context]]
- [[perceived-risk]]
- [[trust-calibration]]
- [[appropriate-reliance]]
- [[explainability]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]

## References

Calisto, F. M., Nunes, N., & Nascimento, J. C. (2025). Personalized explanations for clinician-AI interaction in breast imaging. *International Journal of Human-Computer Studies* [details TBD].

He, G., Bhatt, U., & Weller, A. (2024). Opening the analogical portal to explainability: How analogies shape AI explanations for different expertise levels. *CHI Conference on Human Factors in Computing Systems* [details TBD].

Kleizen, B., Van Dooren, W., Verhoest, K., & Tan, J. (2023). Do citizens trust trustworthy artificial intelligence? Experimental evidence on the limits of ethical AI measures in government. *Government Information Quarterly* [details TBD].

Kornowicz, J., & Thommes, K. (2025). Algorithm, expert, or both? Determinants of algorithm adoption in managerial decision-making. *Journal of Behavioral Decision Making* [details TBD].

Lee, J., & Chew, E. (2023). Understanding the effect of counterfactual explanations on trust and reliance on AI for human-AI collaborative clinical decision making. *Proceedings of the ACM on Human-Computer Interaction* (CSCW2), 7.

Leichtmann, B., Humer, C., Hinterreiter, A., Streit, M., & Mara, M. (2023). Effects of explainable artificial intelligence on trust and human behavior in a high-risk decision task. *Computers in Human Behavior* [details TBD].

Nelekar, P., Kulkarni, A., & Krishnaswamy, N. (2021). Effectiveness of embodied conversational agents for managing academic stress. *ACM International Conference on Intelligent Virtual Agents* [details TBD].

Okolo, C. T., Agarwal, Y., Dell, N., & Vashistha, A. (2024). "If it is easy to understand then it will have value": Examining perceptions of explainable AI with community health workers in rural India. *Proceedings of the ACM on Human-Computer Interaction* (CSCW), 8.

Perlmutter, S., Gifford, T., & Krening, S. (2024). Impact of example-based XAI for neural networks on trust, understanding, and performance. *International Journal of Human-Computer Studies* [details TBD].

Spitzer, M., Schlegel, U., & Keim, D. A. (2025). Imperfections of XAI: Phenomena influencing AI-assisted decision-making. *ACM Transactions on Interactive Intelligent Systems* [details TBD].

Wang, D., & Ding, Y. (2024). The rationality of explanation or human capacity? A study of human-AI collaboration in clinical decision support. *Journal of the American Medical Informatics Association* [details TBD].

Xian, Y., Mehandjiev, N., Constantinides, M., Chen, Y., Quboa, Q., & Kitchen, G. (2026). Clinician preferences for explainable AI in critical care. *International Journal of Medical Informatics*, 210 [details TBD].

Yu, K., Guo, J., Shen, Y., & Martens, H. (2025). Research and analysis of trust and control in human–AI collaboration in healthcare. *Frontiers in Psychology* [details TBD].

Zhao, Y., Xu, L., Yu, F., & Jin, W. (2024). Perceived opacity leads to algorithm aversion in the workplace. *Acta Psychologica Sinica*, 56(4), 497–514.
