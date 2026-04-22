# Wiki Log

Append-only record of all wiki operations. Most recent entry at the top.

---

## 2026-04-19 — Second batch of methods pages: 11 papers (Alarcon through Cau)

**Operation**: Created methods pages for 11 papers (Alarcon et al. through Cau et al.) that had source pages but no corresponding methods pages. Appended 11 rows to `wiki/methods/index.md`. Updated `wiki/index.md` Methods Pages section with 11 new entries.

**Methods pages created**:
- `alarcon-2023-methods.md` ← Alarcon et al. — Calibrated vs. uncalibrated ML confidence displays (N=396, 3 experiments, MTurk)
- `angerschmid-2022-methods.md` ← Angerschmid et al. — Explanation type × fairness level on trust in health AI (N=25, 3×3 factorial)
- `aoki-2023-methods.md` ← Aoki et al. — Four XAI explanation types on governmental decision trust (N=1,200 Japanese corporate officers)
- `banovic-2022-methods.md` ← Banovic et al. — Deceptive competence disclosure enables untrustworthy AI to gain trust (N=120, chess, MTurk)
- `bernardo-2023-methods.md` ← Bernardo & Seva — XAITC model with affective processing route from XAI design to trust (N=202 pre-study, Philippines)
- `bhaskara-2021-methods.md` ← Bhaskara et al. — SAT model three transparency levels in UAV task (N=176 undergraduates)
- `bigras-2019-methods.md` ← Bigras et al. — Transparent low-effort recommendation agent maximizes decision quality (N=20 retail planners, lab)
- `brand-2023-methods.md` ← Brand et al. — E-BART joint NL explanation generation improves misinformation detection (MTurk + NLP benchmarks)
- `calisto-2025-methods.md` ← Calisto et al. — Assertive vs. non-assertive AI communication × clinician expertise in breast imaging (N=52, Portugal)
- `cau-spano-2026-methods.md` ← Cau & Spano — Four XAI styles in loan-approval task; NFC as moderator (N=288, Prolific, pre-registered)
- `cau-2023-methods.md` ← Cau et al. — Inductive/abductive/deductive explanation logic-styles on reliance in image and text tasks (N≈1,324, Prolific)

**Updated**:
- `wiki/methods/index.md` — Appended 11 new rows (Alarcon through Cau)
- `wiki/index.md` — Methods Pages section extended with 11 new entries

**Note on year uncertainty**: Years for Alarcon, Aoki, and Banovic could not be confirmed from PDF title pages (PDFs not accessible as text in this session). Years used are best estimates from contextual evidence in source pages: Alarcon (~2023), Aoki (~2023 based on December 2022 survey date), Banovic (~2022 based on August–September 2021 study date). Files are named accordingly; years should be verified against the original PDFs.

---

## 2026-04-19 — First batch of methods pages: 11 papers (Karagoz through Li)

**Operation**: Created methods pages for 11 papers that had source pages but no corresponding methods pages. Also created `wiki/methods/index.md` (did not previously exist) and updated `wiki/index.md` Methods Pages section.

**Methods pages created**:
- `karagoz-2025-methods.md` ← Karagoz et al. (2025) — XIMED dual-loop RCT (N=97 medical experts, LIME vs. SHAP)
- `karran-2022-methods.md` ← Karran et al. (2022) — Design for Confidence (N=206 online + N=19 lab, explanation visualization design)
- `kleizen-2023-methods.md` ← Kleizen et al. (2023) — Belgian citizen experiments (N=1,269 + N=738, ethical AI disclosures)
- `knapic-2021-methods.md` ← Knapic et al. (2021) — LIME/SHAP/CIU comparison (N=60, gastric bleeding detection)
- `kornowicz-2025-methods.md` ← Kornowicz & Thommes (2025) — Feature selection method experiment (N=216, Prolific)
- `la-gatta-2021-methods.md` ← La Gatta et al. (2021) — PASTLE technical paper + user study (N=36)
- `larasati-2023-methods.md` ← Larasati et al. (2023) — Meaningful explanation participatory design + surveys (N=55, N=88)
- `lee-chew-2023-methods.md` ← Lee & Chew (2023) — Counterfactual explanations overreliance experiment (N=17)
- `lee-limeade-2023-methods.md` ← Lee et al. (2023) — LIMEADE framework + user study (N=21 CS researchers)
- `leichtmann-2023-methods.md` ← Leichtmann et al. (2023) — Mushroom XAI experiment (N=410, Austria)
- `li-2025-methods.md` ← Li et al. (2025) — GenAI vs. XAI grading explanations (N=60 educators, Prolific)

