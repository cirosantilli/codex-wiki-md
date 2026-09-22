<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

On $I=g(\mathbb R)$ define $h(y)=g'(g^{-1}(y))$. Differentiation gives

$$
\boxed{h'(y)=\frac{g''(g^{-1}(y))}{g'(g^{-1}(y))}
=-2b(g^{-1}(y)),\qquad |h'(y)|\leq2B.}
$$

The mean value theorem proves [Lipschitz continuity](../../../../../../lipschitz-continuity.md) of $h$ on $I$, with constant $2B$.

If an endpoint of $I$ is finite, the Lipschitz bound gives a finite limiting value of $h$ there. That value must be zero. Otherwise $h$ would be bounded below by a positive number near the endpoint, and

$$
\frac{d}{dy}g^{-1}(y)=\frac1{h(y)}
$$

would make $g^{-1}$ approach a finite limit, contradicting its tending to $+\infty$ or $-\infty$. The [zero extension of a scale diffusion coefficient at finite endpoints](../../../../../../zero-extension-of-a-scale-diffusion-coefficient-at-finite-endpoints.md) therefore gives a globally Lipschitz function $\bar h$ on $\mathbb R$: set it to zero beyond each finite endpoint and retain $h$ on $I$.

Use the following standard [global existence theorem for stochastic differential equations with Lipschitz coefficients](../../../../../../global-existence-theorem-for-stochastic-differential-equations-with-lipschitz-coefficients.md): globally Lipschitz drift and diffusion coefficients give a nonexplosive, pathwise unique [strong stochastic solution](../../../../../../strong-solution-of-a-stochastic-differential-equation.md) for every prescribed initial state and driving [Brownian motion](../../../../../../brownian-motion-split.md). Global Lipschitz continuity also gives the required linear-growth bound. Apply it to

$$
dY_t=\bar h(Y_t)\,dW_t,\qquad Y_0=g(x).
$$

It remains to check that $Y$ stays in $I$, so the inverse transform is defined.

Before the first boundary time, put $X=g^{-1}(Y)$. Since $(g^{-1})'=1/h$ and $(g^{-1})''=-h'/h^2$, the [Itô formula](../../../../../../ito-s-lemma.md), stopped inside compact subintervals of $I$, yields

$$
dX_t=dW_t-\frac12h'(Y_t)\,dt=dW_t+b(X_t)\,dt.
$$

For each finite $T$, up to that boundary time,

$$
|X_t|\leq|x|+\sup_{s\leq T}|W_s|+BT,\qquad t\leq T.
$$

A finite endpoint of $I$ would require $X$ to diverge, which this bound excludes. Therefore $Y$ stays in $I$ at every finite time, and $X=g^{-1}(Y)$ is a global [strong stochastic solution](../../../../../../strong-solution-of-a-stochastic-differential-equation.md).

Finally, any two solutions driven by the same $W$ transform into solutions of the globally Lipschitz $Y$ equation. Its [pathwise uniqueness](../../../../../../pathwise-uniqueness.md) makes the transforms, and hence their inverses, indistinguishable. Thus

$$
\boxed{X=g^{-1}(Y)\text{ exists globally and is pathwise unique}.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
