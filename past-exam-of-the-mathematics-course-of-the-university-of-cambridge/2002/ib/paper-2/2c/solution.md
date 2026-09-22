<h1 id="2c/solution">Solution</h1>

↑ **Parent:** [2C](../2c.md)

Let $R_{ij}$ be the components of an [orthogonal matrix](../../../../../orthogonal-matrix.md) relating two Cartesian frames by $v'_i=R_{ij}v_j$. Repeated indices are summed from $1$ to $3$. The [tensor component transformation law](../../../../../tensor-component-transformation-law.md) for a [Cartesian second-rank tensor](../../../../../cartesian-second-rank-tensor.md) is

$$
\boxed{A'_{ij}=R_{ik}R_{j\ell}A_{k\ell}},\qquad A'=RAR^{\mathsf T}.
$$

For a proper [rotation](../../../../../rotation-mathematics.md), $\det R=1$; the transformation law itself also holds for orthogonal changes of Cartesian frame with determinant $-1$.

To find a [cubically invariant second-rank tensor](../../../../../cubically-invariant-second-rank-tensor.md), first square each of the prescribed quarter-turns. For example the half-turn about the first axis is $S_x=\operatorname{diag}(1,-1,-1)$. Invariance under $S_xAS_x^{\mathsf T}$ forces $A_{12},A_{13},A_{21},A_{31}$ to vanish. The corresponding half-turns about the other axes eliminate the remaining off-diagonal components, even though symmetry of $A$ was never assumed.

Now write $A=\operatorname{diag}(a,b,c)$. A quarter-turn about the third axis interchanges $a,b$, so $a=b$; a quarter-turn about the first axis gives $b=c$. Conversely a scalar multiple of the [identity matrix](../../../../../identity-matrix.md) is invariant under every [rotation](../../../../../rotation-mathematics.md). Thus the most general answer is

$$
\boxed{A_{ij}=a\delta_{ij}}.
$$

## ↑ Ancestors (10)

1. [2C](../2c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
