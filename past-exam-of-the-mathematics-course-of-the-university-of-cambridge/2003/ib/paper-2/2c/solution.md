<h1 id="2c/solution">Solution</h1>

↑ **Parent:** [2C](../2c.md)

Let $M_{ij}=\int_Sx_ix_j\,dS$. A [rotation matrix](../../../../../rotation-matrix.md) $Q$ maps the unit sphere and its surface measure to themselves. Changing variables therefore gives $Q_{ip}Q_{jq}M_{pq}=M_{ij}$, so $M$ is an [isotropic second-rank tensor](../../../../../isotropic-second-rank-tensor.md). Reflection symmetry also directly makes its off-diagonal entries zero, while interchange of coordinates makes its three diagonal entries equal. Its [trace](../../../../../matrix-trace.md) is

$$
\sum_i M_{ii}=\int_S|x|^2\,dS=4\pi,
$$

hence $M_{ij}=(4\pi/3)\delta_{ij}$. Oddness gives $\int_Sx_i\,dS=0$. Expanding the defining product for $T$ now gives

$$
\boxed{T_{ij}(y)=\frac{4\pi}{3}\delta_{ij}+4\pi y_iy_j,
\qquad\lambda=\frac{4\pi}{3},\quad\mu=4\pi.}
$$

The action on a vector is $Tv=\lambda v+\mu y(y\cdot v)$. For $y\ne0$, its [eigenvalues](../../../../../eigenvalue.md) and [eigenspaces](../../../../../eigenspace.md) are therefore

$$
\boxed{\frac{4\pi}{3}+4\pi|y|^2\text{ on }\operatorname{span}\{y\},
\qquad\frac{4\pi}{3}\text{ on }y^\perp.}
$$

The latter has multiplicity two. If $y=0$, the single [eigenvalue](../../../../../eigenvalue.md) $4\pi/3$ has multiplicity three and every vector is an [eigenvector](../../../../../eigenvector.md) apart from the excluded zero vector.

## ↑ Ancestors (10)

1. [2C](../2c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
