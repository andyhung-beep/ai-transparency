# Algorithmic and HCI Aspects for Explaining Recommendations of Artistic Images

**Source file**: [Original article](../../raw/Dominguez et al._Algorithmic and HCI aspects for explaining recommendations.pdf)

**Summary**: Two crowdsourced user studies (AMT, total N ≈ 300) examining how explanation style, recommendation algorithm, device type, and explanation optionality affect user experience with a visual art recommender system, finding that explanations improve satisfaction primarily through enhanced understandability and trust.

**Sources**: Dominguez et al._Algorithmic and HCI aspects for explaining recommendations.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Dominguez, Donoso-Guzmán, Messina, and Parra (2020), published in *ACM Transactions on Interactive Intelligent Systems*, report two Amazon Mechanical Turk user studies on an online art image recommender system built from the UGallery e-commerce dataset (1,371 users, 3,490 items, 2,846 transactions).

**Study 1** (N = 121 valid participants) used a 3 × 2 mixed design: three interface conditions (no explanation; black-box explanation via top-3 similar images; transparent explanation via visual feature bar chart) crossed with two recommendation algorithms (DNN—accurate but opaque; AVF—less accurate but humanly interpretable visual features). Outcome variables included understandability, relevance, diversity, satisfaction, trust, and perceived explainability.

**Study 2** (N = 177 valid participants) used a 2 × 2 between-subjects design: device (mobile vs. desktop) × explanation obligatoriness (mandatory vs. optional), with a single DNN-based algorithm and similar-item explanations. A structural equation modelling (SEM) approach based on Knijnenburg et al.'s recommender evaluation framework was used in both studies to build comprehensive user experience models.

## Key Findings

- Recommendation interfaces with explanations increased user satisfaction compared to no-explanation interfaces, mediated by improved understandability and trust. (source: Dominguez et al._Algorithmic and HCI aspects for explaining recommendations.txt; domain: e-commerce / art recommendation)
- Trust had an effect on satisfaction approximately 3× larger than understandability in Study 1, and 10× larger in Study 2—highlighting trust as the dominant driver of overall satisfaction with a recommender system. (source: Dominguez et al._Algorithmic and HCI aspects for explaining recommendations.txt; domain: e-commerce / art recommendation)
- Neither the interface type nor the algorithm had a direct effect on trust; both effects were fully mediated by perceived understandability—suggesting users only trust what they understand. (source: Dominguez et al._Algorithmic and HCI aspects for explaining recommendations.txt; domain: e-commerce / art recommendation)
- Higher transparency (feature-level bar chart) was not always perceived as superior to simpler black-box similarity explanations; more transparency is not always better. (source: Dominguez et al._Algorithmic and HCI aspects for explaining recommendations.txt; domain: e-commerce / art recommendation)
- Algorithm accuracy (DNN > AVF) positively affected understandability and satisfaction independently of explanation style, confirming that interface-level explanation cannot compensate for a weak algorithm. (source: Dominguez et al._Algorithmic and HCI aspects for explaining recommendations.txt; domain: e-commerce / art recommendation)
- Explanation obligatoriness (mandatory vs. optional) had no significant effect on user experience in Study 2—user control over seeing explanations did not improve outcomes. (source: Dominguez et al._Algorithmic and HCI aspects for explaining recommendations.txt; domain: e-commerce / art recommendation)
- Device type (mobile vs. desktop) affected preference elicitation time but showed only indirect effects on satisfaction; mobile users spent less time comparing items, leading to different rating patterns. (source: Dominguez et al._Algorithmic and HCI aspects for explaining recommendations.txt; domain: e-commerce / art recommendation)
- User cognitive load (effort/haste) negatively moderated both understandability and trust; higher mental effort during the task reduced perceived understanding and trust. (source: Dominguez et al._Algorithmic and HCI aspects for explaining recommendations.txt; domain: e-commerce / art recommendation)
- Domain expertise (art experience) was a significant personal characteristic in Study 2's SEM, linking to the moderating role of user knowledge on recommender system experience. (source: Dominguez et al._Algorithmic and HCI aspects for explaining recommendations.txt; domain: e-commerce / art recommendation)
- Trust effects on satisfaction replicated across both studies and are consistent with findings in prior recommender systems literature (Cramer et al., 2008; Holliday et al.), supporting generalisability within the recommender systems domain. (source: Dominguez et al._Algorithmic and HCI aspects for explaining recommendations.txt; domain: e-commerce / art recommendation)

## Transparency Constructs

The study examines two forms of explanation within the [[example-based-explanations]] category: (1) black-box similarity explanations showing top-3 visually similar items from the user's past preferences, and (2) white-box feature-based explanations showing a bar chart of visual attractiveness features (brightness, saturation, sharpness, colorfulness). The distinction maps onto opaque vs. transparent algorithmic reasoning, addressing both [[algorithmic-transparency]] and [[explainability]]. The finding that more transparency does not automatically improve trust or satisfaction challenges a naive transparency-is-always-better assumption and connects to the [[process-transparency]] literature on appropriate levels of disclosure.

## Trust Constructs

Trust is measured as a single self-report item ("I trusted the recommendations made") on a 0–100 scale, aligned with the ResQue recommender evaluation framework. This is a [[cognitive-trust]] operationalisation focused on perceived system competence and reliability. The SEM results establish trust as the dominant mediator between explanations and user satisfaction, providing structural evidence for [[behavioural-trust]] (willingness to use / recommend the system again). The study does not measure [[affective-trust]] separately.

## Relevance to Research Questions

**RQ1**: The study operationalises explainability as a user perception ("explanations made sense to me") and trust as a subjective rating, situating them within the recommender systems evaluation tradition. The SEM framework integrates personal characteristics (domain expertise), subjective system aspects (understandability, trust), and outcomes (satisfaction), contributing to [[rq1-conceptualizations]].

**RQ2**: The SEM models demonstrate a mediated, non-direct pathway from explanations to trust (via understandability), and a dominant path from trust to satisfaction. This conditional, mediated structure—with algorithm accuracy as a boundary condition—contributes nuanced evidence on transparency–trust relationships to [[rq2-relationships]].

**RQ3**: Domain expertise (art knowledge) was captured and included as a personal characteristic in Study 2, with experienced art users reporting higher satisfaction. This is one of the few recommender system studies to systematically include user expertise as a covariate, contributing to [[rq3-user-roles]].

## Related pages

- [[explainability]]
- [[example-based-explanations]]
- [[algorithmic-transparency]]
- [[cognitive-trust]]
- [[behavioural-trust]]
- [[user-expertise]]
