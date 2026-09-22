<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $\mathbb N=\{1,2,\ldots\}$ and let $\chi$ be the given [finite coloring](../../../../../../finite-coloring.md) of the [edges](../../../../../../edge-of-a-graph.md) of the [complete graph](../../../../../../complete-graph.md) on the [positive integers](../../../../../../positive-integer.md). Construct an increasing [sequence](../../../../../../sequence.md) $(v_i)$ and nested [infinite sets](../../../../../../infinite-set.md) $A_0\supset A_1\supset\cdots$ as follows. Set $A_0=\mathbb N$. Having chosen $A_{i-1}$, take $v_i=\min A_{i-1}$, partition $A_{i-1}\setminus\{v_i\}$ by the color of $\{v_i,w\}$, and use the [infinite pigeonhole principle](../../../../../../infinite-pigeonhole-principle.md) to choose an [infinite set](../../../../../../infinite-set.md) $A_i$ on which this color is constant, say $r_i$. Every element of $A_i$ exceeds $v_i$.

The [infinite pigeonhole principle](../../../../../../infinite-pigeonhole-principle.md) applied again to $(r_i)$ gives an [infinite set](../../../../../../infinite-set.md) of indices $I$ and a color $r$ such that $r_i=r$ for all $i\in I$. For $i<j$ in $I$, nesting gives $v_j\in A_i$, so $\chi(\{v_i,v_j\})=r$. Thus the [infinite set](../../../../../../infinite-set.md) $X=\{v_i:i\in I\}$ is a [monochromatic](../../../../../../monochromatic-set.md) [complete graph](../../../../../../complete-graph.md):

$$
\boxed{\chi\big|_{X^{(2)}}\equiv r.}
$$

This proves the required infinite case of [Ramsey's theorem](../../../../../../ramsey-s-theorem.md); finiteness of the color set is used at both applications of the [infinite pigeonhole principle](../../../../../../infinite-pigeonhole-principle.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 130](../../../paper-130-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
