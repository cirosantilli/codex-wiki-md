<h1 id="14f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The nearest-point assertion requires **$F\ne\varnothing$**. If $F=\varnothing$, there is no possible point $q$, so the literal assertion for every closed subset has that exception.

For a nonempty closed subset $F$ of a [compact metric space](../../../../../../compact-metric-space.md), $F$ is itself compact. The function $q\mapsto d(p,q)$ is continuous, since $|d(p,q)-d(p,q')|\leq d(q,q')$ by the [triangle inequality](../../../../../../triangle-inequality.md). The [extreme value theorem](../../../../../../extreme-value-theorem.md) therefore gives a minimizer $q\in F$, with

$$
\boxed{d(p,q)=\inf_{q'\in F}d(p,q').}
$$

Now assume the midpoint property and suppose $X$ were disconnected. There would be nonempty disjoint relatively open sets $A,B$ with $X=A\cup B$. Each is also closed, hence compact. The continuous distance function on the compact product $A\times B$ attains its minimum $\delta=d(a,b)$. It is positive, since a zero value would imply $a=b$.

Choose a midpoint $m$ of this minimizing pair. It lies in either $A$ or $B$. In the first case $d(m,b)=\delta/2<\delta$ contradicts minimality; in the second, $d(a,m)=\delta/2<\delta$ does. Thus **the midpoint property forces $X$ to be connected**. The empty space is connected by the usual no-separation definition, so it also causes no exception here.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [14F](../../14f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
