# Explainable AI for Government: Does the Type of Explanation Matter to the Accuracy, Fairness, and Trustworthiness of an Algorithmic Decision as Perceived by Those Who Are Affected?

**Source file**: [Original article](../../raw/Aoki et al._Explainable AI for government.pdf)

**Summary**: Aoki et al. conduct two pre-registered online survey experiments (total N = 1200) with corporate officers in Japan to test whether four XAI explanation types — input-based, group-based, case-based, and counterfactual — differentially affect affectees' perceived accuracy, fairness, and trustworthiness of adverse algorithmic administrative decisions, finding that providing any explanation generally helps but that the detailed effects of explanation type are not robust across the two decision contexts studied.

**Sources**: Aoki et al._Explainable AI for government.txt

**Research questions addressed**: RQ1, RQ2

**Last updated**: 2026-04-18

---

## Overview

This study addresses a gap in XAI research on public administration: whereas most XAI work focuses on developers or end-users in commercial contexts, this paper examines how members of the public who are adversely affected by government algorithmic decisions perceive those decisions depending on how they are explained. The study is grounded in equity theory, procedural justice theory (Thibaut and Walker; Leventhal), interactional justice (Bies and Moag), and psycho-ergonomics accounts of human trust in automation (Lee and See, 2004).

Two studies were conducted as pre-registered online survey experiments in December 2022 with N = 1200 participants (600 per study), all of whom were officers in senior positions at stock companies registered in Japan. In Study 1, subjects were presented with a scenario in which a government ministry rejected their company's grant application. In Study 2, subjects faced a scenario in which a tax authority selected their company for an on-site tax inspection. Both scenarios represented realistic adverse government decisions. Subjects were randomly assigned to receive one of four explanation types (input-based, group-based, case-based, or counterfactual) or no explanation at all, and then rated the perceived fairness, accuracy, and trustworthiness of the decision on separate scales. The domain is public administration / e-government in a Japanese context.

## Key Findings

- Providing some type of explanation had a generally positive effect on affectees' perceptions of the decision's fairness, accuracy, and trustworthiness compared to receiving no explanation at all; this finding held across both decision contexts (domain: public administration/government).
- The effects of specific explanation types were not consistent or robust across the two studies; no single explanation type uniformly outperformed the others across all three outcome variables in both scenarios (domain: public administration/government).
- Counterfactual explanations — which tell affectees what they would need to change to receive a favorable outcome — were theorized and found in some analyses to be distinctive in supporting perceived procedural fairness, because they fulfill Leventhal's "corrective" criterion for fair process by giving subjects a route to challenge or change the decision (domain: public administration/government).
- Input-based and group-based explanations were expected to function as more global explanations and thus contribute more to perceived accuracy than instance-specific case-based and counterfactual explanations, but empirical support for this hypothesis was inconsistent across the two studies (domain: public administration/government).
- The authors note that the inconsistency between the two studies calls for a nuanced, context-sensitive approach to explanation design rather than a one-size-fits-all recommendation, as decision context (grant rejection vs. tax audit) moderated which explanation type was most effective (domain: public administration/government).
- The paper identifies a gap between normative legal frameworks mandating the right to an explanation (e.g., EU GDPR) and empirical evidence about which explanation types best support the values those frameworks aim to protect (domain: public administration/legal).

## Transparency Constructs

The study examines four distinct explanation types as operationalizations of XAI transparency in public sector contexts:
- **Input-based explanations**: feature-contribution explanations identifying which input variables drove the decision and by how much (analogous to feature importance or SHAP outputs); global in principle.
- **Group-based explanations**: outcome distribution explanations reporting the proportion of similar entities in the training data that received the same decision; global in principle.
- **Case-based explanations**: instance-level explanations presenting a similar past case from the training data for comparison; local and instance-specific.
- **Counterfactual explanations**: contrastive explanations specifying the smallest change to inputs that would have produced a favorable outcome; local and action-oriented.

The paper maps these types onto local vs. global distinctions and links them to different components of procedural and distributive justice.

## Trust Constructs

Trustworthiness is treated as a perceived attribute of the decision (and by extension the public institution making it), measured as a self-reported rating by affectees. The paper draws on psycho-ergonomics frameworks (Lee and See, 2004) to connect understanding of decision processes to trust in automation, and invokes procedural justice theory to explain why explanations that give affectees a sense of process comprehension and corrective recourse should enhance perceived trustworthiness. Institutional trust is implicated in that the subjects are evaluating government decisions; the paper notes that positive recognition of individual decision quality may reinforce broader institutional trust in government.

## Relevance to Research Questions

**RQ1**: The paper contributes a theoretically grounded taxonomy of four government-relevant explanation types and links each type to procedural and distributive justice mechanisms. It operationalizes trustworthiness as perceived by the affected party (affectee perspective), which is underrepresented in most XAI research focusing on developers or direct users.

**RQ2**: The relationship between explanation type and trust/fairness perceptions is **conditional on context**: providing any explanation was better than none, but the advantage of specific explanation types did not replicate consistently across the grant-rejection and tax-audit scenarios. This non-robustness is a key empirical finding suggesting that the explanation-trust relationship is context-dependent rather than uniformly linear.

## Related pages

- [[counterfactual-explanations]]
- [[explainability]]
- [[process-transparency]]
- [[institutional-trust]]
- [[algorithmic-transparency]]
- [[domain-context]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]
