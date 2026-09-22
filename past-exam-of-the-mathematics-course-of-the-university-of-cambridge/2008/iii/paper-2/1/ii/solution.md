<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use $c=[a,b]=a^{-1}b^{-1}ab$. The two defining [relators](../../../../../../relator.md) say that $c$ commutes with $a,b$, hence is central. The given [group commutator](../../../../../../group-commutator.md) identities give

$$
(a^mb^nc^k)(a^rb^sc^\ell)
=a^{m+r}b^{n+s}c^{k+\ell-nr}.
$$

Consequently a [word collection in a two-step nilpotent group](../../../../../../word-collection-in-a-two-step-nilpotent-group.md) algorithm maintains an integer triple $(m,n,k)$, initially $(0,0,0)$. Reading $a^\epsilon$, with $\epsilon=\pm1$, changes it to $(m+\epsilon,n,k-n\epsilon)$; reading $b^\epsilon$ changes it to $(m,n+\epsilon,k)$. Each step uses the displayed multiplication rule and reads one letter, so it terminates and produces the requested expression.

By the stipulated uniqueness, **the word is trivial exactly when $\boxed{(m,n,k)=(0,0,0)}$**, which solves its [word problem for a group](../../../../../../word-problem-for-groups.md). Moreover the [commutator subgroup](../../../../../../commutator-subgroup.md) is $\langle c\rangle$: the quotient by $\langle c\rangle$ is abelian, and $c$ itself is a commutator. It is central, so the [nilpotency class](../../../../../../nilpotency-class.md) is at most two. Uniqueness also implies $c\ne1$, since $(0,0,1)$ and $(0,0,0)$ are distinct triples. Hence **the exact nilpotency class is $\boxed{2}$.**

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
