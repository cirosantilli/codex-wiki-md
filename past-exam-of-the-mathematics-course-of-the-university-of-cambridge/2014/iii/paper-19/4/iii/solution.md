<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Fix a [diamond principle](../../../../../../diamond-principle.md) sequence $D_\alpha\subseteq\alpha$. Construct a normal splitting [set-theoretic tree](../../../../../../set-theoretic-tree.md) of height $\omega_1$ with countable levels. At successors give every node two successors. At a countable limit stage $\alpha$, the [set-theoretic tree](../../../../../../set-theoretic-tree.md) below $\alpha$ is countable. Choose countably many [cofinal branches](../../../../../../cofinal-branch.md) through it covering all its nodes, and put one node at level $\alpha$ above each distinct chosen branch. This preserves extension to all higher levels and [tree with unique limits](../../../../../../tree-with-unique-limits.md).

Arrange a coding of each level into the [ordinal](../../../../../../ordinal.md) block $[\omega\alpha,\omega(\alpha+1))$. On the [club set](../../../../../../club-set.md) of limit fixed points of $\alpha\mapsto\omega\alpha$, the nodes coded below $\alpha$ are exactly the nodes of height below $\alpha$. At a limit stage, if $D_\alpha$ codes a maximal [tree antichain](../../../../../../tree-antichain.md) of the current [set-theoretic tree](../../../../../../set-theoretic-tree.md) below $\alpha$, require every chosen branch to meet it. This is possible: for any starting node $t$, maximality provides a comparable [tree antichain](../../../../../../tree-antichain.md) member; if above $t$, first extend to it, and if below $t$, it has already been met. Then extend along a sequence of heights cofinal in $\alpha$. If the prediction is not a maximal [tree antichain](../../../../../../tree-antichain.md), use the ordinary covering branches. Thus every level is countable and the construction remains normal.

Here is the full chain-condition verification. Let $A$ be a maximal [tree antichain](../../../../../../tree-antichain.md) in the final [set-theoretic tree](../../../../../../set-theoretic-tree.md). For every node $t$, choose a witness $a_t\in A$ comparable with $t$. There is a [club set](../../../../../../club-set.md) of countable limit stages $\alpha$ closed under these witness choices: starting from any bound, repeatedly bound the heights of witnesses for all the countably many nodes below the current stage, and take the supremum after countably many steps. At such an $\alpha$, $A\cap T_{<\alpha}$ is already maximal in $T_{<\alpha}$.

View $A$ as a [subset](../../../../../../subset.md) of $\omega_1$ through the coding. Diamond gives stationarily many stages with $D_\alpha=A\cap\alpha$. Choose one also in the witness-closure [club set](../../../../../../club-set.md) and the coding [club set](../../../../../../club-set.md). The construction at that stage seals this very [tree antichain](../../../../../../tree-antichain.md): every node of level $\alpha$ extends one of its members below $\alpha$, and so does every node at a later level. No such node can itself belong to $A$, since it is comparable with an earlier member of $A$. Hence

$$
\boxed{A\subseteq T_{<\alpha},\qquad A\text{ is countable}.}
$$

Every [tree antichain](../../../../../../tree-antichain.md) extends to a maximal one, so the [set-theoretic tree](../../../../../../set-theoretic-tree.md) has no uncountable [tree antichain](../../../../../../tree-antichain.md). Its normal splitting also excludes uncountable branches by part (ii). It is therefore a [Suslin tree](../../../../../../suslin-tree.md). By the standard Suslin-tree characterization of [Suslin hypothesis](../../../../../../suslin-hypothesis.md), **diamond implies failure of [Suslin hypothesis](../../../../../../suslin-hypothesis.md)**. The decisive step is [antichain sealing by diamond](../../../../../../antichain-sealing-by-diamond.md), with maximality below a correctly guessed [club set](../../../../../../club-set.md) stage verified explicitly.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 19](../../../paper-19-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
