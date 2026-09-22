<h1 id="4c/solution">Solution</h1>

↑ **Parent:** [4C](../4c.md)

A [Cartesian second-rank tensor](../../../../../cartesian-second-rank-tensor.md) is an [isotropic tensor](../../../../../isotropic-tensor.md) if its components are unchanged under every proper [rotation matrix](../../../../../rotation-matrix.md) $R$:

$$
T_{ij}=R_{ik}R_{j\ell}T_{k\ell},\qquad\text{or equivalently }T=RTR^T.
$$

The [Kronecker delta](../../../../../kronecker-delta.md) is isotropic because $R_{ik}R_{jk}=\delta_{ij}$, the orthogonality relation $RR^T=I$.

No symmetry of $T$ needs to be assumed. A half-turn about the first axis has matrix $\operatorname{diag}(1,-1,-1)$; invariance under it forces $T_{12},T_{13},T_{21},T_{31}$ to vanish. A half-turn about the second axis additionally kills $T_{23}$ and $T_{32}$. Thus $T=\operatorname{diag}(d_1,d_2,d_3)$. Each half-turn is the square of an allowed quarter-turn. A quarter-turn about the third axis interchanges $d_1,d_2$, so they are equal. A quarter-turn about the second axis interchanges $d_1,d_3$, so all three are equal. Consequently the complete family of [isotropic second-rank tensors](../../../../../isotropic-second-rank-tensor.md) is

$$
\boxed{T_{ij}=\lambda\delta_{ij},\qquad\lambda\in\mathbb R.}
$$

Conversely, every member of this family is invariant because $R(\lambda I)R^T=\lambda I$.

## ↑ Ancestors (10)

1. [4C](../4c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
