<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [nilpotent element](../../../../../../nilpotent.md) belongs to every [prime ideal](../../../../../../prime-ideal.md) and therefore to every [maximal ideal](../../../../../../maximal-ideal.md), so

$$
\sqrt{(0)}\subseteq\operatorname{Jac}(R).
$$

For the reverse containment, let $r$ be nonnilpotent. The [localization of a ring](../../../../../../localization-of-a-ring.md) $S=R[1/r]$ is nonzero: if $1=0$ there, some power of $r$ would annihilate $1$ in $R$. This is still a [finite-type integer algebra](../../../../../../finite-type-integer-algebra.md), because it can be presented as $R[T]/(rT-1)$.

Choose a [maximal ideal](../../../../../../maximal-ideal.md) $\mathfrak n$ of $S$. Its [residue field](../../../../../../residue-field.md) $L=S/\mathfrak n$ is a [finite-type integer algebra](../../../../../../finite-type-integer-algebra.md), hence finite by part (a). Consider the image $F$ of $R$ in $L$. It is a finite [integral domain](../../../../../../integral-domain.md) containing $1$, so it is a [field](../../../../../../field.md): multiplication by a nonzero element is injective on the finite set $F$, hence surjective, and therefore has an inverse in $F$.

The kernel $\mathfrak m$ of $R\to F$ is consequently maximal. The image of $r$ is nonzero, since $r$ became a unit in $S$ and remains a unit in its nonzero [residue field](../../../../../../residue-field.md). Thus $r\notin\mathfrak m$. Every nonnilpotent element can therefore be avoided by a [maximal ideal](../../../../../../maximal-ideal.md), giving

$$
\boxed{\operatorname{Jac}(R)=\sqrt{(0)}}.
$$

This [radical equality for finitely generated integer algebras](../../../../../../radical-equality-for-finitely-generated-integer-algebras.md) uses part (a) to ensure that the contraction of the localized [maximal ideal](../../../../../../maximal-ideal.md) is maximal. Such contraction is not generally maximal for arbitrary [localization of a ring](../../../../../../localization-of-a-ring.md); the finite-field image is the decisive additional step. The zero [ring](../../../../../../ring.md) is immediate, with the intersection of its empty set of [maximal ideals](../../../../../../maximal-ideal.md) understood as the whole [ring](../../../../../../ring.md). No general theorem that integer algebras are [Jacobson rings](../../../../../../jacobson-ring.md) is being quoted.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