**Also created**:
- `wiki/methods/index.md` — Cross-study methods index table (11 rows, one per paper above)

**Updated**:
- `wiki/index.md` — Methods Pages section updated from placeholder to listing all 11 new pages

---

## 2026-04-18 — Single ingest: Knapic et al. (2021)

**Source ingested**: `Knapic et al._Explainable_Artificial_Intelli.pdf` → `wiki/sources/knapic-xai-medical-decision-support.md`

**What changed**:
- Created source page `knapic-xai-medical-decision-support.md`
- Updated `wiki/concepts/explainability.md`: added CIU method description; added three-way transparency/interpretability/explainability distinction; added SHAP complexity/null-effect finding
- Updated `wiki/findings/rq2-relationships.md`: added Knapic et al. to null-effects table; extended the null-effect pattern note with explanation-capacity mismatch condition
- Updated `wiki/findings/rq3-user-roles.md`: added Knapic et al. to under-specified expertise list with explicit note on medical domain / lay user gap
- Updated `wiki/index.md`: count 86→87; added entry for new source page

---

## 2026-04-18 — Full initial ingest: 86 sources, 22 concept pages, 3 findings pages

**Operation**: First-time wiki build. All 87 PDFs in `raw/` were batch-converted to text via `pdftotext`, then read and ingested in parallel batches. One PDF (`Knapič et al._Explainable_Artificial_Intelli.pdf`) failed to convert due to special characters in the filename; no source page was created for it.

**Source pages created** (86 files in `wiki/sources/`):

