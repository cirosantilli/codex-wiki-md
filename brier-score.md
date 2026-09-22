# Brier score

↑ **Parent:** [Strictly proper scoring rule](strictly-proper-scoring-rule.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Brier_score)

The binary [Brier score](brier-score.md) applies [squared-error loss](squared-error-loss.md) to a reported success [probability](probability.md) $p$ and the observed indicator $y\in\{0,1\}$. It is a loss, so smaller is better. Its values lie in $[0,1]$: predicting the outcome with certainty gives zero, while assigning it zero [probability](probability.md) gives one. Unlike the [logarithmic scoring rule](logarithmic-scoring-rule.md) loss, the binary [Brier score](brier-score.md) remains bounded even for a confidently wrong forecast.

For a [Bernoulli distribution](bernoulli-distribution.md) with true success [probability](probability.md) $q$, averaging the two squared losses gives

$$
\mathbb E_q[(p-Y)^2]=q(p-1)^2+(1-q)p^2=(p-q)^2+q(1-q).
$$

The report controls only $(p-q)^2$; the remaining term is the [variance](variance-split.md) of the [Bernoulli random variable](bernoulli-distribution.md). Consequently the [Brier score](brier-score.md) is a [strictly proper scoring rule](strictly-proper-scoring-rule.md). At $q=0.7$, the expected loss is $(p-0.7)^2+0.21$, with unique minimum $0.21$ at $p=0.7$. Reporting $p=0.2$ instead gives expected loss $0.46$, despite its better loss on the particular outcome $Y=0$ above.

For several possible categories, the [Brier score](brier-score.md) sums the squared differences between reported [probabilities](probability.md) and observed category indicators. With two categories that sum is $2(p-y)^2$, so its numerical values are twice the binary convention used here, with the same optimizing report. Brier's original [Verification of Forecasts Expressed in Terms of Probability (1950), equation (2)](https://www.u-cursos.cl/ingenieria/2025/1/CI71C/1/material_docente/bajar?bajar=1&id=8745481) averages these category-sum losses over forecasts. [Strictly Proper Scoring Rules, Prediction, and Estimation by Tilmann Gneiting and others](strictly-proper-scoring-rules-prediction-and-estimation-by-tilmann-gneiting-and-others.md) (Section 3.1, Example 1, and Table 1) gives the category-sum and binary forms as negative rewards; negating them gives the losses described here.

## ↑ Ancestors (8)

1. [Strictly proper scoring rule](strictly-proper-scoring-rule.md)
2. [Proper scoring rule](proper-scoring-rule.md)
3. [Scoring rule](scoring-rule.md)
4. [Statistical inference](statistical-inference-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Brier score](brier-score.md)
- [Linear probability score](linear-probability-score.md)
- [Logarithmic scoring rule](logarithmic-scoring-rule.md)
- [Proper scoring rule](proper-scoring-rule.md)
- [Scoring rule](scoring-rule.md)
- [Strictly proper scoring rule](strictly-proper-scoring-rule.md)
