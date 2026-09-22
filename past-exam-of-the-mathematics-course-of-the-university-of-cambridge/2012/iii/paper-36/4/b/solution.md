<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Vary only the [probability density function](../../../../../../probability-density-function.md) of $X$, using $\eta_t=\eta(1+tb)$ with bounded $b$ and $E_\eta b(X)=0$. The nuisance [score function](../../../../../../informant-function.md) is $b(X)$, giving the [statistical tangent set](../../../../../../statistical-tangent-set.md)

$$
\{b(X):\ b\text{ bounded and measurable},\ E_\eta b(X)=0\}.
$$

Its closed linear span is the [nuisance tangent space](../../../../../../nuisance-tangent-space.md) of all centered $L^2(\eta)$ [functions](../../../../../../function-split.md) of $X$, by [density of bounded centered scores](../../../../../../density-of-bounded-centered-scores.md).

The [conditional expectation](../../../../../../conditional-expectation.md) of the parametric [score function](../../../../../../informant-function.md) given $X$ is zero:

$$
E\left[\frac{h_\theta(X)\varepsilon}{\sigma^2}\,\middle|\,X\right]=0.
$$

It is therefore orthogonal to this [nuisance tangent space](../../../../../../nuisance-tangent-space.md). Its [orthogonal projection](../../../../../../orthogonal-projection.md) onto that space vanishes, so the [efficient score](../../../../../../efficient-score.md) is unchanged. By [independence](../../../../../../independent-random-variables.md) and $E\varepsilon^2=\sigma^2$,

$$
\boxed{\widetilde\ell_{\theta,\eta}=\frac{h_\theta(X)\varepsilon}{\sigma^2},\qquad
\widetilde I_{\theta,\eta}=\frac{E_\eta h_\theta(X)^2}{\sigma^2}.}
$$

These equal the parametric [score function](../../../../../../informant-function.md) and [Fisher information](../../../../../../fisher-information-matrix.md) when $\eta$ is known. **There is no loss of information from the unknown covariate density.** This is [adaptivity to an unknown covariate distribution](../../../../../../adaptivity-to-an-unknown-covariate-distribution.md); it follows from score orthogonality, without having to estimate the [nuisance parameter](../../../../../../nuisance-parameter.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
