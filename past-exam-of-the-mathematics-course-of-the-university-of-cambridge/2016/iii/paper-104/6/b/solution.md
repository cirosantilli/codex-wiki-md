<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

An isomorphism-invariant [Markov property of finitely presented groups](../../../../../../markov-property-of-finitely-presented-groups.md) $\rho$ has two finitely presented witnesses: a group $A_+$ with $\rho$, and a group $A_-$ which cannot embed in any finitely presented group having $\rho$. In symbols,

$$
\boxed{A_+\text{ has }\rho,\qquad A_-\hookrightarrow B\Longrightarrow B\text{ does not have }\rho.}
$$

The second condition is an obstruction to embedding, stronger than merely saying that $A_-$ itself fails the property.

Let $U$ be a fixed finitely presented [group](../../../../../../group-split.md) with unsolvable [word problem for a group](../../../../../../word-problem-for-groups.md). Form the finitely presented [free product](../../../../../../free-product.md) $P=U*A_-$. Given a word $w$ in the generators of $U$, apply part (a) to this $P$ and $w$, and output the finite presentation of

$$
B(w)=A_+*P(w).
$$

If $w=1$ in $U$, it is also $1$ in $P$, so $P(w)$ is trivial and $B(w)\cong A_+$ has $\rho$. If $w\ne1$ in $U$, its image stays nontrivial in the [free product](../../../../../../free-product.md) $P$, and $P$ embeds in $P(w)$. Therefore $A_-$ embeds in $B(w)$, which cannot have $\rho$. We have the effective equivalence

$$
\boxed{B(w)\text{ has }\rho\quad\Longleftrightarrow\quad w=1\text{ in }U.}
$$

An algorithm recognizing whether an arbitrary [finite group presentation](../../../../../../finite-group-presentation.md) has $\rho$ would decide the unsolvable [word problem for a group](../../../../../../word-problem-for-groups.md) $U$. This contradiction proves the [Adian–Rabin theorem](../../../../../../adian-rabin-theorem.md): no [Markov property of finitely presented groups](../../../../../../markov-property-of-finitely-presented-groups.md) is algorithmically decidable.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 104](../../../paper-104-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
