<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A sequence of [integrable random variables](../../../../../../integrable-random-variable.md) $(X_n)$ has [uniform integrability](../../../../../../uniform-integrability.md) exactly when

$$
\boxed{\lim_{K\to\infty}\sup_{n\geq0}\mathbb E\left[|X_n|\mathbf1_{\{|X_n|>K\}}\right]=0.}
$$

The [uniformly integrable martingale convergence theorem](../../../../../../uniformly-integrable-martingale-convergence-theorem.md) states that a [uniformly integrable](../../../../../../uniform-integrability.md) discrete-time [martingale](../../../../../../martingale-split.md) $(M_n)$ has an [integrable random variable](../../../../../../integrable-random-variable.md) $M_\infty$ with

$$
\boxed{M_n\to M_\infty\ \text{almost surely and in }L^1,\qquad M_n=\mathbb E[M_\infty\mid\mathcal F_n].}
$$

Indeed, [uniform integrability](../../../../../../uniform-integrability.md) implies $\sup_n\mathbb E|M_n|<\infty$, so the [martingale convergence theorem](../../../../../../martingale-convergence-theorem.md) gives [almost sure convergence](../../../../../../almost-sure-convergence.md). The combination of [uniform integrability](../../../../../../uniform-integrability.md) and [almost sure convergence](../../../../../../almost-sure-convergence.md) gives [convergence in L1](../../../../../../convergence-in-l1.md). For $m\geq n$, the [martingale](../../../../../../martingale-split.md) identity $\mathbb E[M_m\mid\mathcal F_n]=M_n$ passes to the limit by the [L1 contraction of conditional expectation](../../../../../../l1-contraction-of-conditional-expectation.md).

Conversely, [uniform integrability of conditional expectations](../../../../../../uniform-integrability-of-conditional-expectations.md) shows that a [martingale](../../../../../../martingale-split.md) of the form $M_n=\mathbb E[Y\mid\mathcal F_n]$ for one [integrable random variable](../../../../../../integrable-random-variable.md) $Y$ is [uniformly integrable](../../../../../../uniform-integrability.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