- `alarcon-trust-process-ml.md` ← Alarcon et al. — calibrated vs. uncalibrated ML models on user trust and performance
- `angerschmid-fairness-explanation-ai.md` ← Angerschmid et al. — explanation type and fairness level jointly affect trust in health AI
- `aoki-xai-government.md` ← Aoki — XAI explanation types on perceived fairness and trust in governmental decisions
- `banovic-being-trustworthy-not-enough.md` ← Banovic et al. — less competent AI can gain trust by exploiting transparency displays
- `bernardo-seva-affective-design-xai.md` ← Bernardo & Seva — XAITC model with affective processing as a route to trust calibration
- `bhaskara-automation-transparency-uav.md` ← Bhaskara et al. — three automation transparency levels in UAV tasks; intermediate optimal
- `bigras-recommendation-agent-adoption.md` ← Bigras et al. — transparent low-cognitive-effort agents improve decision quality
- `brand-neural-model-truthfulness.md` ← Brand et al. — E-BART transformer jointly predicting veracity and generating explanations
- `calisto-personalized-explanations-breast-imaging.md` ← Calisto et al. — personalised AI assertiveness by clinician expertise in breast imaging
- `cau-logic-explanations-uncertainty.md` ← Cau et al. — inductive explanation style most persuasive; drives overreliance
- `cau-spano-xai-cognitive-capabilities.md` ← Cau & Spano — counterfactual explanations uniquely improve accuracy despite lower understandability
- `chu-user-judgement-ai-model.md` ← Chu et al. — labelling AI as "advanced" biases user agreement with identical outputs
- `conati-personalized-xai-education.md` ← Conati et al. — explanation effects moderated by NFC, Conscientiousness, Reading Proficiency
- `conijn-explanations-essay-scoring.md` ← Conijn et al. — accuracy statements and explanations do not increase trust in essay scoring
- `cramer-transparency-recommender-systems.md` ← Cramer et al. — "why" explanations increase acceptance but not overall system trust
- `diprose-physician-understanding-ml.md` ← Diprose et al. — understanding, explainability, and trust in ML risk calculators
- `dominguez-art-recommendations-hci.md` ← Dominguez-Almela et al. — explanations improve recommender satisfaction via understandability and trust
- `du-av-explanations-timing-trust.md` ← Du et al. — before-action AV explanations significantly outperform after-action
- `duan-xai-gender-stereotypes-ai.md` ← Duan et al. — feature-contribution XAI reduces gender stereotyping of AI
- `esmaeilzadeh-patients-perceptions-ai-healthcare.md` ← Esmaeilzadeh et al. — physician-only encounters elicit higher trust than AI-based alternatives
- `fleiss-algorithm-aversion-recruiting.md` ← Fleiß et al. — explanation content matters more than explanation type in recruiting
- `galanti-explainable-process-analytics.md` ← Galanti et al. — SHAP explanations in business process management validated as trusted
- `gunning-aha-darpa-xai-program.md` ← Gunning & Aha — DARPA XAI framework; psychologically grounded XAI evaluation
- `guo-chen-ai-physicians-replacement.md` ← Guo & Chen — patients trust physicians more than AI; explanations improve AI trust
- `hassan-unlocking-black-box-healthcare.md` ← Hassan et al. — XAI for cerebral palsy risk prediction increases expert trust
- `he-analogies-xai-laypeople.md` ← He et al. — analogy-based XAI for laypeople; format effectiveness depends on expertise
- `hernandez-bocanegra-conversational-explanations.md` ← Hernandez-Bocanegra et al. — conversational interactive explanations for recommenders
- `humer-xai-methods-effects-decisions.md` ← Humer et al. — nearest-neighbor examples best improve decision correctness
- `ihongbe-xai-chest-radiology.md` ← Ihongbe et al. — Grad-CAM vs. LIME for AI-assisted chest diagnosis; professionals prefer Grad-CAM
- `jang-yoon-xai-patent-novelty.md` ← Jang & Yoon — XAI–human collaborative framework for patent novelty classification
- `jansen-longitudinal-uncertainty-av.md` ← Jansen et al. — three-day longitudinal study on AV uncertainty visualization and trust
- `jansen-visualizing-imperfect-av.md` ← Jansen et al. — EDULICIT method for AV uncertainty visualization evaluation
- `jaziri-explainable-by-design.md` ← Jaziri & Sassi — hybrid DRL framework with intrinsic explainability; improves trust
- `karagoz-ximed-medical-imaging.md` ← Karagoz et al. — XIMED framework integrating faithfulness and human-centered trust assessments
- `karran-design-for-confidence.md` ← Karran et al. — lower-clarity explanation visualizations maximize user confidence
- `kleizen-citizens-trustworthy-ai.md` ← Kleizen et al. — ethical AI measures have minimal trust effect; prior attitudes dominate
- `kornowicz-algorithm-expert-reliance.md` ← Kornowicz & Thommes — attitude–behaviour gap in feature-selection transparency
- `la-gatta-pastle-local-explanations.md` ← La Gatta et al. — PASTLE local XAI technique with directional feature-importance
- `larasati-meaningful-explanations-medical-ai.md` ← Larasati et al. — 14 explanation guidelines for healthcare AI
- `lee-chew-counterfactual-explanations-trust.md` ← Lee & Chew — counterfactual explanations reduce overreliance on wrong AI by 21%
- `lee-limeade-explanations-advice-taking.md` ← Lee et al. — LIMEADE; acting on explanations increases trust, control, and satisfaction
- `leichtmann-xai-trust-high-risk.md` ← Leichtmann et al. — visual XAI improves high-risk decision accuracy; AI literacy intervention does not
- `li-ai-natural-language-explanations.md` ← Li et al. — GenAI NL explanations outperform XAI highlights for grading feedback
- `lim-ai-apologies-trust-forgiveness.md` ← Lim et al. — human-attributed apologies outperform AI-attributed on trust and forgiveness
- `liu-in-ai-we-trust.md` ← Liu — real vs. placebic transparency; real transparency reduces uncertainty
- `lundberg-xai-invehicle-intrusion-detection.md` ← Lundberg et al. — SHAP-based VisExp for automotive intrusion detection; trust increased
- `mourali-posthoc-explanations-consumer.md` ← Mourali et al. — actionable sensitivity explanations improve consumer trust perceptions
- `mukhtar-explanations-fault-prediction.md` ← Mukhtar et al. — NL explanations most effective; LIME visualizations no better than no explanation
- `musick-recommendations-benefits.md` ← Musick et al. — benefit-focused explanations increase trust competence, reduce privacy concerns
- `naiseh-c-xai-framework.md` ← Naiseh et al. — C-XAI participatory design framework for trust calibration
- `naiseh-explanation-classes-trust-calibration.md` ← Naiseh et al. — Local/Example/Counterfactual/Global XAI classes; all risk overreliance
- `nelekar-conversational-agents-stress-trust.md` ← Nelekar et al. — ECA stress reduction; trust moderated by culture and personality
- `okolo-xai-community-health-workers.md` ← Okolo et al. — LIME/SHAP incomprehensible to low-literacy CHWs; explanations reinforce overreliance
- `panigutti-codesign-xai-clinical.md` ← Panigutti et al. — co-design with Doctor XAI; explanations increase implicit but not explicit trust
- `papenmeier-its-complicated-transparency-trust.md` ← Papenmeier et al. — accuracy-conditional explanation effects; self-report/behavioural dissociation
- `park-ai-ux-defense-system.md` ← Park et al. — 9-factor AI UX questionnaire validated in military defense context
- `perlmutter-example-based-xai-pipeline.md` ← Perlmutter et al. — example-based XAI with oil-and-gas experts; trust increases, performance stable
- `rezaeian-ai-explanations-clinician-trust.md` ← Rezaeian et al. — most detailed explanation degraded understandability and diagnosis accuracy
- `sajno-ai-says-better.md` ← Sajno et al. — Learning to Defer + XAI protocol; psychological moderators foregrounded
- `salehi-mast-trustworthy-ai-dss.md` ← Salehi et al. — MAST checklist validation for trustworthy AI DSS
- `schilke-transparency-dilemma.md` ← Schilke & Reimann — AI disclosure by humans decreases interpersonal trust (13 experiments)
- `schmager-citizens-ai-public-services.md` ← Schmager et al. — citizens' stances on AI in public services; social contract framing
- `schrills-franke-traceability-ai-systems.md` ← Schrills & Franke — SIPA/traceability construct; subjective vs. objective transparency divergence
- `shin-explainability-causability-trust.md` ← Shin — causability vs. explainability distinction; dual-process model of algorithmic trust
- `shulner-fairness-explainability.md` ← Shulner-Tal et al. — fairness perceptions driven by decision outcome, not explanation type
- `spitzer-imperfections-xai.md` ← Spitzer et al. — imperfect XAI and expertise; novices deceived, experts detect incorrect XAI
- `suen-hung-trust-video-interviews.md` ← Suen & Hung — tangibility, immediacy, disclosure effects on cognitive and affective trust in AI interviews
- `suffian-fce-counterfactual-feedback.md` ← Suffian et al. — FCE user-feedback-driven counterfactual method; more actionable explanations
- `suffian-user-feedback-understanding-trust.md` ← Suffian et al. — UFCE vs. DiCE; UFCE improves performance, understanding, and reliance
- `sun-transparency-performance-expectations.md` ← Sun et al. — transparency benefits trust only when AI performance violates prior expectations
- `sun-trust-human-vs-ai-health-info.md` ← Sun et al. — actual vs. disclosed AI source effects on health information trust
- `tatasciore-concurrent-tasks-transparency.md` ← Tatasciore et al. — high transparency improved accuracy under divided attention but increased automation bias
- `tatasciore-loft-time-pressure-transparency.md` ← Tatasciore & Loft (2024) — transparency improved accuracy but did not buffer time-pressure degradation
- `tatasciore-loft-transparency-effects.md` ← Redirect to [[tatasciore-loft-time-pressure-transparency]] (duplicate raw file)
- `tintarev-masthoff-explanation-effectiveness.md` ← Tintarev & Masthoff — personalized explanations improve satisfaction but harm decision effectiveness
- `van-zetten-trust-fairness-mortgage-ml.md` ← van Zetten et al. — XAI prototypes for mortgage fraud detection improve trust and fairness
- `vered-demand-driven-transparency.md` ← Vered et al. — demand-driven transparency increases trust and reduces task completion time
- `von-zahn-xai-metacognition.md` ← von Zahn et al. — global XAI improves metacognitive accuracy and increases human-to-AI delegation
- `wang-ding-rationality-explanation-capacity.md` ← Wang & Ding — high-capacity users need valid XAI; low-capacity users show placebo effect
- `weitz-virtual-agents-xai.md` ← Weitz et al. — human-likeness of XAI agent linearly increases trust in AI system
- `woodcock-explanations-symptom-checker.md` ← Woodcock et al. — explanation type effects on trust contingent on prior disease knowledge
- `xian-clinician-xai-critical-care.md` ← Xian et al. — dual-encoded heatmap preferred for ICU intubation prediction; cognitive fit
- `yeganejou-interpretable-fuzzy-classifier.md` ← Yeganejou et al. — CNN-fuzzy hybrid classifier improving interpretability at modest accuracy cost
- `yu-trust-control-human-ai-healthcare.md` ← Yu et al. — transparency amplifies trust when AI correct; accelerates erosion when AI errs
- `zhang-ai-explanations-human-ai-teams.md` ← Zhang et al. — AI teammate explanation effects on trust depend on action type and personality
- `zhao-opacity-algorithm-aversion-workplace.md` ← Zhao et al. — perceived opacity (not inherent distrust) drives algorithm aversion

