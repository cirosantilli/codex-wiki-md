<h1 id="13/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

On the circular arc, $z=0$ and $dz=0$, so the [line integral](../../../../../../line-integral.md) reduces to

$$
\int(x^2\,dx+y^2\,dy)
=\left[\frac{x^3+y^3}{3}\right]_{(0,0)}^{(1,1)}=\frac23.
$$

This [exact differential](../../../../../../exact-differential.md) evaluation applies to the specified arc; for example its [parametric equation](../../../../../../parametric-equation.md) is $(x,y,z)=(1-\cos\theta,\sin\theta,0)$, $0\leq\theta\leq\pi/2$. On the vertical segment $x=y=1$, only $dz$ contributes, giving $\int_0^1(\lambda+1)\,dz=\lambda+1$. The whole path therefore gives

$$
\boxed{\lambda+\frac53}.
$$

To answer the final conservativeness requirement, compute the [curl](../../../../../../curl.md):

$$
\nabla\times\mathbf M=((2-\mu)y,\ (1-2\lambda)x,\ 0)^T.
$$

It vanishes identically exactly when

$$
\boxed{\mu=2,\qquad\lambda=\frac12}.
$$

On the [simply connected](../../../../../../simply-connected-space.md) whole space this condition is sufficient for a [conservative vector field](../../../../../../conservative-vector-field.md). Explicitly a [vector-field potential](../../../../../../potential-of-a-conservative-vector-field.md) is

$$
\phi=\frac12x^2z+y^2z+\frac{x^3+y^3}{3}+C.
$$

Both path calculations then give $13/6$, equal to $\phi(1,1,1)-\phi(0,0,0)$ by the [fundamental theorem for line integrals](../../../../../../fundamental-theorem-for-line-integrals.md). Equality of just these two path values would only force $\mu=2\lambda+1$; it is the [curl](../../../../../../curl.md) calculation that establishes full [path independence](../../../../../../path-independence.md).

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [13](../../../13.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
