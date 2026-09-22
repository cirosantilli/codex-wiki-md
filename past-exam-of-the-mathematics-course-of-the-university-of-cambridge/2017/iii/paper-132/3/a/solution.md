<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A generalized [conformal metric](../../../../../../conformal-metric.md) is locally $ds_\rho=\rho(z)|dz|$, where $\rho$ is nonnegative and measurable and transforms as a length density under a [holomorphic](../../../../../../complex-differentiability-at-a-point.md) change of coordinate. Its area is $A_\rho=\int_X\rho^2\,dx\,dy$. Use the usual convention of using [locally rectifiable paths](../../../../../../locally-rectifiable-path.md) for a [path family](../../../../../../path-family.md) $\Gamma$, and put $L_\rho(\Gamma)=\inf_{\gamma\in\Gamma}\int_\gamma\rho|dz|$. Then

$$
\boxed{\lambda(\Gamma,X)=\sup_{\rho:\ 0<A_\rho<\infty}
\frac{L_\rho(\Gamma)^2}{A_\rho}.}
$$

This is [extremal length](../../../../../../extremal-length.md). Zeros and isolated singularities of an admissible density are allowed; requiring a [smooth](../../../../../../smooth-function.md) strictly positive [Riemannian metric](../../../../../../riemannian-metric.md) would unnecessarily restrict the definition. Line integrals have their extended nonnegative values; if an arbitrary family is supplied, use its members that are [locally rectifiable paths](../../../../../../locally-rectifiable-path.md). An empty [path family](../../../../../../path-family.md) has infinite infimal length, whereas a family containing a constant path has [extremal length](../../../../../../extremal-length.md) zero.

Both numerator and denominator scale quadratically when $\rho$ is multiplied by a positive constant. The coordinate transformation of the area element makes the quotient unchanged under [conformal equivalence](../../../../../../conformal-equivalence.md).

The normalization relevant later is worth deriving. On the [conformal cylinder](../../../../../../conformal-cylinder.md) $(\mathbb R/\mathbb Z)\times(0,M)$, let $\Gamma$ contain the loops going once around it. For the horizontal loop at height $t$, [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) gives

$$
\left(\int_0^1\rho(x,t)\,dx\right)^2\leq\int_0^1\rho(x,t)^2\,dx.
$$

Integrating in $t$ shows $L_\rho(\Gamma)^2\leq A_\rho/M$. The constant density achieves equality, since every winding-one loop has Euclidean length at least one. Hence

$$
\boxed{\lambda(\Gamma,\text{cylinder})=\frac1M.}
$$

Here $M$ is the height divided by circumference, the [conformal modulus of an annulus](../../../../../../conformal-modulus-of-an-annulus.md); the reciprocal is used for the family joining its boundary components.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 132](../../../paper-132-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
