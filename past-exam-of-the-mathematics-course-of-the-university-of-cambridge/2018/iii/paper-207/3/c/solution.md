<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Under the displayed [causal directed acyclic graphs](../../../../../../causal-directed-acyclic-graph.md), with nonzero effects along the relevant arrows and no exact cancellation of the effects on $B$, **the valid [instrumental variables](../../../../../../instrumental-variable.md) are scenarios (i), (ii), and (iv)**. The path arguments are:

- In (i), $G\to B$ supplies [instrument relevance](../../../../../../instrument-relevance.md), and every directed path from $G$ to $Y$ goes through $B$. The unmeasured $U$ does not cause $G$, so [instrumental-variable independence](../../../../../../instrumental-variable-independence.md) holds.
- In (ii), $G\to A\to B$ supplies [instrument relevance](../../../../../../instrument-relevance.md). Although $A$ is unmeasured, every directed path from $G$ to $Y$ still passes through $B$. The path $G\to A\leftarrow U\to Y$ is blocked at its collider $A$ without conditioning, so it does not violate [instrumental-variable independence](../../../../../../instrumental-variable-independence.md).
- In (iii), $G\to C\to Y$ bypasses $B$, violating the [exclusion restriction](../../../../../../exclusion-restriction.md). There is also no directed effect of $G$ on $B$, so [instrument relevance](../../../../../../instrument-relevance.md) is absent in this graph.
- In (iv), both $G\to B$ and $G\to A\to B$ affect $B$, and all directed paths to $Y$ still pass through $B$. The unconditioned collider $G\to A\leftarrow U$ blocks the route to $U$, so both [instrumental-variable independence](../../../../../../instrumental-variable-independence.md) and the [exclusion restriction](../../../../../../exclusion-restriction.md) hold. Conditioning on $A$ could introduce [collider bias](../../../../../../collider-bias.md), but $A$ is not being conditioned on here.
- In (v), $G\to C\to Y$ bypasses $B$, so the [exclusion restriction](../../../../../../exclusion-restriction.md) fails despite the additional $G\to B$ arrow.
- In (vi), $G\to U\to Y$ bypasses $B$, and $G$ affects the unmeasured common cause $U$. Thus the [exclusion restriction](../../../../../../exclusion-restriction.md) and the stated [instrumental-variable independence](../../../../../../instrumental-variable-independence.md) requirement fail.

An upstream intermediate variable need not invalidate an [instrumental variable](../../../../../../instrumental-variable.md) if its routes to the outcome all pass through the target [exposure](../../../../../../exposure.md); an outcome intermediate reached without that [exposure](../../../../../../exposure.md) does invalidate it.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
