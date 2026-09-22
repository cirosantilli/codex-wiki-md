# Scoring rule

↑ **Parent:** [Statistical inference](statistical-inference-split.md)

A [scoring rule](scoring-rule.md) turns a [probability distribution](probability-distribution-split.md) forecast and an observed outcome into a number. For example, a forecast of rain with [probability](probability.md) $0.7$ should express uncertainty more usefully than a bare prediction of rain. A [scoring rule](scoring-rule.md) lets us compare such forecasts after observations arrive, and its choice determines whether exaggerating confidence pays. A [proper scoring rule](proper-scoring-rule.md) rewards an honest account of uncertainty in [expected value](expected-value-split.md).

There are two sign conventions. A reward $S(P,x)$ is maximized; a [loss function](loss-function.md) $L(P,x)$ is minimized. The conversion $L=-S$ reverses every comparison. Here the [linear probability score](linear-probability-score.md) is a reward, while the binary [Brier score](brier-score.md) and the negative [logarithmic scoring rule](logarithmic-scoring-rule.md) are losses. Calling all three a "score" without specifying the direction would hide the central difference.

Throughout the binary examples, the [random variable](random-variable-split.md) $Y$ has a [Bernoulli distribution](bernoulli-distribution.md) with actual success [probability](probability.md) $q=0.7$, and the report $p\in[0,1]$ assigns [probability](probability.md) $p$ to $Y=1$ and $1-p$ to $Y=0$. The value $q=0.7$ is stipulated by this [statistical model](statistical-model-split.md); it is not inferred from data or a claim that a forecasting system is calibrated. In practice the true [predictive distribution](predictive-distribution.md) is unknown, and the relevant $q$ is the [conditional probability](conditional-probability.md) of success given the information available when the forecast is issued. [Propriety](proper-scoring-rule.md) evaluates incentives for reporting that [predictive distribution](predictive-distribution.md); it does not supply the unknown [probabilities](probability.md).

**Table of contents**

- [Linear probability score](linear-probability-score.md)
- [Proper scoring rule](proper-scoring-rule.md)
  - [Strictly proper scoring rule](strictly-proper-scoring-rule.md)
    - [Brier score](brier-score.md)
    - [Logarithmic scoring rule](logarithmic-scoring-rule.md)
      - [Prequential log score identity](prequential-log-score-identity.md)

## ↑ Ancestors (5)

1. [Statistical inference](statistical-inference-split.md)
2. [Probability and statistics](probability-and-statistics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-34/4/a/solution.md)
- [Scoring rule](scoring-rule.md)
