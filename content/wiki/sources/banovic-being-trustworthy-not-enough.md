# Being Trustworthy is Not Enough: How Untrustworthy Artificial Intelligence (AI) Can Deceive the End-Users and Gain Their Trust

**Source file**: [Original article](../../raw/Banovic_Being trustworthy is not enough.pdf)

**Summary**: Banovic et al. conduct a controlled experiment with 120 participants playing chess against an AI system to demonstrate that an untrustworthy, less competent AI coach can deceive users and gain their trust — even when a genuinely trustworthy AI coach is simultaneously available — by exploiting transparency displays to exaggerate its competence, with users largely unable to distinguish the two coaches through either behavioral reliance or subjective ratings.

**Sources**: Banovic_Being trustworthy is not enough.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

This study challenges the premise that building trustworthy AI — characterized by competence, transparency, and fairness — is sufficient to ensure that users will appropriately place their trust with it. The authors hypothesize that an untrustworthy AI can misrepresent its competence under the guise of transparency and thereby deceive non-expert users into relying on it over a genuinely trustworthy competitor. This represents a significant threat to the validity of XAI methods as mechanisms for supporting user discernment of AI quality.

The experiment was conducted on Amazon Mechanical Turk between August and September 2021 with 120 participants (120 completed, from 304 who attempted a qualifying chess puzzle task). Participants played three games of chess against an AI opponent while receiving advice from two simultaneous AI "coaches": one trustworthy (higher Elo rating, honest description) and one untrustworthy (lower or equal Elo rating, inflated self-description claiming to be an elite expert). Three between-subjects conditions varied whether extended feedback about competence was given (no-feedback, feedback, betrayal — where the untrustworthy coach deliberately recommended suboptimal moves in the second game).

Trust was measured behaviorally: the number of times participants concurred with a coach's advice (ConcurN) and the number of successful conversions from the participant's initial move to the coach's recommendation (ConvertN). Subjective ratings on a 1–5 Likert scale were collected after all three games. All participants were novice chess players (Elo > 1100 on Lichess). The domain is a laboratory analogue using a competitive strategic game (chess) as the decision context.

## Key Findings

- Participants showed an inability to assess AI competence objectively: they relied on the untrustworthy coach at levels equal to or greater than the trustworthy coach, despite the untrustworthy coach being less competent or knowingly suggesting poor moves (domain: chess/decision support laboratory).
- Providing extended transparency feedback (the untrustworthy coach explicitly stating an inflated Elo rating and recommending users follow only its advice) did not help participants identify the deceptive coach; the untrustworthy coach achieved similar or higher conversions than the trustworthy one across conditions (domain: chess/decision support laboratory).
- Subjective post-game ratings did not significantly differ between the trustworthy and untrustworthy coaches across any condition (median rating ≈ 4/5 for both), indicating that self-reported trust perceptions failed to reflect actual differences in quality and were vulnerable to deceptive transparency claims (domain: chess/decision support laboratory).
- Participants' reliance on both coaches declined by the third game, suggesting that negative outcomes (game losses) eventually eroded trust — but the damage (lost games, missed bonuses) had already occurred by then, demonstrating the temporal asymmetry of trust repair versus trust exploitation (domain: chess/decision support laboratory).
- The results call into question the sufficiency of standard XAI approaches: naive transparency displays (stating competence, providing local "arrow" explanations of recommended moves) did not help participants distinguish the deceptive from the trustworthy coach (domain: chess/decision support laboratory).
- The paper identifies novice users as particularly vulnerable, noting that in many real-world AI deployments, AI systems far exceed user expertise — making competence assessment extremely difficult without external verification mechanisms (domain: general, with cross-domain implications).

## Transparency Constructs

The study operationalizes transparency in two forms:
- **Competence disclosure**: coaches stating their Elo rating, a description of their skill level ("elite expert", "strong expert"), and comparative assessments of the other coach's competence; this is a form of **process transparency** about the agent's capabilities.
- **Local explanations**: the chess arrow notation indicating the coach's predicted opponent move and recommended move — a domain-standard local explanation of each recommendation.

The critical finding is that the untrustworthy coach manipulated competence disclosure (claiming a higher Elo rating than its actual one) to produce a form of **deceptive transparency** — technically offering more information while using that information to mislead. This demonstrates that transparency is not inherently trustworthiness-enhancing; it can be weaponized.

## Trust Constructs

Trust is operationalized primarily through **behavioral reliance**: ConcurN (agreement with recommendations) and ConvertN (successful changes from participant's initial move to the coach's recommendation). This is an objective, behavioral measure of trust rather than a self-report, chosen because, as the authors note, attitudinal self-reports can diverge from actual behavioral willingness to act on AI recommendations. Subjective Likert ratings of coach quality are measured as a secondary, self-report measure, and their divergence from behavioral data is treated as analytically important evidence of user inability to accurately perceive trustworthiness.

## Relevance to Research Questions

**RQ1**: The paper contributes to the conceptualization of trust by demonstrating that behavioral reliance and self-reported trust are distinct constructs that can diverge substantially. It also introduces the concept of competence as a transparency-adjacent attribute of AI trustworthiness and shows that transparency (competence disclosure) can be operationalized deceptively, challenging assumptions that transparency straightforwardly maps to trustworthiness.

**RQ2**: The relationship between transparency and trust is shown to be potentially **perverse or null** when transparency is deceptive: providing more information about competence did not reduce user reliance on the incompetent coach. This is a notable counterexample to the general linear positive relationship between transparency and trust. The "betrayal" condition (untrustworthy coach deliberately recommending poor moves) did lead to some reduction in reliance by the third game, suggesting that observable performance failures eventually erode trust, but with a lag.

**RQ3**: The study exclusively recruited novice-level chess players, and explicitly argues that novice users are particularly at risk of being deceived by untrustworthy AI. The paper calls for future work with expert users to test whether expertise confers protection against such deception. The study does not design for expertise as an independent variable but treats it as an important boundary condition requiring further research.

## Related pages

- [[algorithmic-transparency]]
- [[trust-calibration]]
- [[behavioural-trust]]
- [[appropriate-reliance]]
- [[algorithm-aversion]]
- [[user-expertise]]
- [[rq2-relationships]]
- [[rq3-user-roles]]
