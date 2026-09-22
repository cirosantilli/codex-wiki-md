<h1 id="2/e/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

**The [covariance](../../../../../../../covariance.md) is zero.** Let $\mathcal F_t=\sigma(\varepsilon_s:s\leq t)$. The stationary noise-series representation makes $f(X_t)$ measurable with respect to $\mathcal F_t$, whereas the [martingale difference sequence](../../../../../../../martingale-difference-sequence.md) property gives $\mathbb E[X_{t+h}\mid\mathcal F_{t+h-1}]=0$. The [law of total expectation](../../../../../../../law-of-total-expectation.md) therefore gives

$$
\mathbb E[X_{t+h}f(X_t)]
=\mathbb E\!\left[f(X_t)\mathbb E(X_{t+h}\mid\mathcal F_{t+h-1})\right]=0.
$$

Since $\mathbb EX_{t+h}=0$, this is the required [covariance](../../../../../../../covariance.md). All products are integrable by the [Cauchy-Schwarz inequality](../../../../../../../cauchy-schwarz-inequality.md), using finite [second moments](../../../../../../../second-moment.md) of $X$ and the stipulated square integrability of $f(X_t)$.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [E](../../e.md)
3. [2](../../../2.md)
4. [Paper 37](../../../../paper-37-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
