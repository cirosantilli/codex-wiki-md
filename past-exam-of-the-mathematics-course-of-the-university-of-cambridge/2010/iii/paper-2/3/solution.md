<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For a finite-dimensional algebra over an [algebraically closed field](../../../../../algebraically-closed-field.md), [basic algebra](../../../../../basic-algebra.md) means $A/J(A)\cong k^n$, so its [simple modules](../../../../../irreducible-module.md) are one-dimensional and occur once in the semisimple quotient of the regular [module](../../../../../module-mathematics.md). A [hereditary ring](../../../../../hereditary-ring.md) has every [submodule](../../../../../submodule.md) of a [projective module](../../../../../projective-module.md) projective; equivalently its [global dimension](../../../../../global-dimension.md) is at most one.

Choose representatives $S_1,\ldots,S_n$ of the [simple modules](../../../../../irreducible-module.md). Our [Ext quiver](../../../../../ext-quiver.md) convention gives one vertex $i$ for $S_i$ and

$$
\#\{i\to j\}=\dim_k\operatorname{Ext}^1_A(S_i,S_j).
$$

With primitive orthogonal [idempotents](../../../../../idempotent.md) $e_i$, put $P_i=Ae_i$ and $J=J(A)$. Applying $\operatorname{Hom}_A(-,S_j)$ to $0\to JP_i\to P_i\to S_i\to0$ gives

$$
\operatorname{Ext}^1_A(S_i,S_j)
\cong\operatorname{Hom}_A(JP_i/J^2P_i,S_j).
$$

The restriction map from $\operatorname{Hom}(P_i,S_j)$ is zero since every map to a simple kills $JP_i$, and $P_i$ is projective. Thus the arrow multiplicity is $\dim e_j(J/J^2)e_i$. This specifies the orientation rather than silently replacing the [quiver](../../../../../quiver.md) by its opposite.

Because $A$ is hereditary, $JP_i$ is projective. Its semisimple top has $a_{ij}$ copies of $S_j$, where $a_{ij}$ is the arrow multiplicity. Its [projective cover](../../../../../projective-cover.md) therefore supplies an epimorphism

$$
\bigoplus_jP_j^{a_{ij}}\twoheadrightarrow JP_i.
$$

This splits by projectivity of $JP_i$. Its [kernel](../../../../../kernel-of-a-linear-map.md) is a summand contained in the radical of the source; projection onto that summand and [Nakayama lemma](../../../../../nakayama-lemma.md) force the [kernel](../../../../../kernel-of-a-linear-map.md) to be zero. Hence

$$
\boxed{JP_i\cong\bigoplus_jP_j^{a_{ij}},\qquad
\dim P_i=1+\sum_ja_{ij}\dim P_j.}
$$

Every arrow $i\to j$ forces $\dim P_i>\dim P_j$, so $Q$ has no directed cycles.

Choose lifts in $e_jJe_i$ of bases of the arrow spaces. Send the vertices and arrows of the [path algebra](../../../../../path-algebra.md) to these [idempotents](../../../../../idempotent.md) and lifts, multiplying paths in the order $\beta\alpha$ for consecutive arrows $\alpha:i\to j$, $\beta:j\to l$. This defines an [algebra homomorphism](../../../../../algebra-homomorphism-over-a-field.md) $kQ\to A$. It is surjective: vertices span $A/J$, arrows span $J/J^2$, and products show that paths of length $r$ span $J^r/J^{r+1}$. Nilpotence of $J$ then gives all of $A$.

Let $N_i$ be the number of directed paths starting at $i$, including the length-zero path. Acyclicity gives the same recursion $N_i=1+\sum_ja_{ij}N_j$, with value one at a sink. Induction from sinks gives $N_i=\dim P_i$. Therefore

$$
\dim kQ=\sum_iN_i=\sum_i\dim P_i=\dim A.
$$

The surjective homomorphism is an isomorphism. This proves the [basic hereditary algebra path-algebra theorem](../../../../../basic-hereditary-algebra-path-algebra-theorem.md):

$$
\boxed{A\cong kQ.}
$$

For each connected component $C$ of the underlying unoriented graph, $e_C=\sum_{i\in C}e_i$ is a [central idempotent](../../../../../central-idempotent.md). Paths never connect distinct components, so $kQ=\bigoplus_Ce_CkQ$ as a [direct sum](../../../../../direct-sum.md) of [two-sided ideals](../../../../../two-sided-ideal.md). To prove each is a block, let $z$ be any [central idempotent](../../../../../central-idempotent.md). Modulo the arrow ideal it has coordinates $c_i\in\{0,1\}$. Commuting $z$ with an arrow $i\to j$ and reducing modulo the square of that ideal gives $c_i=c_j$. Thus these coordinates are constant on each component. If they are zero on a component, the restriction of $z$ there is a nilpotent [idempotent](../../../../../idempotent.md), hence zero; if they are one, apply that argument to $1-z$. Consequently

$$
\boxed{\text{blocks of }A\ \longleftrightarrow\ \text{connected components of the underlying graph of }Q.}
$$

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 2](../../paper-2-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
