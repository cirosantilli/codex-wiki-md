<h1 id="e/e3/solution">Solution</h1>

↑ **Parent:** [E3](../e3.md)

A [connected space](../../../../connected-space.md) has no expression as the union of two disjoint nonempty [open subsets](../../../../open-set.md). A [continuous](../../../../continuous-function.md) [surjection](../../../../surjective-function.md) to the two-point [discrete space](../../../../discrete-space.md) would pull back its singleton sets to such a separation. Conversely, a separation $X=U\sqcup V$ defines a [continuous](../../../../continuous-function.md) [surjection](../../../../surjective-function.md) by taking the values $0$ on $U$ and $1$ on $V$. Thus these two conditions are equivalent, including for the empty space.

If a subset $S\subseteq\mathbb R$ contains $a<c$ but omits some $b$ between them, its intersections with $(-\infty,b)$ and $(b,\infty)$ separate it. Hence every nonempty [connected](../../../../connected-space.md) subset is an [interval](../../../../interval-mathematics.md). Conversely, let an [interval](../../../../interval-mathematics.md) $I$ have a separation and choose $a<b$ in its opposite sides. Restrict the associated two-valued [continuous function](../../../../continuous-function.md) to $[a,b]\subseteq I$ and regard it as a real-valued function. The [intermediate value theorem](../../../../intermediate-value-theorem.md) forces the value $1/2$, a contradiction. Singletons and the empty set are [connected](../../../../connected-space.md) directly.

For the union assertion, let $u:X\to\{0,1\}$ be [continuous](../../../../continuous-function.md). Each restriction $u|_{A_i}$ is constant because $A_i$ is [connected](../../../../connected-space.md). Since every pair of the $A_i$ intersects, these constants agree, so $u$ is constant on $X$. There is no [continuous](../../../../continuous-function.md) [surjection](../../../../surjective-function.md), and $X$ is [connected](../../../../connected-space.md). The empty indexing case gives $X=\varnothing$ and is harmless.

To apply this to the plane, for each $t\in\mathbb R$ take the union of the horizontal line at height $t$ with the vertical axis. Its two lines are [connected](../../../../connected-space.md) and intersect; all such unions share the vertical axis and cover $\mathbb R^2$. Thus the plane is [connected](../../../../connected-space.md). For the punctured plane, take, for every $r>0$, the circle of radius $r$ together with the positive horizontal ray. The circle is the [continuous image](../../../../continuous-image-of-a-connected-space.md) of $[0,2\pi]$, and intersects that [connected](../../../../connected-space.md) ray. These unions share the ray and cover $\mathbb R^2\setminus\{0\}$, so the punctured plane is [connected](../../../../connected-space.md) too. Translation gives the same conclusion after removing any one point.

Finally, suppose $g:\mathbb R^2\to\mathbb R$ were a [continuous](../../../../continuous-function.md) [injection](../../../../injective-function.md). Its image $I$ is a [connected](../../../../connected-space.md) [interval](../../../../interval-mathematics.md) with at least three points. Choose an interior point $c$ of $I$ and its unique preimage $p$. The restriction of $g$ to $\mathbb R^2\setminus\{p\}$ is a [continuous](../../../../continuous-function.md) [surjection](../../../../surjective-function.md) onto $I\setminus\{c\}$. Its domain is [connected](../../../../connected-space.md), whereas its image is separated by the two half-lines on either side of $c$. This contradicts preservation of [connectedness](../../../../connected-space.md) under [continuous images](../../../../continuous-image-of-a-connected-space.md). Therefore **no continuous [injection](../../../../injective-function.md) of the plane into the line exists**.

## ↑ Ancestors (12)

1. [E3](../e3.md)
2. [E](../../e.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
