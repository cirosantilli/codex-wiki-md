<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Suppose first that $Z$ is a [bisimulation](../../../../../../bisimulation.md) containing the root pair. II maintains the invariant that the current pair lies in $Z$. If I moves in the first [rooted directed graph](../../../../../../rooted-directed-graph.md), the forth clause supplies a matching successor in the second; if I moves in the second, the back clause supplies a matching successor in the first. II can choose such a response every time I can move. Therefore II never loses after finitely many steps and wins the [bisimulation game](../../../../../../bisimulation-game.md).

Conversely, let $\sigma$ be a winning strategy for II. Define $Z$ to consist of all endpoint pairs of finite legal plays starting at the roots and consistent with $\sigma$, including the initial root pair. This definition keeps every possible history; it does not assume that $\sigma$ depends only on the current position.

Take $(g,h)\in Z$ and a finite history realizing it. For any successor $g'$ of $g$, extend that history by having I choose the edge $g\to g'$. Since $\sigma$ is winning, it supplies a successor $h'$ of $h$. The new endpoint pair $(g',h')$ belongs to $Z$, proving forth. Letting I choose any successor of $h$ proves back in the same way. Hence $Z$ is a [bisimulation](../../../../../../bisimulation.md) and

$$
\boxed{\text{II wins the bisimulation game}\iff G\text{ and }H\text{ are bisimilar}.}
$$

Connectedness ensures that both projections of $Z$ cover all vertices: I can walk any finite directed path from either root and II's strategy supplies the matching path. The equivalence itself only concerns the rooted reachable behaviour and remains valid without connectedness.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [4](../../4.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
