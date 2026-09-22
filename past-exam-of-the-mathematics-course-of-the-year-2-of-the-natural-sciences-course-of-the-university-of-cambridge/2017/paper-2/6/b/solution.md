<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take the centre of the ball as the origin. An orthogonal change of variables leaves both this domain and its volume measure invariant. Consequently its Cartesian moment integrals are [isotropic tensors](../../../../../isotropic-tensor.md). Equivalently, inversion $x\mapsto-x$ immediately makes every odd moment zero.

There is no nonzero invariant rank-one [vector](../../../../../vector.md), so

$$
\boxed{\int_Vx_i\,dV=0.}
$$

An [isotropic tensor](../../../../../isotropic-tensor.md) of rank two is a scalar multiple of the [Kronecker delta](../../../../../kronecker-delta.md), giving $\int_Vx_ix_j\,dV=\alpha\delta_{ij}$. Contract the indices and use [spherical coordinates](../../../../../spherical-coordinate-system.md):

$$
3\alpha=\int_Vr^2\,dV=4\pi\int_0^a r^4\,dr=\frac{4\pi a^5}{5}.
$$

Thus the [Cartesian moments of a three-dimensional ball](../../../../../cartesian-moments-of-a-three-dimensional-ball.md) give

$$
\boxed{\alpha=\frac{4\pi a^5}{15},\qquad\int_Vx_ix_j\,dV=\frac{4\pi a^5}{15}\delta_{ij},\qquad\int_Vx_ix_jx_k\,dV=0.}
$$

For the last identity, one may also use the general rotation-invariant rank-three tensor $c\epsilon_{ijk}$: the moment is fully symmetric in its indices, whereas the [Levi-Civita symbol](../../../../../levi-civita-symbol.md) is antisymmetric, forcing $c=0$.

The origin convention is necessary. For a ball centred at a nonzero vector $c$, its first moment would instead be $(4\pi a^3/3)c_i$, so the displayed claims implicitly refer to coordinates measured from its centre.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
