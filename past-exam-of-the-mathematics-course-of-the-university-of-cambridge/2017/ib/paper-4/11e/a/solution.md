<h1 id="11e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [structure theorem for finitely generated modules over a principal ideal domain](../../../../../../structure-theorem-for-finitely-generated-modules-over-a-principal-ideal-domain.md) applies in particular to a [Euclidean domain](../../../../../../euclidean-domain.md) $R$: every [finitely generated module](../../../../../../finitely-generated-module.md) has an [isomorphism](../../../../../../isomorphism.md)

$$
M\cong R^r\oplus R/(d_1)\oplus\cdots\oplus R/(d_k),\qquad d_1\mid d_2\mid\cdots\mid d_k,
$$

with each $d_i$ nonzero and a nonunit. The [rank of a free module](../../../../../../rank-of-a-free-module.md) $r$ and the [invariant factors of a finitely generated module](../../../../../../invariant-factor-of-a-finitely-generated-module.md) $d_i$ are unique up to multiplication by units; empty sums are allowed. This is the classification theorem being used, without a proof of that theorem.

The [rational canonical form](../../../../../../rational-canonical-form.md) theorem states that for a [linear operator](../../../../../../linear-operator.md) $T$ on a finite-dimensional [vector space](../../../../../../vector-space-split.md) over any [field](../../../../../../field.md) $F$, there are unique monic nonconstant [polynomials](../../../../../../polynomial-split.md) $p_1\mid\cdots\mid p_k$ such that some [basis](../../../../../../basis.md) gives

$$
\boxed{[T]=\operatorname{diag}(C(p_1),\ldots,C(p_k))}.
$$

Here, for $p(t)=t^d+a_{d-1}t^{d-1}+\cdots+a_0$, the [companion matrix](../../../../../../companion-matrix.md) has ones on its subdiagonal and last column $(-a_0,\ldots,-a_{d-1})^T$. The empty matrix covers a zero-dimensional space. Two [linear operators](../../../../../../linear-operator.md) have [matrix similarity](../../../../../../matrix-similarity.md) exactly when they have the same [invariant factors of a linear operator](../../../../../../invariant-factors-of-a-linear-operator.md).

For the proof, make $V$ an $F[t]$-[module](../../../../../../module-mathematics.md) by $t\cdot v=T(v)$. It is a [finitely generated module](../../../../../../finitely-generated-module.md), since a vector-space [basis](../../../../../../basis.md) also generates it as a [module](../../../../../../module-mathematics.md). It is a [torsion module](../../../../../../torsion-module.md): the powers of $T$ have [linear dependence](../../../../../../linear-dependence.md) in the finite-dimensional space $\operatorname{End}_F(V)$, so some nonzero [polynomial](../../../../../../polynomial-split.md) annihilates every vector. Because $F[t]$ is a [Euclidean domain](../../../../../../euclidean-domain.md), the classification theorem gives

$$
V\cong\bigoplus_{i=1}^kF[t]/(p_i),\qquad p_1\mid\cdots\mid p_k.
$$

There is no free summand, since a nonzero [free module](../../../../../../free-module.md) over $F[t]$ is not a [torsion module](../../../../../../torsion-module.md). Choose monic generators of the ideals. On $F[t]/(p_i)$, the classes of $1,t,\ldots,t^{d_i-1}$ form an $F$-[basis](../../../../../../basis.md) by [polynomial division](../../../../../../polynomial-division.md). Multiplication by $t$ is exactly $C(p_i)$ in that [basis](../../../../../../basis.md), proving existence. Uniqueness in the classification theorem proves uniqueness of the [rational canonical form](../../../../../../rational-canonical-form.md). Finally, an $F[t]$-[module isomorphism](../../../../../../module-isomorphism.md) is precisely an invertible $F$-[linear map](../../../../../../linear-map.md) intertwining the operators, establishing the assertion about [matrix similarity](../../../../../../matrix-similarity.md). In particular the [characteristic polynomial](../../../../../../characteristic-polynomial.md) is $\prod_i p_i$ and the [minimal polynomial](../../../../../../minimal-polynomial.md) is $p_k$ for nonzero $V$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [11E](../../11e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
