<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

We induct on the [nilpotency class](../../../../../../../nilpotency-class.md) $s$. For $s=1$, the group is [Abelian](../../../../../../../abelian-group.md), so take $C_1=A$ and no $X_i$. For $s>1$, part (i) writes

$$
A\subseteq XB_1\cdots B_k
$$

with $X$ small and every $\langle B_i\rangle$ of class at most $s-1$. Apply the induction hypothesis to each $B_i$. Since $B_i\subseteq A^{O(1)}$ and its approximation parameter is $K^{O(1)}$, all resulting small sets lie in $A^{O_s(1)}$, all their sizes are at most

$$
\exp\bigl(O_s(\log^{O(1)}(2K))\bigr),
$$

and all resulting approximate groups lie in $A^{O_s(1)}$ and have approximation parameter $K^{O_s(1)}$. Their generated subgroups are [abelian groups](../../../../../../../abelian-group.md).

There are $O(\log^{O(1)}(2K))$ factors at each of at most $s$ induction levels. Absorbing the resulting products of the bounds into the $O_s$ notation gives

$$
\boxed{m,n\leq O_s(\log^{O_s(1)}(2K)).}
$$

Keeping the factors in the order supplied by the induction yields the required product of the $X_i$ and $C_j$ containing $A$.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 149](../../../../paper-149-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
