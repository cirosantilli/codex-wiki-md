<h1 id="12h/solution">Solution</h1>

↑ **Parent:** [12H](../12h.md)

The [second fundamental form](../../../../../second-fundamental-form-split.md) records the normal component of second-order bending of the surface. For a surface curve $\gamma(t)=\sigma(u(t),v(t))$, the terms containing $u''$ and $v''$ are tangent and therefore

$$
\gamma''\cdot\boldsymbol N=L(u')^2+2Mu'v'+N(v')^2.
$$

Thus on a unit tangent direction it gives the [normal curvature](../../../../../normal-curvature.md); for a general coordinate direction the [normal curvature](../../../../../normal-curvature.md) is the ratio of the second to the [first fundamental form](../../../../../first-fundamental-form.md). Equivalently the quadratic part of displacement out of the [tangent plane](../../../../../tangent-plane.md) is one half of this form. Reversing the chosen [unit normal](../../../../../unit-normal.md) changes its sign.

Now suppose $L=M=N=0$. Differentiate $\boldsymbol N\cdot\sigma_u=\boldsymbol N\cdot\sigma_v=0$. This gives

$$
\boldsymbol N_u\cdot\sigma_u=-L=0,\quad\boldsymbol N_u\cdot\sigma_v=-M=0,\qquad\boldsymbol N_v\cdot\sigma_u=-M=0,\quad\boldsymbol N_v\cdot\sigma_v=-N=0.
$$

Also differentiation of $\boldsymbol N\cdot\boldsymbol N=1$ gives $\boldsymbol N_u\cdot\boldsymbol N=\boldsymbol N_v\cdot\boldsymbol N=0$. The parametrization is regular, so $\sigma_u,\sigma_v,\boldsymbol N$ form a [basis](../../../../../basis.md) of three-dimensional space. Both normal derivatives are orthogonal to this [basis](../../../../../basis.md) and hence vanish:

$$
\boxed{\boldsymbol N_u=\boldsymbol N_v=0.}
$$

The parameter ball is [connected](../../../../../connected-space.md); integrating these derivatives along a straight segment between parameter points shows that $\boldsymbol N=\boldsymbol N_0$ is constant. Finally both derivatives of $\sigma\cdot\boldsymbol N_0$ vanish, because $\sigma_u,\sigma_v$ are tangent. Thus the [zero second fundamental form implies planar image](../../../../../zero-second-fundamental-form-implies-planar-image.md) statement is

$$
\boxed{U\subset\{\boldsymbol x:\boldsymbol x\cdot\boldsymbol N_0=C\}.}
$$

The PDF has $\boldsymbol N_v$ in the second derivative equality; the apparent $\boldsymbol N_t$ in the TeX is not a distinct coordinate.

## ↑ Ancestors (10)

1. [12H](../12h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
