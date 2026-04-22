# Naiseh et al. 2024 — Methods

**Summary**: A framework development and evaluation study presenting C-XAI, a four-phase participatory design framework for creating XAI interfaces that support trust calibration, evaluated through structured expert review (N = 6) and a multi-stakeholder healthcare case study (N = 14).

**Sources**: Naiseh et al._C-XAI a conceptual framework for designing XAI tools.pdf

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-19

---

## Study design
mixed-methods (framework development with expert review and qualitative case study evaluation)

## Sample
- N: 6 (Phase 1 expert evaluation) + 14 (Phase 2 healthcare case study) = 20 total evaluators
- Population: Phase 1 — AI, HCI, requirements engineering, and psychology domain experts (5–12 years experience); Phase 2 — medical doctors, pharmacists, ML engineers, HCI researchers, psychologists, and requirements engineers
- Domain: healthcare (prescription screening) as primary case study; framework intended for criminal justice and any high-stakes decision domain
- Country / region: United Kingdom, Germany, United States, Italy (Phase 2 case study participants drawn internationally)
- Recruitment method: purposive sampling of domain and disciplinary experts; recruitment method not further reported

## Transparency operationalization
- Type: explainability — technical properties of XAI methods assessed across five dimensions (Functional, Operational, Usability, Safety, Validation) using the Explainability Facts Sheets (EFS) framework
- Manipulation or measure: not applicable as an experimental manipulation; C-XAI framework specifies an assessment procedure for evaluating XAI method properties (accuracy, completeness, soundness, novelty, interactivity) and mapping them to trust calibration risk profiles; four design principles proposed: Persuasive Design, Challenging Habitual Actions, Attention Guidance, Training and Learning
- Scale / instrument name: Explainability Facts Sheets (EFS) framework (existing instrument integrated into C-XAI); framework itself is the primary methodological contribution
- Number of items: not applicable

## Trust operationalization
- Type: behavioural (trust calibration — agreement and compliance as behavioural indicators)
- Measure: the framework proposes four behavioural metrics for measuring trust calibration: (1) agreement percentage — how often users agree with AI recommendations; (2) compliance percentage — how often users comply after initially disagreeing; (3) incorrect decisions — human-AI collaboration outcomes that are wrong; (4) correct decisions; framework distinguishes over-trust (uncritical compliance) and under-trust (rejection of valid recommendations) as the two failure modes
- Scale / instrument name: not applicable (proposed behavioural metrics, not a validated scale)
- Number of items: not applicable
- Behavioural vs self-report: behavioural (proposed metrics); Phase 1 and Phase 2 evaluations use qualitative expert feedback, not trust measurement instruments

## Moderators and covariates tested
- User expertise / domain knowledge: explicitly incorporated into C-XAI's identification phase; framework recommends recruiting diverse stakeholders including representative users, domain experts, and psychologists; AI literacy, domain knowledge, and curiosity level are cited as factors enriching XAI requirements — directly relevant to RQ3
- Stakeholder role: medical professionals, ML engineers, and behavioral scientists brought different XAI needs and risk perceptions in the healthcare case study — relevant to RQ3
- XAI technical properties (novelty, complexity, interactivity): identified as sources of trust calibration risk (e.g., high novelty may cause habituation and over-trust; static explanations may cause under-engagement)

## Statistical approach
- Primary analysis method: qualitative thematic analysis of structured expert feedback (Phase 1); qualitative analysis of case study stakeholder outputs (Phase 2); no quantitative statistical analysis
- Software: not reported
- Key model fit or effect size reported: not applicable (qualitative framework evaluation); 5 of 6 Phase 1 experts rated C-XAI positively on completeness

## Author-noted limitations
- The framework cannot eliminate all trust calibration risks; it provides systematic anticipation and mitigation tools, not guarantees
- Framework has only been evaluated in one empirical domain (healthcare prescription screening); generalisability to other high-stakes domains (criminal justice, finance) is claimed but not empirically tested in this paper
- Expert and stakeholder evaluations are qualitative; no controlled trial of C-XAI against a baseline design process was conducted
- The proposed behavioral trust calibration metrics require longitudinal deployment data that are not collected in the current study
- Mapping of XAI technical properties to trust calibration risks is based on prior literature and expert judgment, not empirical data generated here

## Related pages
- [[naiseh-c-xai-framework]]
- [[trust-calibration]]
- [[appropriate-reliance]]
- [[explainability]]
- [[causability]]
- [[traceability]]
- [[user-expertise]]
- [[domain-context]]
- [[cognitive-trust]]
- [[behavioural-trust]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]
- [[rq3-user-roles]]
