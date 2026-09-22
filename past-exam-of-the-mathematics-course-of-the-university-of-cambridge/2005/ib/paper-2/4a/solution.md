<h1 id="4a/solution">Solution</h1>

↑ **Parent:** [4A](../4a.md)

Suppose the union $W$ has a separation $W=A\cup B$ into disjoint, nonempty, relatively open subsets. Each [connected](../../../../../connected-space.md) $U_j$ must lie entirely in one of them: otherwise its intersections with $A$ and $B$ would separate $U_j$ in its [subspace topology](../../../../../subspace-topology.md). In particular $U_1$ lies on one side, say $A$. Every other $U_j$ intersects $U_1$, so it cannot lie in $B$ and must also lie in $A$. Then $W\subseteq A$, contradicting $B\ne\varnothing$. **The union is [connected](../../../../../connected-space.md).** This is the [connected union with a connected hub](../../../../../connected-union-with-a-connected-hub.md) argument.

For path-connectedness, take any $x\in U_i$ and $y\in U_j$. Choose $a\in U_i\cap U_1$ and $b\in U_j\cap U_1$. There is a [path](../../../../../continuous-path.md) from $x$ to $a$ inside $U_i$, a [path](../../../../../continuous-path.md) from $a$ to $b$ inside $U_1$, and a [path](../../../../../continuous-path.md) from $b$ to $y$ inside $U_j$. Concatenate the three [paths](../../../../../continuous-path.md) on successive thirds of $[0,1]$. They agree at the joining points, so the resulting map is [continuous](../../../../../continuous-function.md) and remains in $W$. **The union is [path-connected](../../../../../path-connected-space.md).** There need not be a single point common to all the subsets.

## ↑ Ancestors (10)

1. [4A](../4a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
