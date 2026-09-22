<h1 id="4a/solution">Solution</h1>

↑ **Parent:** [4A](../4a.md)

The [divergence theorem](../../../../../divergence-theorem.md) states that, for a bounded region $V$ with piecewise smooth boundary $S$, outward unit [normal vector](../../../../../normal-vector.md) $n$, and a continuously differentiable [vector field](../../../../../vector-field.md) $F$ on a neighborhood of $\overline V$,

$$
\int_S F\cdot n\,dS=\int_V\nabla\cdot F\,dV.
$$

The outward orientation fixes the sign of the [flux](../../../../../flux.md).

On the [sphere](../../../../../sphere.md) of radius $R$, the outward unit [normal vector](../../../../../normal-vector.md) is $\mathbf r/R$. Thus $r^n\mathbf r\cdot n=R^{n+1}$. Multiplying by the [surface area](../../../../../surface-area.md) $4\pi R^2$ gives

$$
\boxed{I=4\pi R^{n+3}.}
$$

For the second calculation, use the [product rule](../../../../../product-rule.md) in [Cartesian coordinates](../../../../../cartesian-coordinate-system.md):

$$
\nabla\cdot(r^n\mathbf r)=3r^n+\mathbf r\cdot\nabla r^n=(n+3)r^n\qquad(r>0).
$$

The field remains continuously differentiable at the origin when $n>0$. Indeed, for $r>0$ its [Jacobian matrix](../../../../../jacobian-matrix.md) entries are $r^n\delta_{ij}+nr^{n-2}x_ix_j$, all tending to zero as $r\to0$; its derivative at zero is also zero because $|r^n\mathbf r|/r=r^n\to0$. The [divergence theorem](../../../../../divergence-theorem.md) therefore applies to the entire ball. In [spherical coordinates](../../../../../spherical-coordinate-system.md), it yields

$$
I=4\pi(n+3)\int_0^R r^{n+2}\,dr=4\pi R^{n+3},
$$

in agreement with the direct [surface integral](../../../../../surface-integral.md).

## ↑ Ancestors (10)

1. [4A](../4a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
