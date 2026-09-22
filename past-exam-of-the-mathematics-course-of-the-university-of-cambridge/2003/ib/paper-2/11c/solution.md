<h1 id="11c/solution">Solution</h1>

↑ **Parent:** [11C](../11c.md)

For an orthogonal change of Cartesian coordinates $x'_i=Q_{ij}x_j$, an ordinary [rank](../../../../../rank-one-quadratic-form.md)-$n$ [tensor](../../../../../tensor.md) transforms by

$$
\boxed{T'_{i_1\cdots i_n}=Q_{i_1j_1}\cdots Q_{i_nj_n}T_{j_1\cdots j_n}.}
$$

An [isotropic tensor](../../../../../isotropic-tensor.md) is invariant under such rotations. Orthogonality gives $Q_{ip}Q_{jq}\delta_{pq}=\delta_{ij}$, so transforming any of the three products of two [Kronecker deltas](../../../../../kronecker-delta.md) leaves it unchanged. Their linear combination with arbitrary scalar [coefficients](../../../../../coefficient.md) is therefore isotropic.

For completeness, these three products exhaust the [rank](../../../../../rank-one-quadratic-form.md)-four isotropic [tensors](../../../../../tensor.md) in three dimensions. Half-turns about coordinate axes force a nonzero component to contain each coordinate label an even number of times. Axis interchanges then leave just the values $X=c_{1111}$, $\alpha=c_{1122}$, $\beta=c_{1212}$ and $\gamma=c_{1221}$. Rotating the first two axes by $\pi/4$ gives $X=\tfrac12X+\tfrac12(\alpha+\beta+\gamma)$, so $X=\alpha+\beta+\gamma$. These component values are exactly those of the three-delta-product expression. Thus isotropy of the elastic medium gives this form for its elasticity [tensor](../../../../../tensor.md).

Contracting with the symmetric strain gives

$$
\sigma_{ij}=\alpha e_{kk}\delta_{ij}+\beta e_{ij}+\gamma e_{ji}
=\lambda e_{kk}\delta_{ij}+2\mu e_{ij},\qquad
\boxed{\lambda=\alpha,\quad2\mu=\beta+\gamma.}
$$

These are the [Lamé parameters](../../../../../lame-parameter.md). Taking the [trace](../../../../../matrix-trace.md) determines the scalar part of the strain:

$$
\boxed{p=\frac13e_{kk},\qquad d_{ij}=e_{ij}-p\delta_{ij},\qquad d_{ii}=0.}
$$

Since $\sum_{ij}e_{ij}^2=3p^2+\sum_{ij}d_{ij}^2$, the stored [strain energy density](../../../../../strain-energy-density.md) is

$$
E=\frac\lambda2(e_{kk})^2+\mu e_{ij}e_{ij}
=\frac32(3\lambda+2\mu)p^2+\mu\sum_{ij}d_{ij}^2.
$$

A nonzero traceless test strain proves necessity of $\mu\ge0$, and a pure scalar strain proves necessity of $3\lambda+2\mu\ge0$. Conversely these two conditions make both terms nonnegative for every strain. Thus [nonnegative isotropic elastic strain energy](../../../../../nonnegative-isotropic-elastic-strain-energy.md) is equivalent to

$$
\boxed{\mu\ge0,\qquad\lambda\ge-\frac23\mu.}
$$

## ↑ Ancestors (10)

1. [11C](../11c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
