# User Judgment of an AI Model is Biased by its Description: A Study in a Job Interview Training Context

**Source file**: [Original article](../../raw/Chu et al._User judgement of an AI model.pdf)

**Summary**: A controlled Wizard-of-Oz experiment (N = 42) showing that describing an AI model as "advanced" rather than "basic" — while holding actual system output constant — significantly increased participants' agreement with system outputs, pre-to-post rating shifts toward AI, and willingness to apply feedback, demonstrating that initial framing information about AI origin biases user judgment even before any system capability is observed.

**Sources**: Chu et al._User judgement of an AI model.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Chu et al. (2025) investigate how initial, up-front descriptive information about an AI model — specifically, how technologically sophisticated the model is described to be — shapes users' first impressions and subsequent judgments of system output. The study was conducted in the context of an AI-based job interview training system (JITS) that provided automated scores and feedback on participants' mock interviews (conciseness and verbal anxiety ratings).

The study used a between-subjects Wizard-of-Oz design: all 42 participants received identical simulated system outputs (manually coded interview ratings and feedback), but half were told the system was powered by a "basic" AI (a graduate student's NLTK decision tree trained on 150 transcripts) and half were told it used an "advanced" AI (Meta AI's RoBERTa deep neural network trained on 63 million articles). Only the model description text differed; no actual AI differences existed.

The research is motivated by the concern that non-expert users form lasting first impressions from initial information that may bias their evaluation of AI-generated outputs — a form of anchoring or framing effect distinct from post-hoc explanations.

## Key Findings

- Participants in the advanced AI condition showed significantly less disagreement with the system's numerical ratings (higher human-AI agreement; Mann-Whitney U, p = .007, r = .42). (Domain: job interview training)
- Participants agreed more with the system's constructive textual feedback when shown the advanced AI description (p = .031, r = .33). (Domain: job interview training)
- Participants in the advanced AI condition were significantly more likely to shift their own pre-ratings to align with the AI's ratings after seeing system output (pre-post rating change, p = .004, r = .44). (Domain: job interview training)
- Willingness to apply the system's feedback in future interviews was significantly higher in the advanced condition (p = .044, r = .31). (Domain: job interview training)
- Trust (as measured by the adapted Körber and Madsen & Gregor scales) did not differ significantly between conditions (p = .269), nor did willingness to use the system in future (p = .061, non-significant trend). (Domain: job interview training)
- None of the background variables — interviewing confidence, Big-5 personality, or general propensity to trust AI — moderated the results.
- The effect emerged purely from a one-time, low-effort framing of technical details, without any interactive engagement with explanations or longitudinal exposure.

## Transparency Constructs

The paper operationalises a novel form of transparency: **up-front model description transparency** — the disclosure of an AI system's origin, developer credibility, algorithmic complexity, and training data size prior to any interaction. This is conceptually related to [[disclosure]] and [[algorithmic-transparency]], but distinct from post-hoc [[explainability]].

The "advanced" condition disclosed: developer (Meta AI), architecture (RoBERTa DNN transformer), and training data (63 million news articles + fine-tuning). The "basic" condition disclosed: a graduate student developer, NLTK tokenizer, decision tree, and 150 training transcripts.

This operationalisation sits at the intersection of [[process-transparency]] (how the model was built) and [[outcome-transparency]] (implicit claim about expected accuracy/quality).

## Trust Constructs

The paper examines multiple trust-adjacent constructs:

- **[[behavioural-trust]]** (reliance/behavioural alignment): Operationalised via human-AI rating agreement differences and pre-post rating change — the degree to which participants shifted their judgments toward the AI.
- **Willingness to apply feedback**: Closer to reliance than trust per se (cf. Scharowski et al., 2023, cited in the paper, who distinguish trust as attitude from reliance as behaviour).
- **Explicit [[cognitive-trust]]**: Measured via Körber Trust in Automation scale and Madsen & Gregor Human-Computer Trust items — not significantly different between conditions.

The key finding is a dissociation: framing affected behavioural alignment (reliance) but not self-reported trust, suggesting that up-front framing information operates on users' implicit judgments and behaviours without necessarily changing their consciously held trust attitudes.

## Relevance to Research Questions

**RQ1**: Contributes a novel operationalisation of transparency as pre-interaction model description rather than post-hoc explanation. Highlights that users' mental models of AI quality are shaped by framing cues about technical sophistication, developer reputation, and data scale — not only by observed performance or explicit explanations.

**RQ2**: Demonstrates a conditional, framing-based transparency–reliance effect: transparency about model origin (even when artificially constructed) increases behavioural alignment with AI outputs. However, the effect does not extend to self-reported trust or longer-term usage intentions, indicating a bounded relationship between transparency cues and trust. The effect is a form of overreliance risk: users defer more to a system they believe is sophisticated, regardless of actual output quality.

**RQ3**: Sample was recruited from computer science courses, providing at least some technical background. The authors note that the framing effect may require a minimum level of technical literacy (enough to understand descriptions of DNN vs. decision tree) and call for replication with varied expertise levels. Directly relevant to [[user-expertise]] as a moderator: novice non-technical users may not respond to the same framing cues.

## Related pages

- [[disclosure]]
- [[algorithmic-transparency]]
- [[behavioural-trust]]
- [[cognitive-trust]]
- [[appropriate-reliance]]
- [[algorithm-aversion]]
- [[rq2-relationships]]
- [[rq3-user-roles]]
