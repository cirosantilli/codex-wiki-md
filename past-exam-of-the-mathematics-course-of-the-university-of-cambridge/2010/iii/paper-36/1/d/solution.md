<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Under the [null hypothesis](../../../../../../null-hypothesis.md), $Y\sim\operatorname{Bin}(n,1/2)$, with [expected value](../../../../../../expected-value.md) $n/2$ and [variance](../../../../../../variance-split.md) $n/4$. Approximating its probability at an integer by the [normal distribution](../../../../../../normal-distribution.md) density over a unit-width cell gives

$$
p(y\mid H_0)\approx\frac1{\sqrt{2\pi(n/4)}}\exp\left[-\frac{(y-n/2)^2}{2(n/4)}\right]
=\sqrt{\frac2{\pi n}}\exp\left[-\frac2n(y-n/2)^2\right].
$$

Dividing by the [prior predictive distribution](../../../../../../bayesian-model-evidence.md) from the preceding part gives the [uniform-alternative binomial Bayes factor](../../../../../../uniform-alternative-binomial-bayes-factor.md)

$$
B_{01}(y)\approx(n+1)\sqrt{\frac2{\pi n}}\exp\left[-\frac2n(y-n/2)^2\right]
\approx\boxed{\sqrt{\frac{2n}{\pi}}\exp\left[-\frac2n(y-n/2)^2\right]}.
$$

The second approximation replaces $n+1$ by $n$. Both are large-sample approximations for counts in the central range, rather than exact identities at extreme counts.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
