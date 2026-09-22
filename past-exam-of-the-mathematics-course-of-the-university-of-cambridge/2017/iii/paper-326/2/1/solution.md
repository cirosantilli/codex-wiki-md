<h1 id="2/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [regularization of an inverse problem](../../../../../../regularization-of-an-inverse-problem.md) is a family of continuous maps $R_\alpha:V\to U$, $\alpha>0$, such that $R_\alpha f\to K^\dagger f$ for each $f\in\mathcal D(K^\dagger)$ as $\alpha\downarrow0$. A [linear regularization](../../../../../../linear-regularization.md) requires each $R_\alpha$ to be a [bounded linear operator](../../../../../../continuous-linear-operator.md).

A [regularization parameter choice](../../../../../../regularization-parameter-choice.md) assigns $\alpha=\alpha(\delta,f^\delta)>0$ from the noise bound and possibly the measured data. A [convergent regularization of an inverse problem](../../../../../../convergent-regularization-of-an-inverse-problem.md) satisfies, for every fixed admissible exact datum,

$$
\boxed{\sup_{\|g-f\|\leq\delta}\|R_{\alpha(\delta,g)}g-K^\dagger f\|\longrightarrow0\quad(\delta\downarrow0).}
$$

In the usual definition the chosen parameter also tends to zero uniformly over this noise ball. For a linear regularization with exact-data consistency, the conditions $\alpha(\delta)\to0$ and $\delta\|R_{\alpha(\delta)}\|\to0$ are sufficient.

For example, [Tikhonov regularization](../../../../../../tikhonov-regularization.md) with identity penalty has $R_\alpha=(K^*K+\alpha I)^{-1}K^*$ and $\|R_\alpha\|\leq1/(2\sqrt\alpha)$. Its spectral filter converges to the [Moore–Penrose inverse of an operator](../../../../../../moore-penrose-inverse-of-an-operator.md) on its domain. Taking $\alpha(\delta)=\delta$ for small positive noise levels gives both required limits.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [2](../../2.md)
3. [Paper 326](../../../paper-326-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
