<h1 id="1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Consider the following game on the real numbers. On their first moves, Player I plays $y\in\mathbb R$ and Player II replies with $x\in\mathbb R$; later moves are ignored. Declare Player II the winner when

$$
y\notin pA
\quad\text{or}\quad
(x,y)\in A.
$$

Player I cannot have a [winning strategy in an infinite game](../../../../../../winning-strategy-in-an-infinite-game.md): its first move is some fixed $y$, and if $y\notin pA$ then II wins automatically, while if $y\in pA$ then II can reply with an $x$ satisfying $(x,y)\in A$.

The [axiom of determinacy](../../../../../../axiom-of-determinacy.md) for games on $\mathbb R$ therefore gives Player II a winning strategy $\tau$. For every $y\in pA$, define $f(y)$ to be II's first response to the move $y$. The winning condition forces

$$
(f(y),y)\in A,
$$

so $f:pA\to\mathbb R$ is the required [uniformization of a binary relation](../../../../../../uniformization-of-a-binary-relation.md). This is the direct game proof of [uniformization from determinacy](../../../../../../uniformization-from-determinacy.md).

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [1](../../1.md)
3. [Paper 158](../../../paper-158-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
