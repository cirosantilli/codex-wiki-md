<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

On $T=V^{\otimes n}$, define the [permutation](../../../../../permutation.md) and diagonal actions by

$$
\sigma(v_1\otimes\cdots\otimes v_n)
=v_{\sigma^{-1}(1)}\otimes\cdots\otimes v_{\sigma^{-1}(n)},\qquad
g(v_1\otimes\cdots\otimes v_n)=gv_1\otimes\cdots\otimes gv_n.
$$

The inverse in the first formula gives a left action. Applying $g$ to every tensor factor and then reordering produces the same tensor as reordering and then applying $g$. Thus the two actions commute. The [Schur algebra](../../../../../schur-algebra.md) is

$$
\boxed{S_{\mathbb C}(m,n)=\operatorname{End}_{\mathbb CS_n}(T).}
$$

It is the [commutant of an operator algebra](../../../../../commutant-of-an-operator-algebra.md) of the [permutation](../../../../../permutation.md) action.

To identify this commutant, use the multilinear isomorphism

$$
\operatorname{End}(T)\cong\operatorname{End}(V)^{\otimes n}.
$$

Conjugation by a [permutation](../../../../../permutation.md) reorders the factors on the right. Therefore the invariant subspace is the space of [symmetric tensors](../../../../../symmetric-tensor.md) of degree $n$ in $\operatorname{End}(V)$. It is spanned by $a^{\otimes n}$. Indeed, the polarization identity

$$
\sum_{J\subseteq\{1,\ldots,n\}}(-1)^{n-|J|}
\left(\sum_{j\in J}a_j\right)^{\otimes n}
=\sum_{\sigma\in S_n}a_{\sigma(1)}\otimes\cdots\otimes a_{\sigma(n)}
$$

expresses every symmetrized elementary tensor as a [linear combination](../../../../../linear-combination.md) of pure powers. Those symmetrized elementary tensors span the invariant subspace in [characteristic zero](../../../../../characteristic-zero.md).

One may restrict $a$ to invertible [endomorphisms](../../../../../endomorphism.md) without changing the span. For fixed $a$, the vector-valued [polynomial](../../../../../polynomial-split.md) $(a+tI)^{\otimes n}$ has degree at most $n$. Choose $n+1$ distinct values of $t$ away from the finitely many roots of $\det(a+tI)$. [Polynomial interpolation](../../../../../polynomial-interpolation.md) expresses its constant term $a^{\otimes n}$ as a [linear combination](../../../../../linear-combination.md) of those invertible [tensor powers](../../../../../tensor-power.md). Consequently

$$
S_{\mathbb C}(m,n)=\operatorname{span}_{\mathbb C}\{g^{\otimes n}:g\in\operatorname{GL}(V)\}.
$$

The span is an algebra, since products are $(gh)^{\otimes n}$.

The image $A_T$ of $\mathbb CS_n$ is semisimple, as a quotient of a [semisimple algebra](../../../../../semisimple-algebra.md). The [double-centralizer theorem for semisimple operator algebras](../../../../../double-centralizer-theorem-for-semisimple-operator-algebras.md) gives $A_T''=A_T$. Since the preceding computation says that $A_T'$ is the span of the general linear action, the two actions are **mutual commutants**. More explicitly, [semisimple module](../../../../../semisimple-module.md) decomposition gives

$$
\boxed{V^{\otimes n}\cong
\bigoplus_{\substack{\lambda\vdash n\\\ell(\lambda)\leq m}}
S^\lambda\otimes D_\lambda(V).}
$$

Here $D_\lambda(V)=\operatorname{Hom}_{S_n}(S^\lambda,T)$ is the multiplicity space, with its natural general linear action. The commutant algebra is the product of the full [endomorphism](../../../../../endomorphism.md) algebras of these multiplicity spaces. Hence each nonzero $D_\lambda$ is irreducible, and distinct spaces have nonisomorphic general linear representations, because the operators $g^{\otimes n}$ span that commutant. A primitive $e_t$ picks a one-dimensional factor from $S^\lambda$, so $e_tT$ is an equivalent realization of $D_\lambda$ as a [Schur module](../../../../../schur-module.md).

The range of shapes is exact. If $\lambda$ has more than $m$ rows, a column antisymmetrizes more than $m$ vectors and its action vanishes by $\Lambda^{m+1}V=0$. Conversely, for at most $m$ rows place the $i$th basis vector in every tensor position belonging to row $i$ of $t$. Row symmetrization multiplies this tensor by $\prod_i\lambda_i!$. Column antisymmetrization is nonzero, because all vectors within each column are distinct, and its different [permutations](../../../../../permutation.md) give distinct basis tensors. Thus $h_tT\ne0$. This proves the [length bound for a Schur module](../../../../../length-bound-for-a-schur-module.md) and the stated [Schur–Weyl duality](../../../../../schur-weyl-duality.md). For $n=0$, the empty partition and $V^{\otimes0}=\mathbb C$ give the trivial version.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 3](../../paper-3-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