**Concept pages created** (22 files in `wiki/concepts/`):

*Transparency constructs*: `explainability.md`, `algorithmic-transparency.md`, `process-transparency.md`, `outcome-transparency.md`, `disclosure.md`, `natural-language-explanations.md`, `counterfactual-explanations.md`, `example-based-explanations.md`, `uncertainty-visualization.md`, `causability.md`, `traceability.md`

*Trust constructs*: `cognitive-trust.md`, `affective-trust.md`, `behavioural-trust.md`, `institutional-trust.md`, `algorithmic-trust.md`, `trust-calibration.md`, `appropriate-reliance.md`, `algorithm-aversion.md`

*Moderating factors*: `user-expertise.md`, `domain-context.md`, `perceived-risk.md`

**Findings pages created** (3 files in `wiki/findings/`):

- `rq1-conceptualizations.md` — full taxonomy of transparency and trust constructs; measurement standardization gaps; key conceptual distinctions; summary table of key papers
- `rq2-relationships.md` — effect patterns organized by type: positive linear (~25%), conditional/interaction (~40%), non-linear/inverted-U (~10%), null (~20%), negative (~5%); temporal dynamics; mechanism mediators
- `rq3-user-roles.md` — expertise operationalizations; moderation findings by format, reliance patterns, vulnerability to misleading XAI; cultural/institutional moderators; personalization challenge; gaps

