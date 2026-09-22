<h1 id="28j/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Under the null model, $\pi=1$, which is a boundary point of the parameter space. Standard interior-point asymptotic normality of the [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md) therefore need not apply.

Indeed, put $a=1-e^{-\lambda}$. Under $\pi=1$, $N_+\sim\operatorname{Binomial}(n,a)$. For the unconstrained estimator $\widetilde\pi=N_+/(na)$, the [central limit theorem](../../../../../../central-limit-theorem.md) gives

$$
\sqrt n(\widetilde\pi-1)
\xrightarrow{d}W,
\qquad
W\sim N\!\left(0,\frac{1-a}{a}\right)
=N\!\left(0,\frac{e^{-\lambda}}{1-e^{-\lambda}}\right).
$$

Since $\widehat\pi=\min\{1,\widetilde\pi\}$, the [continuous mapping theorem](../../../../../../continuous-mapping-theorem.md) yields

$$
\boxed{Z=\min\{0,W\}.}
$$

This distribution has probability $1/2$ at zero and a continuous normal half-density on the negative half-line, so it is not normal.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [28J](../../28j.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
