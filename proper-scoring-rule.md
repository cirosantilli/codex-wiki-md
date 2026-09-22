# Proper scoring rule

↑ **Parent:** [Scoring rule](scoring-rule.md)

A [proper scoring rule](proper-scoring-rule.md) makes reporting the true [probability distribution](probability-distribution.md) optimal in [expected value](expected-value.md), for every true [probability distribution](probability-distribution.md) in the allowed class of forecasts. In the reward convention, the inequality in the title holds for every report $P$ and true law $Q$. The [expected value](expected-value.md) is always taken under $Q$, because the report does not change how the outcome is generated. In the loss convention the same definition reads

$$
\mathbb E_Q[L(Q,X)]\leq\mathbb E_Q[L(P,X)]\qquad\text{for every admissible }P,Q.
$$

This requirement makes a [proper scoring rule](proper-scoring-rule.md) useful for eliciting [probabilities](probability.md) and comparing [predictive distributions](predictive-distribution.md): deliberately distorting a known forecast cannot improve its expected reward or expected loss. The reward convention and its strict version are set out in [Strictly Proper Scoring Rules, Prediction, and Estimation by Tilmann Gneiting and others](strictly-proper-scoring-rules-prediction-and-estimation-by-tilmann-gneiting-and-others.md) (Section 1).

For the [Bernoulli distribution](bernoulli-distribution.md) with $q=0.7$, the [Brier score](brier-score.md) has expected loss $(p-0.7)^2+0.21$, and the negative [logarithmic scoring rule](logarithmic-scoring-rule.md) has expected loss $-0.7\ln p-0.3\ln(1-p)$. Both are minimized at the honest report $p=0.7$. The [linear probability score](linear-probability-score.md), by contrast, maximizes its expected reward at $p=1$. These are statements about averaging over both possible outcomes with their actual [probabilities](probability.md).

<a id="image-expected-losses-of-the-brier-score-and-logarithmic-scoring-rule-favor-p-q-0-7-the-linear-probability-score-rewards-p-1"></a>
![](proper-score-expected-losses.png)

**[Figure 4](#image-expected-losses-of-the-brier-score-and-logarithmic-scoring-rule-favor-p-q-0-7-the-linear-probability-score-rewards-p-1). Expected losses of the Brier score and logarithmic scoring rule favor $p=q=0.7$; the linear probability score rewards $p=1$**.

The left panel displays each excess expected loss divided by that rule's expected loss at $p=q$: $0.21$ for the [Brier score](brier-score.md) and approximately $0.610864$ for the [logarithmic scoring rule](logarithmic-scoring-rule.md). This normalization permits comparison of curve shapes and preserves the minimizing report, since it subtracts a constant and divides by a positive constant independent of $p$. Zero means no excess expected loss. The right panel shows the unmodified [linear probability score](linear-probability-score.md) reward, with its maximizing direction labeled explicitly.

**Table of contents**

- [Strictly proper scoring rule](strictly-proper-scoring-rule.md)
  - [Brier score](brier-score.md)
  - [Logarithmic scoring rule](logarithmic-scoring-rule.md)
    - [Prequential log score identity](prequential-log-score-identity.md)

## ↑ Ancestors (6)

1. [Scoring rule](scoring-rule.md)
2. [Statistical inference](statistical-inference-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Linear probability score](linear-probability-score.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-34/4/a/solution.md)
- [Proper scoring rule](proper-scoring-rule.md)
- [Scoring rule](scoring-rule.md)
- [Strictly proper scoring rule](strictly-proper-scoring-rule.md)
