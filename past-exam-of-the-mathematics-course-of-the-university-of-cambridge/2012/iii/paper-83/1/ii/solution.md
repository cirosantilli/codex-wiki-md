<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Order the collection $\operatorname{Ch}(P)$ of every [chain in a partial order](../../../../../../chain-in-a-partial-order.md), including the empty chain, by inclusion. Suppose that $j:\operatorname{Ch}(P)\to P$ is an [order-preserving function](../../../../../../order-preserving-function.md) and an [injection](../../../../../../injective-function.md). Let $\theta=h(P)$ be the [Hartogs ordinal](../../../../../../hartogs-number.md): by [Hartogs theorem](../../../../../../hartogs-theorem.md), no [injection](../../../../../../injective-function.md) from $\theta$ to $P$ exists.

Use [transfinite recursion](../../../../../../transfinite-recursion.md) to define, for $\alpha<\theta$,

$$
C_\alpha=\{p_\beta:\beta<\alpha\},\qquad p_\alpha=j(C_\alpha).
$$

We verify both that $j(C_\alpha)$ is defined and that the values are strictly increasing. Assume inductively that the earlier values are strictly increasing. Then $C_\alpha$ is a [chain in a partial order](../../../../../../chain-in-a-partial-order.md). For any $\beta<\alpha$, $C_\beta\subseteq C_\alpha$, so the fact that $j$ is [order-preserving](../../../../../../order-preserving-function.md) gives $p_\beta\le p_\alpha$. Furthermore $p_\beta\in C_\alpha$, whereas $p_\beta\notin C_\beta$ by distinctness of the earlier values. Thus $C_\beta\ne C_\alpha$, and [injectivity](../../../../../../injective-function.md) gives $p_\beta\ne p_\alpha$. We have proved

$$
\beta<\alpha\quad\Longrightarrow\quad p_\beta<p_\alpha.
$$

The empty initial chain starts the induction, and the same argument applies at every [limit ordinal](../../../../../../limit-ordinal.md).

If a globally defined recursion rule is desired, apply $j$ when the earlier range is a chain and otherwise use the fixed value $j(\varnothing)$. The induction shows that the fallback case never occurs. Thus no choices of new points are being made: the [function](../../../../../../function-split.md) $j$ uniquely determines every stage.

The resulting [function](../../../../../../function-split.md) $\alpha\mapsto p_\alpha$ is an [injection](../../../../../../injective-function.md) from $\theta$ to $P$, contrary to its defining [Hartogs ordinal](../../../../../../hartogs-number.md) property. Hence the [chain-poset nonembedding lemma](../../../../../../chain-poset-nonembedding-lemma.md) gives

$$
\boxed{\text{No order-preserving injection }\operatorname{Ch}(P)\longrightarrow P\text{ exists}.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 83](../../../paper-83-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
