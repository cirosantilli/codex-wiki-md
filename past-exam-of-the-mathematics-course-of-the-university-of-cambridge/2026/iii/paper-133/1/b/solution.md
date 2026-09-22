<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Whenever a combinatorial loop $\alpha$ traverses an oriented edge and immediately traverses the same edge backwards, delete that backtracking pair. Each deletion is a [homotopy relative to endpoints](../../../../../../based-homotopy.md) inside $Z$ and reduces the edge length by two, so the process terminates at a reduced, hence locally injective, combinatorial loop $\beta$.

The universal cover $\widetilde Y$ of a connected graph is a [tree](../../../../../../tree-graph-theory.md). The lift $\widetilde\beta$ is also locally injective because a [covering map](../../../../../../covering-space.md) is a local graph isomorphism. A locally injective edge path in a tree cannot repeat a vertex: the segment between two successive visits would be a nonempty reduced closed path, whereas every closed path in a tree backtracks. Thus $\widetilde\beta$ is injective unless $\beta$ is constant.

Now let a loop in $Z$ become null-homotopic in $Y$. Its reduced representative $\beta$ lifts to a closed path in $\widetilde Y$. The preceding injectivity forces that lift, and hence $\beta$, to be constant. The original loop is null-homotopic in $Z$, proving that

$$
\pi_1(Z,y_0)\longrightarrow\pi_1(Y,y_0)
$$

is an injective [group homomorphism](../../../../../../group-homomorphism.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 133](../../../paper-133-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
