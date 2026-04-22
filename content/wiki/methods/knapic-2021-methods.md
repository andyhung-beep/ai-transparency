# Knapic 2021 — Methods

**Summary**: Three between-subjects user studies (N = 60 total; 20 per group) comparing LIME, SHAP, and CIU visual explanations for a CNN-based gastric bleeding detection system on decision accuracy, satisfaction, understanding, and error detection.

**Sources**: Knapic et al._Explainable_Artificial_Intelli.pdf

**Research questions addressed**: RQ1 / RQ2 / RQ3

**Last updated**: 2026-04-19

---

## Study design
experimental (between-subjects; three-group comparison)

## Sample
- N: 60 (20 per group: LIME, SHAP, CIU)
- Population: university students and staff with STEM backgrounds; no medical expertise; approximately 50% had prior XAI knowledge; predominantly male; ages in 20s–30s
- Domain: healthcare / medical imaging (video capsule endoscopy; gastric bleeding detection)
- Country / region: not reported
- Recruitment method: convenience (university students and staff)

## Transparency operationalization
- Type: post-hoc, model-agnostic local explanation (visual attribution/saliency overlays)
- Manipulation or measure: between-subjects manipulation — each group received one of three explanation types for a CNN achieving 98.58% validation accuracy on gastric bleeding detection: (1) LIME (local surrogate linear model, superpixel-level), (2) SHAP / Kernel SHAP (Shapley values, bidirectional two-color visualization), (3) CIU (Contextual Importance and Utility — non-surrogate, contextual feature attribution); each participant also completed a no-explanation baseline phase for within-group comparison
- Scale / instrument name: not applicable
- Number of items: not applicable

## Trust operationalization
- Type: cognitive (satisfaction and understanding as proxies); behavioural (decision accuracy, error detection)
- Measure: decision accuracy (correct classifications of bleeding vs. non-bleeding endoscopy images); explanation satisfaction (Likert 0–5 scale); self-reported understanding; time on task; error detection (ability to identify incorrect explanations); trust is not measured as a standalone validated construct
- Scale / instrument name: not reported (custom satisfaction and understanding items)
- Number of items: not reported
- Behavioural vs self-report: both (behavioural accuracy and error detection; self-report satisfaction and understanding)

## Moderators and covariates tested
- Prior XAI knowledge: approximately 50% of sample had prior XAI knowledge; measured but moderation not formally tested
- LIME satisfaction vs. accuracy correlation: lower LIME satisfaction correlated with better decision accuracy (p = 0.019), suggesting critical engagement moderates reliance
- No formal moderator analysis reported for user expertise or role (relevant to RQ3 as a gap — lay non-medical users only)

## Statistical approach
- Primary analysis method: Wilcoxon signed-rank test (within-group, explanation vs. no-explanation comparisons for accuracy); Mann-Whitney U test (between-group comparisons for accuracy, satisfaction, error detection, time)
- Software: not reported
- Key model fit or effect size reported: LIME vs. no-explanation p = 0.738; SHAP vs. no-explanation p = 0.464; CIU vs. no-explanation p = 0.158; CIU satisfaction vs. LIME p < 0.001; CIU error detection vs. LIME p = 0.009, vs. SHAP p = 0.037; SHAP vs. LIME time p = 0.011; SHAP vs. CIU time p = 0.016

## Author-noted limitations
- Lay (non-medical) users only — the authors explicitly acknowledge this as the main limitation; findings may not generalize to physician users
- Small samples (N = 20 per group) — insufficient power for comparisons that approach but do not reach significance (e.g., CIU vs. LIME accuracy p = 0.120)
- Single medical dataset (Red Lesion Endoscopy); generalizability across imaging modalities untested
- CIU still in early development at time of publication (2021); less mature tooling than LIME/SHAP

## Related pages
- [[knapic-xai-medical-decision-support]]
- [[explainability]]
- [[appropriate-reliance]]
- [[user-expertise]]
- [[domain-context]]
