<h1 id="1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

A [linear regularization](../../../../../../linear-regularization.md) is a family of [bounded linear operators](../../../../../../continuous-linear-operator.md) $R_\alpha:V\to U$, $\alpha>0$, for which $R_\alpha f\to K^\dagger f$ for every $f\in\mathcal D(K^\dagger)$ as $\alpha\downarrow0$. To obtain a [convergent regularization of an inverse problem](../../../../../../convergent-regularization-of-an-inverse-problem.md) for noisy data, choose a [regularization parameter](../../../../../../regularization-parameter.md) so that the exact-data approximation error and the amplified noise both vanish.

An example is [Tikhonov regularization](../../../../../../tikhonov-regularization.md):

$$
\boxed{R_\alpha=(K^*K+\alpha I)^{-1}K^*.}
$$

The positive quadratic term makes $K^*K+\alpha I$ invertible. The [Tikhonov filter norm bound](../../../../../../tikhonov-filter-norm-bound.md) follows from the filter $s/(s^2+\alpha)$, whose maximum for $s\geq0$ is $1/(2\sqrt\alpha)$. Therefore $\|R_\alpha\|\leq1/(2\sqrt\alpha)$. The spectral factors $s^2/(s^2+\alpha)$ tend to one on the positive spectrum; [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) gives consistency on $\mathcal D(K^\dagger)$. The [noise-bias decomposition for linear regularization](../../../../../../noise-bias-decomposition-for-linear-regularization.md) then proves convergence whenever $\alpha(\delta)\to0$ and $\delta/\sqrt{\alpha(\delta)}\to0$, for example $\alpha(\delta)=\delta$ for sufficiently small positive noise levels.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [1](../../1.md)
3. [Paper 326](../../../paper-326-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
