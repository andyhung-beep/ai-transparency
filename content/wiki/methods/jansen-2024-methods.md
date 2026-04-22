# Jansen et al. 2024 — Methods

**Summary**: Two online studies (Experiment A: N=76 US Prolific participants; Experiment B: N=22 university-recruited German participants) using the novel EDULICIT method to simultaneously educate the public about AV capabilities and evaluate how uncertainty visualization of Situation Detection and Situation Prediction affects user trust, situation awareness, and capability assessments.

**Sources**: Jansen et al._Visualizing imperfect situation detection and prediction.pdf

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-19

---

## Study design
experimental (two studies: Experiment A — between-subjects replication with pre-defined video; Experiment B — within-subjects user-uploaded scenario study)

## Sample
- N: Experiment A: N=76; Experiment B: N=22 (total N=98 across both studies)
- Population: Experiment A — general public (US-based adults, Prolific); Experiment B — general public skewing younger and more educated (50% college students, university-recruited, Germany)
- Domain: automated vehicles / transportation
- Country / region: Experiment A — United States; Experiment B — Germany
- Recruitment method: Experiment A — Prolific; Experiment B — university flyers

## Transparency operationalization
- Type: uncertainty visualization / process transparency — visual overlay of AV's Situation Detection (semantic segmentation coloring detected objects) and Situation Prediction (pedestrian crossing intention icons) on driving video; low-abstraction representation of raw neural network outputs including false positives, misclassifications, and uncertain predictions
- Manipulation or measure: Experiment A — between-subjects: baseline (no visualization) vs. combined visualization of Situation Detection, Situation Prediction, and Trajectory Planning; replication of Colley et al. (2022); Experiment B — within-subjects: participants uploaded their own challenging AV scenarios, website automatically applied neural-network-based Situation Detection (Detectron2 R101-FPN panoptic segmentation) and Situation Prediction (Mordan et al., 2021)
- Scale / instrument name: not applicable (visual overlay displays, not a scale)
- Number of items: not applicable

## Trust operationalization
- Type: cognitive trust / calibrated trust — trust in automation and predictability/understandability; also perceived safety, situational trust, and perceived AV capability
- Measure: Körber (2019) Trust in Automation questionnaire (Trust in Automation and Predictability/Understandability subscales, 5-point Likert); Faas et al. (2020) perceived safety semantic differentials; Situational Trust Scale for Automated Driving — Holthausen et al. (2020) subscales (Performance, Judgment, Reaction); perceived AV capability ratings
- Scale / instrument name: Trust in Automation questionnaire (Körber, 2019); Faas et al. (2020) perceived safety scale; Situational Trust Scale for Automated Driving (Holthausen et al., 2020)
- Number of items: not reported
- Behavioural vs self-report: self-report (all measures are Likert / semantic differential ratings)

## Moderators and covariates tested
- Visualization condition (visualization vs. baseline): primary between-subjects factor in Experiment A
- Scenario type (user-chosen challenging scenarios): primary within-subjects factor in Experiment B; scenarios primarily involved large intersections and multiple vulnerable road users
- Requested information type (perception-related vs. prediction-related): measured in Experiment A; participants without visualization requested significantly more perception- and prediction-related information
- User expertise / AI literacy: not measured or manipulated; both samples are general-public lay users; Experiment B skewed younger and more educated but expertise not formally varied — relevant to RQ3 in that all findings apply to non-expert users

## Statistical approach
- Primary analysis method: Experiment A — Wilcoxon signed-rank test and Mann-Whitney U test (non-parametric; specific tests not fully specified in source page); Experiment B — paired t-test (t(21)=−3.65 for situation awareness); visual clutter tested with Wilcoxon (V=132.50); information requests tested with Wilcoxon (V=825.00)
- Software: not reported
- Key model fit or effect size reported: Experiment A — cognitive load V=825.00, p=0.004, r=−0.39 (significant); visual clutter V=132.50, p<0.001, r=−0.85 (significant); trust, perceived safety, and AV capability not significant; Experiment B — situation awareness t(21)=−3.65, p=0.001, r=−0.75 (significant); trust and perceived safety not significant

## Author-noted limitations
- Non-significant trust effects in both experiments despite significant increases in situation awareness (Experiment B) and information provision; suggests transparency–trust relationship may require additional conditions (error-free visualization, longer exposure) to manifest
- Experiment B sample was small (N=22), skewed younger and more educated, and recruited from a university — limiting generalisability
- User-uploaded videos (Experiment B) varied in quality and scenario type, introducing heterogeneity
- Public misconceptions about AV capabilities suggest the EDULICIT education component may need enhancement before trust calibration effects emerge
- Replication design (Experiment A) uses a pre-defined video, limiting ecological validity
- No expert-user comparison; findings apply exclusively to lay users

## Related pages
- [[jansen-visualizing-imperfect-av]]
- [[uncertainty-visualization]]
- [[trust-calibration]]
- [[process-transparency]]
- [[appropriate-reliance]]
- [[user-expertise]]

## References
Jansen, M., et al. (2024). Visualizing imperfect situation detection and prediction in automated vehicles: Understanding users' perceptions via user-chosen scenarios. (Journal not specified in source page.)
