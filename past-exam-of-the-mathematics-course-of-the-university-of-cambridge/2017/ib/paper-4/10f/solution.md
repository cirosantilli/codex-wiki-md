<h1 id="10f/solution">Solution</h1>

↑ **Parent:** [10F](../10f.md)

The [dual space](../../../../../dual-space.md) here is the algebraic [dual space](../../../../../dual-space.md) $X^*=\operatorname{Hom}_{\mathbb R}(X,\mathbb R)$, consisting of every [linear functional](../../../../../linear-functional.md); no [topology](../../../../../topology-split.md) or boundedness is imposed. For a [basis](../../../../../basis.md) $e_1,\ldots,e_n$, define $e_i^*(\sum_jx_je_j)=x_i$. These are [linear functionals](../../../../../linear-functional.md) satisfying $e_i^*(e_j)=\delta_{ij}$. Evaluating $\sum_i a_ie_i^*=0$ on each $e_j$ gives $a_j=0$, proving [linear independence](../../../../../linear-independence.md). Conversely, for every $T\in X^*$,

$$
T=\sum_{i=1}^nT(e_i)e_i^*.
$$

This proves spanning and hence proves, without assuming a dimension theorem, that the [dual basis](../../../../../dual-basis.md) is a [basis](../../../../../basis.md) and $\dim X^*=n$.

The canonical [bidual evaluation map](../../../../../bidual-evaluation-map.md) is

$$
\boxed{J:X\longrightarrow X^{**},\qquad J(x)(T)=T(x)}.
$$

Its definition makes no choice of [basis](../../../../../basis.md) and it is [linear](../../../../../linearity.md). If $x\ne0$, one coordinate functional is nonzero on $x$, so $J$ is [injective](../../../../../injective-function.md). For any $B\in X^{**}$, choose $x=\sum_iB(e_i^*)e_i$. Expanding $T$ in the [dual basis](../../../../../dual-basis.md) gives $T(x)=\sum_iT(e_i)B(e_i^*)=B(T)$, proving [surjection](../../../../../surjective-function.md) explicitly. Thus $J$ is an [isomorphism](../../../../../isomorphism.md).

If $T_1,\ldots,T_n$ is any [basis](../../../../../basis.md) of $X^*$, its [dual basis](../../../../../dual-basis.md) $B_1,\ldots,B_n$ in $X^{**}$ exists by the result just proved. Put $v_j=J^{-1}(B_j)$. These vectors form a [basis](../../../../../basis.md) of $X$, and $T_i(v_j)=B_j(T_i)=\delta_{ij}$. **Every [basis](../../../../../basis.md) of the finite-dimensional dual is a dual [basis](../../../../../basis.md)**, of a uniquely determined [basis](../../../../../basis.md) of $X$.

For a [separating subspace of an algebraic dual](../../../../../separating-subspace-of-an-algebraic-dual.md) $W$, choose a [basis](../../../../../basis.md) $T_1,\ldots,T_r$ of $W$. The [linear map](../../../../../linear-map.md) $x\mapsto(T_1(x),\ldots,T_r(x))$ is [injective](../../../../../injective-function.md) because $W$ separates nonzero vectors. The [rank-nullity theorem](../../../../../rank-nullity-theorem.md) implies $n\leq r$; but $W\subseteq X^*$ implies $r\leq n$. Hence

$$
\boxed{W=X^*}.
$$

The zero-dimensional case also has this conclusion.

For $X=\mathbb R[x]$, the [monomials](../../../../../monomial.md) $1,x,x^2,\ldots$ form an infinite [basis](../../../../../basis.md), each [polynomial](../../../../../polynomial-split.md) using only finitely many of them. The map $T\mapsto(T(1),T(x),T(x^2),\ldots)$ identifies $X^*$ with all real [sequences](../../../../../sequence.md), because any sequence $(a_j)$ defines $T(\sum_{j=0}^d c_jx^j)=\sum_{j=0}^dc_ja_j$. The [linear subspace](../../../../../vector-subspace.md) of finitely supported sequences is proper (it excludes $(1,1,\ldots)$) and separating (one coefficient functional detects any nonzero [polynomial](../../../../../polynomial-split.md)). Thus

$$
\boxed{\mathbb R^{(\mathbb N_0)}\subsetneq\mathbb R^{\mathbb N_0}\cong X^*\text{ is separating}}.
$$

## ↑ Ancestors (10)

1. [10F](../10f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
