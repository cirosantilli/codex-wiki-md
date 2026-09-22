<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Cameron-Martin space of a Gaussian measure](../../../../../../cameron-martin-space-of-a-gaussian-measure.md) $\mu=\mathcal N(0,\Sigma)$ is

$$
\boxed{E=\operatorname{Ran}\Sigma^{1/2},\qquad
\langle h,g\rangle_E=\langle\Sigma^{-1/2}h,\Sigma^{-1/2}g\rangle_{\mathcal H}.}
$$

The inverse is defined on the range of $\Sigma^{1/2}$. In this infinite-dimensional setting “positive definite” must mean $\langle\Sigma h,h\rangle>0$ for every nonzero $h$, rather than a uniform lower bound: a [trace-class operator](../../../../../../trace-class-operator.md) cannot be uniformly positive on an infinite-dimensional [Hilbert space](../../../../../../hilbert-space-split.md).

By the [spectral theorem for compact Hermitian operators](../../../../../../spectral-theorem-for-compact-hermitian-operators.md), choose an [orthonormal basis](../../../../../../orthonormal-basis.md) $(e_j)$ with $\Sigma e_j=\lambda_je_j$, $\lambda_j>0$, and $\sum_j\lambda_j<\infty$. (A strictly positive [trace-class operator](../../../../../../trace-class-operator.md) also forces the ambient [Hilbert space](../../../../../../hilbert-space-split.md) to be separable.) In coordinates $h_j=\langle h,e_j\rangle$,

$$
E=\left\{h\in\mathcal H:\sum_j\frac{h_j^2}{\lambda_j}<\infty\right\},\qquad
\|h\|_E^2=\sum_j\frac{h_j^2}{\lambda_j}.
$$

This is a [Hilbert space](../../../../../../hilbert-space-split.md) with its indicated norm, even though its range need not be closed in the ambient norm.

The [Cameron-Martin theorem for a Gaussian measure](../../../../../../cameron-martin-theorem-for-a-gaussian-measure.md) states that the translated law $\mu_h(B)=\mu(B-h)=\mathcal N(h,\Sigma)(B)$ is an [equivalent probability measure](../../../../../../equivalent-probability-measure.md) to $\mu$ exactly when $h\in E$. For such $h$, its [Radon-Nikodym derivative](../../../../../../radon-nikodym-derivative.md) is

$$
\boxed{\frac{d\mu_h}{d\mu}(x)=\exp\left(\ell_h(x)-\tfrac12\|h\|_E^2\right),\qquad
\ell_h(x)=\lim_{N\to\infty}\sum_{j=1}^N\frac{h_jx_j}{\lambda_j}.}
$$

The series has [mean-square convergence](../../../../../../convergence-in-l2.md) and converges [almost surely](../../../../../../almost-sure-convergence.md) under $\mu$, since its independent summands have total [variance](../../../../../../variance-split.md) $\sum_jh_j^2/\lambda_j$. Its law is $\mathcal N(0,\|h\|_E^2)$, so the density has [expected value](../../../../../../expected-value.md) one. It is sometimes formally written $\ell_h(x)=\langle h,x\rangle_E$, but a typical infinite-dimensional Gaussian sample is not in $E$; the series interpretation is essential. If $h\notin E$, the two laws are [mutually singular measures](../../../../../../mutually-singular-measures.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 350](../../../paper-350-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
