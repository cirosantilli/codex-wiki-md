# Logarithmic scoring rule

↑ **Parent:** [Strictly proper scoring rule](strictly-proper-scoring-rule.md)

The [logarithmic scoring rule](logarithmic-scoring-rule.md) rewards the [natural logarithm](natural-logarithm.md) of the reported [probability mass](probability-mass.md) or [probability density](probability-density.md) at the observed outcome. The title uses the reward convention. For a binary report $p$, its negative is the [logarithmic loss](logarithmic-loss.md):

$$
L_{\log}(p,y)=-y\ln p-(1-y)\ln(1-p),\qquad 0<p<1.
$$

For $y=1$ this is $-\ln p$; for $y=0$ it is $-\ln(1-p)$. At an endpoint, use these outcome-specific forms: assigning zero [probability](probability.md) to the outcome incurs infinite loss, while assigning it [probability](probability.md) one gives zero. The [natural logarithm](natural-logarithm.md) therefore makes a confidently wrong binary forecast far more costly than the bounded [Brier score](brier-score.md) does.

Under the stipulated [Bernoulli distribution](bernoulli-distribution.md) with $q=0.7$, the expected logarithmic loss is

$$
\mathbb E_{0.7}[L_{\log}(p,Y)]=-0.7\ln p-0.3\ln(1-p).
$$

Its unique minimum is at $p=0.7$, where the expected loss is approximately $0.610864$. At $p=0.2$ it is approximately $1.193550$. More generally, the excess expected logarithmic loss over truthful reporting is the [Kullback-Leibler divergence](kullback-leibler-divergence.md) in the order true law first, reported law second:

$$
\mathbb E_q[L_{\log}(p,Y)]-\mathbb E_q[L_{\log}(q,Y)]
=q\ln\frac qp+(1-q)\ln\frac{1-q}{1-p}
=D_{\rm KL}\!\left(\operatorname{Bernoulli}(q)\Vert\operatorname{Bernoulli}(p)\right).
$$

For $0<q<1$, this [Kullback-Leibler divergence](kullback-leibler-divergence.md) is nonnegative and vanishes only at $p=q$, explaining why the [logarithmic scoring rule](logarithmic-scoring-rule.md) is a [strictly proper scoring rule](strictly-proper-scoring-rule.md). The same [Kullback-Leibler divergence](kullback-leibler-divergence.md) identity applies to [probability density functions](probability-density-function.md) relative to a common [measure](measure-split.md) when the truthful expected [logarithmic loss](logarithmic-loss.md) is finite and the comparison [expected value](expected-value-split.md) is well defined.[Section 3.1, Example 3, and Section 4.1](strictly-proper-scoring-rules-prediction-and-estimation-by-tilmann-gneiting-and-others.md) For sequential forecasts, the existing [prequential log score identity](prequential-log-score-identity.md) explains how logarithmic rewards add over observations.

**Table of contents**

- [Prequential log score identity](prequential-log-score-identity.md)

## ↑ Ancestors (8)

1. [Strictly proper scoring rule](strictly-proper-scoring-rule.md)
2. [Proper scoring rule](proper-scoring-rule.md)
3. [Scoring rule](scoring-rule.md)
4. [Statistical inference](statistical-inference-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (10)

- [Brier score](brier-score.md)
- [Cross-entropy](cross-entropy.md)
- [Kullback-Leibler divergence](kullback-leibler-divergence.md)
- [Linear probability score](linear-probability-score.md)
- [Logarithmic loss](logarithmic-loss.md)
- [Logarithmic scoring rule](logarithmic-scoring-rule.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-34/4/c/solution.md)
- [Proper scoring rule](proper-scoring-rule.md)
- [Relative entropy nonnegativity](relative-entropy-nonnegativity.md)
- [Scoring rule](scoring-rule.md)
