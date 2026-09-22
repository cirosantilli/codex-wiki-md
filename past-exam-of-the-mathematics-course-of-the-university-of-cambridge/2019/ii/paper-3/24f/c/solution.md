<h1 id="24f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let

$$
\omega=\frac{dx}{y^2}.
$$

At a finite ramification point $P_\alpha=(\alpha,0)$, the uniformizer $t=y$ from part b satisfies $x-\alpha=c_\alpha t^3+O(t^6)$. Consequently

$$
\nu_{P_\alpha}(dx)=2,
\qquad
\nu_{P_\alpha}(y^2)=2,
\qquad
\nu_{P_\alpha}(\omega)=0.
$$

At every other affine point, $x-x(p)$ is a uniformizer and $y$ is a unit, so again $\nu_p(\omega)=0$.

At $P_\infty$, take the uniformizer $t=u=X/Y$ used above. Since $v=Z/Y=t^4$ times a local unit,

$$
x=\frac uv=t^{-3}\mathbin{\cdot}(\text{local unit}),
\qquad
y=\frac1v=t^{-4}\mathbin{\cdot}(\text{local unit}).
$$

It follows that $\nu_{P_\infty}(dx)=-4$ and $\nu_{P_\infty}(y^2)=-8$, so the [valuation of a rational differential](../../../../../../valuation-of-a-rational-differential.md) is

$$
\nu_{P_\infty}(\omega)=4.
$$

Thus

$$
\boxed{(\omega)=4P_\infty,}
$$

whose degree four agrees with $2g_X-2$. For the resulting [canonical divisor](../../../../../../canonical-divisor.md) $K_X=4P_\infty$, the functions $1,x,y$ have pole orders $0,3,4$ at $P_\infty$ and no other poles. They therefore belong to the [canonical Riemann-Roch space](../../../../../../canonical-riemann-roch-space.md). Since $\ell(K_X)=g_X=3$, they form a basis:

$$
\boxed{L(K_X)=\operatorname{span}_{\mathbb C}\{1,x,y\}.}
$$

Equivalently, multiplying by $\omega$ gives the basis

$$
\boxed{\left\{
\frac{dx}{y^2},
\frac{x\,dx}{y^2},
\frac{dx}{y}
\right\}}
$$

of [holomorphic differential forms](../../../../../../holomorphic-differential-form.md), also matching the general description of [holomorphic differentials on a smooth plane curve](../../../../../../holomorphic-differentials-on-a-smooth-plane-curve.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [24F](../../24f.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
