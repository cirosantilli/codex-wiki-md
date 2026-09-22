<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a [harmonic function](../../../../../../harmonic-function.md) $u$, let

$$
M(r)=\frac1{|\partial B_r|}\int_{\partial B_r(x)}u.
$$

The [divergence theorem](../../../../../../divergence-theorem.md) gives

$$
M'(r)=\frac1{|\partial B_r|}\int_{\partial B_r(x)}\partial_\nu u
=\frac1{|\partial B_r|}\int_{B_r(x)}\Delta u=0.
$$

Since $M(r)\to u(x)$ as $r\downarrow0$, $M(r)=u(x)$. Integrating the spherical averages in the radial variable gives the corresponding ball average, proving the [mean value property for harmonic functions](../../../../../../mean-value-property-for-harmonic-functions.md). If $u$ attains its maximum at an interior point, the average of the nonnegative function $\max u-u$ on every sufficiently small centred sphere is zero. [Continuity](../../../../../../continuous-function.md) makes $u$ constant on those spheres, and [connectedness](../../../../../../connected-space.md) propagates that value through the domain. Thus the [weak maximum principle for elliptic operators](../../../../../../weak-maximum-principle-for-elliptic-operators.md) gives

$$
\min_{\partial\Omega}u\leq u\leq\max_{\partial\Omega}u.
$$

For the derivative estimate, choose $r>0$ smaller than half the [distance](../../../../../../distance-to-a-set.md) from $\Omega'$ to $\partial\Omega$, and let $\rho_r$ be a smooth radial [mollifier](../../../../../../mollifier.md) supported in $B_r(0)$. Writing its convolution in polar coordinates and using the spherical mean value property shows that $u*\rho_r=u$ on $\Omega'$. Hence, for every [multi-index](../../../../../../multi-index-notation.md) $\alpha$,

$$
D^\alpha u(x)=\int_\Omega D^\alpha\rho_r(x-y)u(y)\,dy,
$$

so [Holder inequality](../../../../../../holder-inequality.md) gives

$$
\boxed{\|D^\alpha u\|_{L^\infty(\Omega')}
\leq\|D^\alpha\rho_r\|_\infty\|u\|_{L^1(\Omega)}
\leq C(n,\alpha,\Omega,\Omega')\|u\|_{L^1(\Omega)}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
