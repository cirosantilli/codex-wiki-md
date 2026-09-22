<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Definition 1 satisfies Property 1 but not Property 2. Let $S_1$ contain every non-descendant that blocks some backdoor path. Every backdoor path begins $A\leftarrow P$ for a parent $P$ of $A$; whenever that path can transmit confounding, $P\in S_1$. Conditioning on $S_1$ therefore blocks every such path at its first nonendpoint vertex, so $S_1$ is sufficient.

For failure of Property 2, consider the faithful graph with arrows

$$
C\to A,qquad C\to Y,qquad C\to X_i\to Y.
$$

The variable $X_i$ blocks the backdoor path $A\leftarrow C\to X_i\to Y$, so Definition 1 calls it a confounder. Every sufficient set containing $X_i$ must nevertheless contain $C$ to block $A\leftarrow C\to Y$. Once $C$ is included, deleting $X_i$ leaves a sufficient set. Thus $X_i$ can never be essential as Property 2 demands.

Definition 2 satisfies Property 2 but not Property 1. If $X_i$ belongs to every [minimal sufficient adjustment set](../../../../../../minimal-sufficient-adjustment-set.md), choose one such set $I$ and put $J=I\setminus\{i\}$. By minimality, $J\cup\{i\}$ is sufficient and $J$ is not, proving Property 2.

For failure of Property 1, use the faithful chain-shaped backdoor path

$$
A\leftarrow C_1\to C_2\to Y.
$$

Both $\{C_1\}$ and $\{C_2\}$ are minimal sufficient adjustment sets. No variable belongs to every minimal sufficient set, so Definition 2 labels no variable a confounder, but the empty set is not sufficient.

Definition 3 satisfies Property 1 but not Property 2. Under faithfulness, its associational criterion contains enough non-descendants to block every open backdoor path. Indeed, if such a path remained open, its first unconditioned parent of $A$ would be D-connected to $A$ and, after a suitable conditioning set, to $Y$ given $A$; faithfulness would place that parent in the Definition 3 set, a contradiction. Thus adjusting for all variables selected by Definition 3 is sufficient.

For failure of Property 2, consider

$$
Z\to A\leftarrow U\to Y,qquad A\to Y,
$$

with both $Z$ and $U$ observed and a faithful distribution. The [instrumental variable](../../../../../../instrumental-variable.md) $Z$ is associated with $A$. Conditioning on the [collider](../../../../../../collider.md) $A$ opens $Z\to A\leftarrow U\to Y$, so $Z$ is associated with $Y$ given $A$ and Definition 3 calls it a confounder. Any sufficient set containing $Z$ must also contain $U$ to block $A\leftarrow U\to Y$, but $\{U\}$ is already sufficient. Hence removing $Z$ never destroys sufficiency, violating Property 2.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 221](../../../paper-221-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
