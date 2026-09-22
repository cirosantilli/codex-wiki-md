<h1 id="18g/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Clebsch-Gordan decomposition for SU2](../../../../../../clebsch-gordan-decomposition-for-su2.md) states

$$
\boxed{V_m\otimes V_n\cong\bigoplus_{r=0}^{\min(m,n)}V_{m+n-2r}.}
$$

Realize the [tensor product](../../../../../../tensor-product.md) as [polynomials](../../../../../../polynomial-split.md) of bidegree $(m,n)$ in $(x_1,y_1)$ and $(x_2,y_2)$. The [determinant](../../../../../../determinant.md) $D=x_1y_2-y_1x_2$ is invariant under the simultaneous SU2 action. For each $r$, the vector

$$
v_r=D^r x_1^{m-r}x_2^{n-r}
$$

has [torus](../../../../../../torus.md) weight $q=m+n-2r$ and is killed by $E=x_1\partial_{y_1}+x_2\partial_{y_2}$. Applying $F=y_1\partial_{x_1}+y_2\partial_{x_2}$ produces $q+1$ nonzero vectors of distinct weights, with $F^{q+1}v_r=0$. The relations $[E,F]=H$ and $H v_r=qv_r$ give $E F^jv_r=j(q-j+1)F^{j-1}v_r$, so their span is an irreducible copy of $V_q$.

These irreducible submodules have distinct [highest weights](../../../../../../highest-weight-of-a-representation.md) and form a [direct sum](../../../../../../direct-sum.md): a sum of earlier ones cannot contain an [irreducible module](../../../../../../irreducible-module.md) inequivalent to all its summands. Equivalently use complete reducibility, obtained by averaging an [inner product](../../../../../../inner-product.md) over the compact group. Assuming $m\leq n$, their total dimension is

$$
\sum_{r=0}^m(m+n-2r+1)=(m+1)(n+1),
$$

which equals the dimension of the [tensor product](../../../../../../tensor-product.md). Hence they exhaust it, proving the theorem.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [18G](../../18g.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
