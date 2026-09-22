<h1 id="13e/solution">Solution</h1>

↑ **Parent:** [13E](../13e.md)

A [metric space](../../../../../metric-space.md) is [complete](../../../../../completeness.md) if every [Cauchy sequence](../../../../../cauchy-sequence.md) in it converges to a point of that space. The stated shrinking-set characterization is the [Cantor intersection theorem](../../../../../cantor-s-intersection-theorem.md) together with its converse.

First assume [completeness](../../../../../completeness.md), and choose $x_n\in A_n$. If $m,n\geq N$, then both points belong to $A_N$, so $d(x_m,x_n)\leq\operatorname{diam}(A_N)$. The vanishing [diameters](../../../../../diameter.md) imply that $(x_n)$ is a [Cauchy sequence](../../../../../cauchy-sequence.md), hence it converges to some $x\in X$. For every fixed $N$, its tail belongs to the [closed set](../../../../../closed-set.md) $A_N$, so $x\in A_N$. Thus $x\in\bigcap_N A_N$. In fact the intersection contains only one point, since any two of its points have distance at most every diameter.

Conversely assume the stated intersection property and let $(x_n)$ be a [Cauchy sequence](../../../../../cauchy-sequence.md). Put

$$
 A_N=\overline{\{x_n:n\geq N\}}^{\,X}.
$$

These [closures](../../../../../closure-topology.md) are nonempty, closed and nested. Taking a [closure](../../../../../closure-topology.md) does not increase the [diameter](../../../../../diameter.md): approximate two points of the closure by points of the set and use [continuity](../../../../../continuous-function.md) of distance. The [Cauchy sequence](../../../../../cauchy-sequence.md) therefore makes $\operatorname{diam}(A_N)\to0$. Choose $x$ in the intersection. For $n\geq N$, both $x_n$ and $x$ belong to $A_N$, and $d(x_n,x)\leq\operatorname{diam}(A_N)\to0$. Every [Cauchy sequence](../../../../../cauchy-sequence.md) converges in $X$, proving **completeness**.

## ↑ Ancestors (10)

1. [13E](../13e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
