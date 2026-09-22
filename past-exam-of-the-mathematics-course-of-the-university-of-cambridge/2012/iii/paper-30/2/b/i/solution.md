<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Assume $\theta(1/2)>0$. The event that some [infinite percolation cluster](../../../../../../../infinite-percolation-cluster.md) exists is invariant under lattice translations. By [translation ergodicity of Bernoulli percolation](../../../../../../../translation-ergodicity-of-bernoulli-percolation.md), its positive [probability](../../../../../../../probability.md) is therefore one.

Let $D_N$ be the event that an [infinite percolation cluster](../../../../../../../infinite-percolation-cluster.md) meets the finite [graph vertex](../../../../../../../vertex-graph-theory.md) box $B_N=[-N,N]^2$. These [increasing events](../../../../../../../increasing-event.md) increase with $N$, and their union is the event that some [infinite percolation cluster](../../../../../../../infinite-percolation-cluster.md) exists. [Continuity from below of a measure](../../../../../../../continuity-from-below-of-a-measure.md) gives

$$
\mathbb P_{1/2}(D_N)\longrightarrow1.
$$

An [infinite percolation cluster](../../../../../../../infinite-percolation-cluster.md) meeting $B_N$ contains an infinite simple open [ray in a graph](../../../../../../../ray-in-a-graph.md) from a [graph vertex](../../../../../../../vertex-graph-theory.md) of the box. This follows from local finiteness and the [König infinity lemma](../../../../../../../konig-s-lemma.md). That ray visits the finite box only finitely many times; its last box [graph vertex](../../../../../../../vertex-graph-theory.md) lies on the boundary, and the subsequent ray is outside. Thus $D_N$ is also the event that the box boundary intersects an [infinite percolation cluster](../../../../../../../infinite-percolation-cluster.md), and is the union of the four exterior-side arm events.

Consequently, for every $\epsilon>0$, choose $N$ with

$$
\boxed{\mathbb P_{1/2}(\partial B_N\text{ meets an infinite open cluster})>1-\epsilon.}
$$

For $\epsilon\ge1$ any sufficiently large $N$ still satisfies the strict inequality. No uniqueness assertion is needed for this preliminary step.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 30](../../../../paper-30-split.md)
5. [Iii](../../../../split.md)
6. [2012](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
