# Linear probability score

↑ **Parent:** [Scoring rule](scoring-rule.md)

The [linear probability score](linear-probability-score.md) pays the reported [probability](probability.md) of whichever binary outcome occurs. With report $p$ and observed $y\in\{0,1\}$, its reward is

$$
S_{\rm lin}(p,y)=yp+(1-y)(1-p).
$$

It looks sensible: assign more [probability](probability.md) to what happens and receive more reward. But the [expected value](expected-value-split.md) under a [Bernoulli distribution](bernoulli-distribution.md) with true success [probability](probability.md) $q$ is

$$
\mathbb E_q[S_{\rm lin}(p,Y)]=qp+(1-q)(1-p)=1-q+(2q-1)p.
$$

This is an [affine function](affine-function.md) of the report. When $q>1/2$, the maximum over $[0,1]$ is at $p=1$; when $q<1/2$, it is at $p=0$. At $q=1/2$, every report ties. Thus the [linear probability score](linear-probability-score.md) encourages reporting certainty about the more likely outcome and is not a [proper scoring rule](proper-scoring-rule.md).

For the stipulated $q=0.7$, the [expected value](expected-value-split.md) of the reward is $0.3+0.4p$. Honest reporting $p=0.7$ earns $0.58$ in [expectation](expected-value-split.md), whereas $p=1$ earns $0.7$. The forecaster improves expected reward by replacing a 70% forecast with a 100% forecast. The [Brier score](brier-score.md) and [logarithmic scoring rule](logarithmic-scoring-rule.md) avoid this incentive, as the expected-score diagram under [proper scoring rule](proper-scoring-rule.md) shows.

## ↑ Ancestors (6)

1. [Scoring rule](scoring-rule.md)
2. [Statistical inference](statistical-inference-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Linear probability score](linear-probability-score.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-34/4/b/solution.md)
- [Proper scoring rule](proper-scoring-rule.md)
- [Scoring rule](scoring-rule.md)
