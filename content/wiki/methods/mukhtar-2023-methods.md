# Mukhtar et al. 2023 — Methods

**Summary**: A between-subjects user study (N = 120) comparing four explanation styles (blackbox, LIME-based visualisation, natural language, human-authored) for a machine-learning spreadsheet fault prediction tool on fault comprehension, trust, and behavioural intention among experienced spreadsheet users.

**Sources**: Mukhtar et al._Explain software fault predictions to spreadsheet users.pdf

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-19

---

## Study design
experimental (between-subjects)

## Sample
- N: 120
- Population: experienced spreadsheet users; over 50% with 7+ years of spreadsheet experience; daily users; screened for spreadsheet experience via Prolific
- Domain: software engineering / developer tooling
- Country / region: not reported (Prolific Academic, international)
- Recruitment method: Prolific Academic

## Transparency operationalization
- Type: outcome transparency and process transparency — post-hoc feature importance explanations for ML fault predictions
- Manipulation or measure: four between-subjects conditions: (1) Blackbox — ranked list of suspicious cells with no explanation; (2) Visualization — LIME-based feature importance chart; (3) NaturalLanguage — LIME features translated into plain English sentences (e.g., "References to cells that are to the left or above this cell may be missing."); (4) HumanExplanation — manually crafted expert explanation (upper performance bound); participants examined a real-world Enron Error corpus spreadsheet with three faulty cells; tool evaluated is SmellChecker (metric-based ML fault prediction)
- Scale / instrument name: not applicable (experimental manipulation); transparency perception measured via single Likert item T1: "I understand why the cells were marked suspicious through the explanations" (1–5 scale)
- Number of items: 1 (transparency item T1)

## Trust operationalization
- Type: cognitive and behavioural
- Measure: two Likert items: TC1 — "explanations are trustworthy" (1–5 scale); TC2 — "overall, I trust SmellChecker" (1–5 scale); behavioural intention items: I1 "would use again" (1–5); recommendation intention R1; satisfaction items also collected
- Scale / instrument name: custom Likert items developed by authors
- Number of items: 2 (trust items TC1, TC2); additional behavioural intention and satisfaction items not fully enumerated in available sources
- Behavioural vs self-report: self-report for all trust items; behavioural intention is self-reported intention (not actual use)

## Moderators and covariates tested
- Explanation type (four levels): primary independent variable; not a moderator per se but the central manipulation
- Spreadsheet experience: measured as a participant characteristic (years of experience, frequency of use); the study samples experienced users but does not formally test experience as a moderator within the study — relevant to RQ3 as the population is specifically intermediate-expertise domain users
- User expertise / AI literacy: not formally tested as a moderator; sample is screened for domain (spreadsheet) expertise rather than AI expertise

## Statistical approach
- Primary analysis method: ANOVA (one-way) for between-group comparisons on comprehension, trust, and satisfaction; qualitative review of participant behaviour for visualization condition
- Software: not reported
- Key model fit or effect size reported: group means for comprehension (HumanExplanation = 1.83/2, NaturalLanguage = 1.58/2, Blackbox = 1.40/2, Visualization = 1.12/2); trust means (TC1: HumanExplanation = 4.47, NaturalLanguage = 4.07, Blackbox = 4.07, Visualization = 3.50; TC2: HumanExplanation = 4.27, NaturalLanguage = 4.23, Blackbox = 3.87, Visualization = 3.57); ANOVA confirmed significant differences between conditions on fault comprehension measures

## Author-noted limitations
- Sample restricted to experienced spreadsheet users; findings may not generalise to novice users or non-spreadsheet domains
- Only one real-world spreadsheet (Enron Error corpus) was used; generalisability to other spreadsheet types is unknown
- The LIME-based visualisation was not explicitly designed for lay end-users; a better-designed visualization might have produced different results
- Crowdsourced sample (Prolific) may not fully represent professional spreadsheet users in enterprise settings
- Small N per condition limits statistical power for secondary analyses
- Trust measured via two single items; validated multi-item trust scales were not used

## Related pages
- [[mukhtar-explanations-fault-prediction]]
- [[natural-language-explanations]]
- [[explainability]]
- [[outcome-transparency]]
- [[cognitive-trust]]
- [[behavioural-trust]]
- [[user-expertise]]
- [[rq2-relationships]]
