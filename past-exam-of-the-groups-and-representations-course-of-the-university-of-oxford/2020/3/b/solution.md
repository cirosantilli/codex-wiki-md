<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use upper indices for the defining [representation](../../../../group-representation.md) of [SU(3)](../../../../su-3-group.md) and lower indices for its [dual representation](../../../../dual-representation.md). A [Young diagram](../../../../young-diagram.md) with row lengths $(\ell_1,\ell_2)$ has [highest weight](../../../../highest-weight-of-a-representation.md) [Dynkin labels](../../../../dynkin-label.md) $(p,q)=(\ell_1-\ell_2,\ell_2)$; a full column of height three is a [determinant representation](../../../../determinant-representation.md) and can be removed for [SU(3)](../../../../su-3-group.md). The [Weyl dimension formula](../../../../weyl-dimension-formula.md) reduces to

$$
\dim(p,q)=\frac{(p+1)(q+1)(p+q+2)}{2}.
$$

The six [irreducible representations](../../../../irreducible-representation.md) of smallest [dimensions](../../../../dimension-vector-space.md) are $\mathbf1,\mathbf3,\overline{\mathbf3},\mathbf6,\overline{\mathbf6},\mathbf8$. The following box arrays draw their [Young diagrams](../../../../young-diagram.md); filling boxes by tensor-slot labels gives representative [Young tableaux](../../../../young-tableau.md):

$$
\begin{array}{c|c|c|c|c}
\text{representation}&\text{diagram}&(\ell_1,\ell_2)&(p,q)&\dim\\\hline
\mathbf1&\varnothing&(0,0)&(0,0)&1\\[2pt]
\mathbf3&\boxed{\phantom{i}}&(1,0)&(1,0)&3\\[2pt]
\overline{\mathbf3}&\begin{array}{|c|}\hline\phantom{i}\\\hline\phantom{i}\\\hline\end{array}&(1,1)&(0,1)&3\\[4pt]
\mathbf6&\begin{array}{|c|c|}\hline\phantom{i}&\phantom{i}\\\hline\end{array}&(2,0)&(2,0)&6\\[4pt]
\overline{\mathbf6}&\begin{array}{|c|c|}\hline\phantom{i}&\phantom{i}\\\hline\phantom{i}&\phantom{i}\\\hline\end{array}&(2,2)&(0,2)&6\\[4pt]
\mathbf8&\begin{array}{l}\boxed{\phantom{i}}\boxed{\phantom{i}}\\[-3pt]\boxed{\phantom{i}}\end{array}&(2,1)&(1,1)&8
\end{array}
$$

Their associated [tensors](../../../../tensor.md), in the same order, can be taken as follows:

- $\mathbf1$: a scalar $s$, unchanged by [SU(3)](../../../../su-3-group.md).
- $\mathbf3$: a [vector](../../../../vector.md) $v^i$, with $v^i\mapsto U^i{}_jv^j$.
- $\overline{\mathbf3}$: an [antisymmetric tensor](../../../../antisymmetric-tensor.md) $A^{[ij]}$, equivalently a [covector](../../../../covector.md) $w_k=\tfrac12\epsilon_{kij}A^{ij}$, with $w_i\mapsto w_j(U^{-1})^j{}_i$.
- $\mathbf6$: a [symmetric tensor](../../../../symmetric-tensor.md) $S^{(ij)}$, with $S^{ij}\mapsto U^i{}_kU^j{}_\ell S^{k\ell}$.
- $\overline{\mathbf6}$: a symmetric [covariant tensor](../../../../covariant-tensor.md) $S_{(ij)}$, with $S_{ij}\mapsto S_{k\ell}(U^{-1})^k{}_i(U^{-1})^\ell{}_j$. In the four-upper-index [Young tableau](../../../../young-tableau.md) description, use two antisymmetric index pairs with symmetry under exchange of pairs, and convert each pair to a lower index with the invariant $\epsilon$ [tensor](../../../../tensor.md).
- $\mathbf8$: a mixed [tensor](../../../../tensor.md) $T^i{}_j$ with $T^i{}_i=0$, transforming as $T\mapsto UTU^{-1}$. This is the [Adjoint representation](../../../../adjoint-representation-of-a-lie-algebra.md). Its nine components obey one independent [trace](../../../../matrix-trace.md) constraint.

These [low-dimensional SU3 tensor representations](../../../../low-dimensional-su3-tensor-representations.md) have [dimensions](../../../../dimension-vector-space.md) $1,3,3,6,6,8$ by direct component counting. To check that none were missed, if $p+q\geq3$ then $(p+1)(q+1)\geq p+q+1$, so the displayed [dimension](../../../../dimension-vector-space.md) is at least $(p+q+1)(p+q+2)/2\geq10$. The pairs with $p+q\leq2$ are precisely the six listed pairs.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2020](../../../2020-split.md)
4. [Past exam of the groups and representations course of the University of Oxford](../../../split.md)
5. [Groups and representations course of the University of Oxford](../../../../groups-and-representations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
