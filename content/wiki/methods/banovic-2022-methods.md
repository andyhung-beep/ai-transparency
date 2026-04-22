# Banovic et al. (2022) — Methods

**Summary**: Controlled online experiment (N = 120 novice chess players) in which participants played chess against an AI while receiving simultaneous advice from a trustworthy and an untrustworthy AI coach, demonstrating that deceptive competence disclosures allow an untrustworthy AI to gain user trust equal to or exceeding a genuinely trustworthy AI.

**Sources**: Banovic_Being trustworthy is not enough.pdf

**Research questions addressed**: RQ1 / RQ2 / RQ3

**Last updated**: 2026-04-19

---

## Study design
experimental (between-subjects online controlled experiment; three conditions)

## Sample
- N: 120 (from 304 who attempted a qualifying chess puzzle task; 184 excluded during qualification)
- Population: novice chess players (Lichess Elo > 1,100 required; general public screened for novice skill level)
- Domain: chess / decision support laboratory (strategic game used as an analogue for AI-assisted decision making)
- Country / region: United States (Amazon Mechanical Turk)
- Recruitment method: Amazon Mechanical Turk; conducted August–September 2021

## Transparency operationalization
- Type: competence disclosure (process transparency about agent capability) and local explanation (move-level recommendation explanation)
- Manipulation or measure: between-subjects manipulation of feedback condition — (1) no-feedback: both coaches provided only move recommendations via chess arrows without competence claims; (2) feedback: the untrustworthy coach disclosed an inflated Elo rating and described itself as an "elite expert," claiming the trustworthy coach was inferior; (3) betrayal: same as feedback, but the untrustworthy coach deliberately recommended suboptimal moves in the second game to test whether observable failures would erode trust. All conditions included local chess arrow explanations (predicted opponent move and recommended move) as standard presentation. The trustworthy coach disclosed an accurate Elo rating.
- Scale / instrument name: not applicable (transparency was a design manipulation; no transparency scale used)
- Number of items: not applicable

## Trust operationalization
- Type: behavioural (primary) and general self-report (secondary)
- Measure: (1) ConcurN — number of times participants agreed with a coach's recommended move (behavioral trust proxy); (2) ConvertN — number of successful changes from participant's initially planned move to the coach's recommended move (behavioral reliance); (3) post-game Likert scale ratings of coach quality on a 1–5 scale (self-report measure, secondary)
- Scale / instrument name: custom 1–5 Likert coach quality rating; ConcurN and ConvertN behavioral metrics
- Number of items: not reported (Likert scale items count not specified in source summary)
- Behavioural vs self-report: both (ConcurN and ConvertN behavioral; Likert ratings self-report)

## Moderators and covariates tested
- Feedback condition (no-feedback, feedback, betrayal): manipulated between subjects; the betrayal condition was designed to test whether observable performance failures would erode trust in the untrustworthy coach
- Game number (Game 1, 2, 3): within-subjects repeated measure; trust in both coaches declined by Game 3, suggesting temporal erosion with negative outcomes, but the untrustworthy coach's advantage persisted through Games 1 and 2
- Note: user expertise was not an independent variable — all participants were novice chess players by design. The authors explicitly identify novice users as vulnerable to deceptive transparency and call for future research with expert users (directly relevant to RQ3).

## Statistical approach
- Primary analysis method: mixed-model ANOVA (between-subjects: feedback condition; within-subjects: game number, coach identity) for behavioral outcomes; descriptive statistics and Wilcoxon signed-rank tests for Likert ratings
- Software: not reported
- Key model fit or effect size reported: significance thresholds reported; median Likert ratings reported (approximately 4/5 for both coaches across conditions); specific effect sizes (Cohen's d, η²) not reported in source summary

## Author-noted limitations
- Novice-only sample limits generalizability to expert users, who may be better equipped to evaluate AI competence claims
- Chess is an artificial context; results may not generalize to high-stakes professional AI deployments (e.g., clinical diagnosis, legal decision making)
- Qualifications stage (chess puzzle task) may have introduced selection bias toward more chess-engaged MTurk workers
- The untrustworthy coach's deception was based on competence inflation; other deception strategies (e.g., manipulated accuracy statistics) were not tested
- Self-reported trust and behavioral reliance diverged substantially, raising questions about which is the more valid trust indicator
- The study did not measure individual differences (e.g., disposition to trust, AI familiarity) that may moderate susceptibility to deceptive transparency

## Related pages
- [[banovic-being-trustworthy-not-enough]]
- [[algorithmic-transparency]]
- [[trust-calibration]]
- [[behavioural-trust]]
- [[appropriate-reliance]]
- [[algorithm-aversion]]
- [[user-expertise]]
- [[rq2-relationships]]
- [[rq3-user-roles]]

## References
Banovic, N., et al. (2022). *Being trustworthy is not enough: How untrustworthy artificial intelligence (AI) can deceive the end-users and gain their trust*. [Journal not reported in source summary.]
