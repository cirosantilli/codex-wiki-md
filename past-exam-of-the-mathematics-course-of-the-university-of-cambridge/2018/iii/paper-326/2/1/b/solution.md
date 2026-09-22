<h1 id="2/1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Suppose each $R_\alpha:\mathcal V\to\mathcal U$ is a [bounded linear operator](../../../../../../../continuous-linear-operator.md) and $R_\alpha f\to K^\dagger f$ for every $f\in\mathcal D(K^\dagger)$ as $\alpha\downarrow0$. A standard sufficient [a priori regularization parameter choice](../../../../../../../a-priori-regularization-parameter-choice.md) satisfies

$$
\boxed{\alpha(\delta)\longrightarrow0,\qquad
\delta\|R_{\alpha(\delta)}\|\longrightarrow0\quad(\delta\downarrow0).}
$$

For every datum with $\|f^\delta-f\|\leq\delta$, the [noise-bias decomposition for linear regularization](../../../../../../../noise-bias-decomposition-for-linear-regularization.md) gives

$$
\|R_{\alpha(\delta)}f^\delta-K^\dagger f\|
\leq\delta\|R_{\alpha(\delta)}\|
+\|R_{\alpha(\delta)}f-K^\dagger f\|\longrightarrow0.
$$

Thus **the parameter rule gives a [convergent regularization of an inverse problem](../../../../../../../convergent-regularization-of-an-inverse-problem.md)**, uniformly over data in the prescribed noise ball for each fixed admissible exact datum. For [Tikhonov regularization](../../../../../../../tikhonov-regularization.md), $\|R_\alpha\|\leq1/(2\sqrt\alpha)$, so $\alpha\to0$ and $\delta/\sqrt\alpha\to0$ suffice. The same sufficient noise scaling holds for [spectral cutoff regularization](../../../../../../../truncated-singular-value-decomposition.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2](../../../2.md)
4. [Paper 326](../../../../paper-326-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
