<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Interpret the invertibility assumption on $G$ as continuity and strict increase on the relevant range, so that $\nu$ is an [atomless measure](../../../../../../non-atomic-measure.md). Suppose a non-decreasing [transport map](../../../../../../transport-map.md) $T$ with $T_\#\mu=\nu$ exists. Then $\mu$ is also an [atomless measure](../../../../../../non-atomic-measure.md): if $\mu(\{x\})>0$, the [pushforward measure](../../../../../../pushforward-measure.md) would give $\nu(\{T(x)\})\geq\mu(\{x\})>0$. Thus $F$ is continuous.

At any point $x$ where the non-decreasing representative is defined, the definition of a [monotone function](../../../../../../monotonic-function.md) gives

$$
\{z:z\leq x\}\subseteq\{z:T(z)\leq T(x)\},\qquad
\{z:T(z)<T(x)\}\subseteq\{z:z<x\}.
$$

Using the [pushforward measure](../../../../../../pushforward-measure.md) identity and continuity of the two [cumulative distribution functions](../../../../../../cumulative-distribution-function.md), we obtain

$$
F(x)\leq G(T(x)),\qquad
G(T(x))=G(T(x)-)\leq F(x-)=F(x).
$$

Consequently

$$
\boxed{T(x)=G^{-1}(F(x))\quad\mu\text{-almost everywhere}.}
$$

The [monotone rearrangement](../../../../../../monotone-rearrangement.md) in part (c) is optimal for the [convex](../../../../../../convex-function.md) difference cost, so $T$ has the same cost and solves the [Monge optimal transport problem](../../../../../../monge-optimal-transport-problem.md). The meaningful uniqueness is up to a $\mu$-null set; arbitrary values away from the source do not affect transport or cost. Existence of the non-decreasing [transport map](../../../../../../transport-map.md) supplies the source condition missing in part (c).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 348](../../../paper-348-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
