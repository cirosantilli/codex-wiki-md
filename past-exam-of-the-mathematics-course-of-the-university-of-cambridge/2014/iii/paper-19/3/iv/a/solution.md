<h1 id="3/iv/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a regular uncountable [kappa-tree](../../../../../../../kappa-tree.md), keep exactly the nodes whose extensions have unbounded heights:

$$
T^*=\{t\in T:\sup\{\operatorname{ht}(u):u\ge_Tt\}=\kappa\}.
$$

This [set](../../../../../../../set-split.md) is predecessor-closed. At any level $\alpha$, if no node survived, the extension heights above each of its fewer than $\kappa$ nodes would be bounded. Regularity would give a single bound for their union, contradicting the height of the original [set-theoretic tree](../../../../../../../set-theoretic-tree.md). Thus every level of $T^*$ is nonempty and still has size less than $\kappa$.

If $t\in T^*$ and $\beta>\operatorname{ht}(t)$, consider its extensions at level $\beta$. If none survived, fewer than $\kappa$ bounded extension [sets](../../../../../../../set-split.md) would again bound every extension of $t$, a contradiction. Therefore a surviving level-$\beta$ extension exists. Hence

$$
\boxed{T^*\text{ is a well-pruned }\kappa\text{-subtree}.}
$$

This [unbounded-extension kernel of a regular tree](../../../../../../../unbounded-extension-kernel-of-a-regular-tree.md) uses regularity essentially. If one permits singular-height [set-theoretic trees](../../../../../../../set-theoretic-tree.md) in the term “$\kappa$-tree”, the unrestricted assertion is false: take fewer than $\kappa$ disjoint branches with lengths cofinal in a singular $\kappa$. The levels are small and the height is $\kappa$, but no node has unbounded extensions. A common root can be added without creating a well-pruned subtree. The usual regular-height convention is therefore the one used here.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [Iv](../../iv.md)
3. [3](../../../3.md)
4. [Paper 19](../../../../paper-19-split.md)
5. [Iii](../../../../split.md)
6. [2014](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