**Infrastructure updated**:
- `wiki/index.md` — complete table of contents covering all 86 source pages, 22 concept pages, 3 findings pages
- `wiki/log.md` — this file

**Known gaps**:
- `Knapič et al._Explainable_Artificial_Intelli.pdf` was not ingested (pdftotext conversion failed due to special characters in filename)
- No methods pages created yet (`wiki/methods/` is empty)

---

## 2026-04-19 — Bulk wiki maintenance run (Phases 1–5)

### Phase 1–2: Methods pages created
87 new methods pages written to `wiki/methods/` covering all ingested articles.
PDF content was extracted from `wiki/sources/` summary pages (pdftoppm unavailable).

### Phase 3: Source file back-links
**Source file** back-link added to all 86 `wiki/sources/` pages linking to corresponding raw PDFs.

### Phase 4: Citation cleanup
25 wiki pages edited (concepts/ and findings/) to replace `(source: FILENAME.pdf)` legacy citations with APA inline format `(Author, Year)`. `## References` sections added to all edited pages.

### Phase 5: Index reconciliation
`wiki/methods/index.md` completed with one row per article (87 total, excluding 1 duplicate PDF entry).
- Pre-existing rows before this phase: 54 (from batches A, D, F, G, H)
- Rows added in this phase: 33 (covering batches B, C, E)
- Total rows after reconciliation: 87
- Duplicate entry excluded: `tatasciore-loft-2024a-methods.md` (duplicate of `tatasciore-loft-2024-methods.md`)
- Extra source file identified: `wiki/sources/tatasciore-loft-transparency-effects.md` (87th source file corresponding to the duplicate PDF; not a new unique paper)
