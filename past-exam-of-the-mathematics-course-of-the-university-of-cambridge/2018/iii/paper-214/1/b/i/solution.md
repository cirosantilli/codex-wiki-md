<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $I=\{x:|C(x)|=\infty\}$, the union of all infinite [percolation clusters](../../../../../../../percolation-cluster.md). Since $p>p_c$, the [percolation probability](../../../../../../../percolation-probability.md) $\theta(p)$ is positive. The [translation ergodicity of Bernoulli percolation](../../../../../../../translation-ergodicity-of-bernoulli-percolation.md) makes $\{I\ne\varnothing\}$ a zero-one event; it has positive probability because $\mathbb P_p(0\in I)=\theta(p)>0$, hence it occurs [almost surely](../../../../../../../almost-sure-convergence.md).

Let $D_m=\{B(m)\cap I\ne\varnothing\}$. These events increase to $\{I\ne\varnothing\}$, so [continuity from below of a measure](../../../../../../../continuity-from-below-of-a-measure.md) gives $\mathbb P_p(D_m)\to1$. On $D_m$, some vertex of $B(m)$ has an infinite open [path in a graph](../../../../../../../path-in-a-graph.md). For every $N\geq m$, the segment up to its first visit to $\partial B(N)$ lies entirely in $B(N)$. Thus even with this restriction on the connecting [path in a graph](../../../../../../../path-in-a-graph.md),

$$
\boxed{\inf_{n\geq1}\mathbb P_p\bigl(B(m)\longleftrightarrow\partial B(m+n)\text{ within }B(m+n)\bigr)\geq\mathbb P_p(D_m)\longrightarrow1.}
$$

This proves the requested uniformity and supplies the version needed for crossings later.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 214](../../../../paper-214-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
