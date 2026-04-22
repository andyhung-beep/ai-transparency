# Lundberg et al. 2022 — Methods

**Summary**: A quantitative expert survey (N = 30 domain experts) comparing the effect of a SHAP-based visual explanation (VisExp) versus a rule-based textual explanation on trust in a deep neural network in-vehicle intrusion detection system (IV-IDS) for automotive CAN bus traffic.

**Sources**: Lundberg et al._Experimental_Analysis_of_Trustworthy_In-Vehicle_Intrusion_Detection_System_Using_eXplainable_Artificial_Intelligence_XAI.pdf

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-19

---

## Study design
experimental (between-subjects comparison with expert survey)

## Sample
- N: 30
- Population: domain experts — AI specialists, cybersecurity professionals, wireless/IoT researchers, automotive engineers, data analysts; recruited from Mid Sweden University and RISE Research Institutes of Sweden
- Domain: automotive cybersecurity (in-vehicle intrusion detection)
- Country / region: Sweden
- Recruitment method: convenience sampling from Mid Sweden University and RISE Research Institutes of Sweden

## Transparency operationalization
- Type: explainability — post-hoc visual and rule-based feature importance explanations
- Manipulation or measure: three conditions compared within a structured survey: (1) raw model input/output only (no explanation); (2) rule-based textual explanation; (3) VisExp — a pseudo-global SHAP-based visualisation using KernelSHAP, displayed as dual swarm plots with violin overlays showing feature-level SHAP values for normal vs. attack traffic; all conditions used the same underlying DNN IV-IDS trained on the "Survival" CAN bus dataset (1,735,840 instances)
- Scale / instrument name: not applicable (structured comparison design with Likert-scale survey items)
- Number of items: not applicable

## Trust operationalization
- Type: cognitive and behavioural
- Measure: structured questionnaire with Likert-scale items asking participants to rate trustworthiness and understandability of each explanation type; key items include Q6 (understanding) and Q7 (trustworthiness of the IV-IDS when shown each explanation); responses on a 0–4 scale (0 = Strongly Disagree, 4 = Strongly Agree); overall in-vehicle trust and general AI trust also assessed
- Scale / instrument name: custom Likert-scale questionnaire developed by authors
- Number of items: not reported (multiple items; specific count not stated in available sources)
- Behavioural vs self-report: self-report (Likert-scale ratings); no behavioural trust outcome collected

## Moderators and covariates tested
- User expertise / domain specialisation: measured and used to stratify results; participants grouped into "primary experts" (AI, cybersecurity, automotive) vs. "secondary experts" (wireless/IoT, data analysis, AI novices); primary experts showed stronger preference for VisExp over rule-based explanation, while secondary experts and novices showed smaller differences — directly relevant to RQ3
- Explanation type (VisExp vs. rule-based vs. no explanation): primary manipulation; not a moderator per se but the key independent variable

## Statistical approach
- Primary analysis method: paired-samples t-tests comparing trust means across explanation conditions for each expert group
- Software: not reported
- Key model fit or effect size reported: mean trust difference (VisExp vs. raw output) = 0.786, t(26) = 6.904, p < 0.001; mean trust difference (rule-based vs. raw output) = 0.357, p = 0.019; mean trust difference (VisExp vs. rule-based) = 0.429, t(26) = 3.122, p = 0.0081; 72.4% of all participants preferred VisExp; DNN IV-IDS F1-score = 0.9868, accuracy = 0.9973 (10-fold cross-validation)

## Author-noted limitations
- Small sample size (N = 30) limits statistical power and generalisability
- Expert sample from a single university and research institute; may not represent the full range of automotive or cybersecurity practitioners
- Trust items are self-reported; behavioural reliance on the system (actual use of IDS alerts) was not tested
- Study relies on static visualisation artefacts rather than a live deployed system
- AI novices and secondary experts were not further stratified; finer-grained expertise analysis was not possible
- The DNN was trained on a single benchmark dataset (Survival CAN bus), limiting cross-dataset generalisability

## Related pages
- [[lundberg-xai-invehicle-intrusion-detection]]
- [[explainability]]
- [[algorithmic-transparency]]
- [[cognitive-trust]]
- [[user-expertise]]
- [[appropriate-reliance]]
- [[rq2-relationships]]
- [[rq3-user-roles]]
