<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $\langle D_\alpha:\alpha\in S\rangle$ witness the [stationary diamond principle](../../../../../../../stationary-diamond-principle.md): for every $A\subseteq\omega_1$, the set of $\alpha\in S$ with $D_\alpha=A\cap\alpha$ is stationary. We construct a normal splitting [Suslin tree](../../../../../../../suslin-tree.md); this will be a nonspecial [Aronszajn tree](../../../../../../../aronszajn-tree.md).

Construct its levels by recursion. Start with one root, and give every node two immediate successors. At a countable limit $\alpha$, the constructed portion $T\upharpoonright\alpha$ is countable. Through each of its nodes choose a [cofinal branch](../../../../../../../cofinal-branch.md) of that portion, and put one new node above each chosen branch at level $\alpha$. This keeps the level countable and gives every earlier node an extension. Branches are identified by their predecessor chains, so nodes at a limit level are uniquely determined by their predecessors.

At a limit $\alpha\in S$, decode $D_\alpha$ as a candidate [tree antichain](../../../../../../../tree-antichain.md) $B$ of $T\upharpoonright\alpha$. If it is maximal, choose the branches just described to meet $B$. This is possible: for any node, maximality supplies a comparable member of $B$, and normality of the already constructed portion extends the larger of those two nodes to a [cofinal branch](../../../../../../../cofinal-branch.md) up to $\alpha$. Then every node at level $\alpha$, and every later node, lies above a member of $B$. This is [antichain sealing by diamond](../../../../../../../antichain-sealing-by-diamond.md).

Here is a precise way to handle the coding. Give the countable level $\xi$ node codes in $[\omega\xi,\omega\xi+\omega)$. There is a [club set](../../../../../../../club-set.md) of countable limit $\alpha$ with $\omega\alpha=\alpha$, and on this club the nodes below $\alpha$ have exactly the relevant codes below $\alpha$. Empty unused codes are ignored. Thus any subset of the entire tree has an ordinal code set to which the [stationary diamond principle](../../../../../../../stationary-diamond-principle.md) applies.

Let $B$ now be any maximal [tree antichain](../../../../../../../tree-antichain.md) of the completed tree. There is a [club set](../../../../../../../club-set.md) of $\alpha$ such that $B\cap(T\upharpoonright\alpha)$ is maximal in $T\upharpoonright\alpha$. Indeed, choose a comparable member of $B$ for each node; closure under the heights of these witnesses gives that club. Intersect it with the coding club. Stationary correct guessing supplies an $\alpha\in S$ on this intersection at which $B$ is sealed. A member of $B$ at or above level $\alpha$ would extend a member of $B$ below $\alpha$, contradicting the [tree antichain](../../../../../../../tree-antichain.md) property. So $B$ is contained in the countable portion below $\alpha$. Every [tree antichain](../../../../../../../tree-antichain.md) extends to a maximal one, hence every [tree antichain](../../../../../../../tree-antichain.md) is countable.

There is no [cofinal branch](../../../../../../../cofinal-branch.md) of length $\omega_1$. Otherwise, choosing at each successor level the other successor of its branch node would give an uncountable [tree antichain](../../../../../../../tree-antichain.md). Thus the resulting tree is a [Suslin tree](../../../../../../../suslin-tree.md). A [special Aronszajn tree](../../../../../../../special-aronszajn-tree.md) is a union of countably many [tree antichains](../../../../../../../tree-antichain.md); here those would all be countable and could not cover the $\aleph_1$ nodes. Therefore

$$
\boxed{\diamondsuit_S\ \Longrightarrow\ \text{a nonspecial Aronszajn tree exists}.}
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 24](../../../../paper-24-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
