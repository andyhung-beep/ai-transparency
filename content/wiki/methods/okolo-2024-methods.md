# Okolo et al. 2024 — Methods

**Summary**: A qualitative field study with 35 low-literacy community health workers (CHWs) in rural Uttar Pradesh, India, examining perceptions of simplified LIME and SHAP explanations presented via a Figma-prototype neonatal jaundice diagnostic AI tool through semi-structured interviews and iterative design probe interactions.

**Sources**: Okolo et al._If it is easy to understand then it will have value.pdf

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-19

---

## Study design
qualitative (field study with semi-structured interviews and iterative design probe interactions)

## Sample
- N: 35
- Population: female community health workers (CHWs / ASHAs) with low digital literacy and no prior AI experience; employed in rural primary healthcare
- Domain: primary / community healthcare (neonatal jaundice diagnosis), rural India
- Country / region: Uttar Pradesh, India
- Recruitment method: purposive sampling through local NGO / health worker networks in rural Uttar Pradesh (specific method not further reported)

## Transparency operationalization
- Type: explainability — simplified visual LIME and SHAP explanations for an AI diagnostic tool
- Manipulation or measure: design probe study using a Figma prototype simulating an AI-based neonatal jaundice diagnostic tool; two XAI visualisations iteratively presented and refined across interviews: (1) LIME-based — yellow/grey colour overlay highlighting contributing body regions (colours modified from standard red/green to avoid medical danger associations); (2) SHAP-based — multiple annotated images with coloured boxes and a horizontal colour bar (yellow/green); visualisations were iteratively redesigned during fieldwork based on CHW feedback; shape-based cues (circles/squares) were tested as alternatives to colour coding in later sessions
- Scale / instrument name: not applicable (qualitative design probe; no formal scale)
- Number of items: not applicable

## Trust operationalization
- Type: behavioural (over-reliance) and institutional
- Measure: trust and reliance assessed qualitatively through interview responses and observation of CHW interactions with the prototype; constructs identified: (1) behavioural over-reliance — uncritical acceptance of AI outputs, including when CHWs could not interpret the explanations; (2) institutional trust — CHWs believed showing the AI app and its explanations to patients would increase their own professional legitimacy and community trust; (3) cognitive trust — attributed high AI competence by analogy with trusted medical devices (thermometer, blood pressure monitor)
- Scale / instrument name: not applicable (qualitative coding of interview data)
- Number of items: not applicable
- Behavioural vs self-report: qualitative observation and self-report within interview context

## Moderators and covariates tested
- User AI literacy: the entire study is framed around the consequences of very low AI and digital literacy for XAI effectiveness; CHWs had no prior AI experience; this is the central user characteristic examined — directly relevant to RQ3
- Cultural colour mental models: CHWs applied public-health colour conventions (green=safe, yellow=warning, red=danger, grey=lack of blood), leading to systematic misinterpretation of LIME/SHAP colour schemes; identified as a critical design moderator — relevant to RQ3
- Numeracy / text literacy: CHWs consistently ignored or could not interpret textual and numerical elements (legends, colorbars, percentage confidence labels, decimal values); limited to purely visual/graphical interpretation
- Familiarity with medical devices: CHWs drew on device-based rather than AI-based mental models, shaping how they interpreted AI outputs

## Statistical approach
- Primary analysis method: thematic analysis of semi-structured interview transcripts; iterative grounded analysis informing design probe refinement
- Software: not reported
- Key model fit or effect size reported: not applicable (qualitative study)

## Author-noted limitations
- All-female sample of CHWs in one Indian state; findings may not generalise to other low-resource contexts or male health workers
- Figma prototype, not a live deployed tool; actual field use may differ
- Iterative redesign of visualisations during data collection introduces confounds between early and late interview sessions
- Trust and reliance assessed qualitatively; no validated trust instruments used
- Researchers are from a WEIRD (Western, Educated, Industrialised, Rich, Democratic) background; positionality may have influenced interpretation
- Design recommendations are preliminary and require further co-design and evaluation with CHWs

## Related pages
- [[okolo-xai-community-health-workers]]
- [[explainability]]
- [[uncertainty-visualization]]
- [[appropriate-reliance]]
- [[user-expertise]]
- [[domain-context]]
- [[institutional-trust]]
- [[rq3-user-roles]]
- [[rq2-relationships]]
