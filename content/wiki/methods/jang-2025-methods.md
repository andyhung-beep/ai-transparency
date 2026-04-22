# Jang & Yoon 2025 — Methods

**Summary**: A computational study evaluating an XAI–human collaborative framework for patent novelty classification using a self-explaining deep neural network (RoBERTa-based) on 30,918 patent pairs from the EPO dataset, with expert feedback incorporated via a modified loss function; includes a human-AI interaction component comparing expert-guided (Type 1) and XAI-guided (Type 2) feedback.

**Sources**: Jang & Yoon_An explainable artificial intelligence-human collaborative model.pdf

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-19

---

## Study design
technical paper (computational modeling with human-in-the-loop evaluation component; not a controlled user experiment)

## Sample
- N: 30,918 patent pairs (EPO full-text dataset); number of expert participants providing feedback not reported
- Population: technical domain experts (patent examiners and R&D practitioners) for the feedback component
- Domain: intellectual property / patent analysis (technology management)
- Country / region: European Patent Office dataset; participant country not reported
- Recruitment method: not reported

## Transparency operationalization
- Type: intrinsic / self-explaining explainability — claim-level relevance scores (saliency weights) produced as part of the model's loss function; not post-hoc but model-native
- Manipulation or measure: two experimental feedback types compared: Type 1 — expert provides advice independently of XAI explanations (reviews all claims); Type 2 — expert provides advice guided by XAI explanations (reviews top-3 highest-relevance claims only); lambda parameter varied (0.1–0.9) to control the weight of self-explainability in the loss function
- Scale / instrument name: not applicable (computational metric — claim-level relevance scores)
- Number of items: not applicable

## Trust operationalization
- Type: not directly measured; trust is treated as an implicit motivator (black-box AI is argued to create trust barriers; XAI is proposed to address them); appropriate reliance is discussed at the design level
- Measure: no trust measure administered; model performance (accuracy, F1 score) used as the primary outcome; reference to automation bias (Bond et al., 2019) and appropriate reliance as design rationale
- Scale / instrument name: not applicable
- Number of items: not applicable
- Behavioural vs self-report: not applicable

## Moderators and covariates tested
- Lambda parameter (self-explainability weight): varied from 0.1 to 0.9; higher lambda increased self-explainability but reduced source model accuracy; moderated the performance–explainability trade-off
- Feedback type (Type 1 vs. Type 2): comparison of expert advice provided independently vs. guided by XAI explanations; near-equivalent performance (F1 difference of 0.001 at lambda=0.6) suggesting XAI guidance does not substantially distort expert judgment
- User expertise: domain experts (patent examiners, R&D professionals) are the assumed user population; expertise is treated as a prerequisite for the collaboration model — relevant to RQ3; non-expert users are not studied

## Statistical approach
- Primary analysis method: performance comparison using accuracy and F1 score across model variants and lambda settings; base model vs. refined model comparison
- Software: not reported
- Key model fit or effect size reported: accuracy 0.890, F1 0.916 (refined model at lambda=0.6); source model accuracy 0.589, F1 0.652; base model (additional training, no advice) F1 0.875

## Author-noted limitations
- Unconditional trust in expert advice is assumed; if experts provide incorrect advice, model performance could degrade
- The framework assumes expert domain knowledge is available and reliable; scalability to contexts where expert feedback is scarce or inconsistent is uncertain
- Type 2 (XAI-guided) advice reviews only top-3 claims, which may miss relevant claims; this is balanced against efficiency
- The self-explaining model shows a performance–explainability trade-off at the source model level (higher lambda reduces accuracy before human feedback is incorporated)
- No user study measuring trust, cognitive load, or user experience was conducted; human-in-the-loop component is described but experimental details of the expert feedback process are limited
- Non-expert participants have been overrepresented in prior XAI collaboration studies; this paper does not correct that gap empirically (addresses it only argumentatively)

## Related pages
- [[jang-yoon-xai-patent-novelty]]
- [[explainability]]
- [[traceability]]
- [[causability]]
- [[appropriate-reliance]]
- [[user-expertise]]
- [[behavioural-trust]]

## References
Jang, H., & Yoon, J. (2025). An explainable artificial intelligence–human collaborative model for investigating patent novelty. *Engineering Applications of Artificial Intelligence*.
