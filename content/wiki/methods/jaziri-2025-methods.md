# Jaziri & Sassi 2025 — Methods

**Summary**: A hybrid technical study combining a computational evaluation across 20,000 simulated episodes in autonomous vehicle (CARLA) and healthcare (sepsis treatment) domains with a controlled lab human-AI interaction study (N=120; 60 clinicians, 60 engineers), evaluating a Deep Reinforcement Learning framework with embedded symbolic reasoning, multi-head self-attention, and Layer-wise Relevance Propagation on task performance, user trust, comprehension, cognitive load, and response time.

**Sources**: Jaziri & Sassi_Explainable by design.pdf

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-19

---

## Study design
mixed-methods (technical paper with computational evaluation + controlled laboratory user study)

## Sample
- N: 120 (60 clinicians, 60 engineers); computational evaluation used 20,000 simulated episodes (12,000 AV scenarios + 8,000 sepsis patient cases)
- Population: domain professionals (clinicians) and technical experts (engineers)
- Domain: autonomous vehicles (CARLA simulator) and healthcare (sepsis treatment planning; synthetic MIMIC-IV/eICU-based data)
- Country / region: not reported
- Recruitment method: not reported (controlled lab study)

## Transparency operationalization
- Type: intrinsic / embedded explainability ("explainability-by-construction") — three complementary explanation mechanisms integrated into the model architecture during training rather than applied post-hoc:
  (1) Symbolic reasoning — decision trees (CART, max depth 12) mapping state-action pairs to logical rules; corresponds to algorithmic transparency;
  (2) Multi-head self-attention (12 heads) — attention weights highlighting which state features drove each decision; corresponds to process transparency;
  (3) Layer-wise Relevance Propagation (LRP) — backward propagation of relevance scores attributing each neuron's contribution; corresponds to traceability
- Manipulation or measure: between-subjects comparison of hybrid explainable model (DDQN + symbolic reasoning + attention + LRP) vs. standard DDQN baseline; lab study participants interacted with 4K display interfaces with eye tracking (Tobii Pro) and haptic feedback; participant-rated trust, comprehension, cognitive load, and response time measured
- Scale / instrument name: seven-point Likert trust scale (researcher-constructed); NASA-TLX for cognitive load
- Number of items: trust — not reported (seven-point Likert); NASA-TLX — 6 subscales (standard instrument)

## Trust operationalization
- Type: cognitive trust — based on comprehension and confidence in the system's reasoning; pre/post trust ratings measured
- Measure: seven-point Likert trust scale (mean trust score); pre- and post-exposure measurement; strong correlation between comprehension and trust (R²=0.94) supports cognitive-trust interpretation
- Scale / instrument name: researcher-constructed seven-point Likert scale; not a validated published scale
- Number of items: not reported
- Behavioural vs self-report: self-report (Likert trust rating); response time as a behavioural efficiency measure

## Moderators and covariates tested
- User expertise group (clinicians vs. engineers): between-subjects; clinicians showed higher trust (+11 vs. +10 trust points) and comprehension (90% vs. 89%); engineers showed lower cognitive load (53 vs. 59 NASA-TLX) and faster response times (2.7 s vs. 3.1 s) — directly relevant to RQ3, demonstrating expertise-dependent differences in explainability benefits
- Explanation component (ablation): symbolic reasoning contributed ~45% of comprehension gains; attention heads contributed +35% comprehension and +0.5 trust points; LRP contributed +0.2 clarity points — component-level moderation of explanation effectiveness
- Sensor noise robustness: Gaussian perturbation up to 20%; hybrid model TCR declined only 1.3% vs. 2.3% for DDQN
- Explanation preference: decision trees (88% preference) and attention heatmaps (82%) preferred; LRP heatmaps found too complex (12% preference) — user-perceived usability moderated by explanation type

## Statistical approach
- Primary analysis method: between-groups comparison of task-completion rate (TCR), safety scores, critical error rate, mean inference latency, trust score, comprehension, response time, and NASA-TLX; Cohen's d for effect sizes; correlation analysis (R² for comprehension–trust relationship)
- Software: not reported
- Key model fit or effect size reported: trust Cohen's d=1.05 (p<0.001); comprehension Cohen's d=1.23 (p<0.001); response time Cohen's d=0.97 (p<0.001); cognitive load Cohen's d=0.90 (p<0.001); R²=0.94 (comprehension–trust correlation, N=120, p<0.001)

## Author-noted limitations
- ~4% task-completion-rate trade-off of hybrid model vs. standard DDQN (91.9% vs. 96.2% in AV domain)
- Evaluation conducted in simulated environments (CARLA simulator; synthetic healthcare data); real-world deployment conditions may differ
- LRP heatmaps found too complex by most participants, limiting practical utility of this component for non-technical users
- Human-AI interaction study involves only two expert groups (clinicians and engineers); general-public / non-expert users not evaluated
- Controlled lab setting with 4K displays and haptic feedback may not reflect typical deployment contexts
- Trust scale is researcher-constructed and not a validated standardized instrument, limiting comparability

## Related pages
- [[jaziri-explainable-by-design]]
- [[explainability]]
- [[causability]]
- [[traceability]]
- [[algorithmic-transparency]]
- [[process-transparency]]
- [[cognitive-trust]]
- [[user-expertise]]

## References
Jaziri, A., & Sassi, M. (2025). Explainable by design: Enhancing trustworthiness in AI-driven control systems. (Journal not specified in source page.)
