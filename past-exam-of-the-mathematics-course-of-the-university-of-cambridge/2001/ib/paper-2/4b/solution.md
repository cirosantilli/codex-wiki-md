<h1 id="4b/solution">Solution</h1>

↑ **Parent:** [4B](../4b.md)

A [connected space](../../../../../connected-space.md) admits no separation into two disjoint nonempty open subsets whose union is the space. A [path-connected space](../../../../../path-connected-space.md) has, for every pair of points, a continuous path from $[0,1]$ joining them. If a path-connected space had a separation $U,V$, choose its endpoints in different pieces. Their inverse images under the path would separate the connected interval $[0,1]$, a contradiction. Thus **path connectedness implies connectedness**.

For the specified subspace, first consider $Y=I\cup\bigcup_{n\ge1}J_n$. Every point of a tooth $J_n$ can move vertically to its base in $I$, then horizontally to the origin; points already on $I$ use only the horizontal segment. Concatenating these paths shows that $Y$ is [path-connected](../../../../../path-connected-space.md) and hence connected.

Every point $(0,t)$ of $A$ is a limit of $(1/n,t)\in Y$. Consequently $Y$ is dense in $X=Y\cup A$ in the [subspace topology](../../../../../subspace-topology.md). To prove $X$ connected, suppose $X=U\cup V$ were a separation. Restricting to the connected $Y$ puts all of $Y$ in one piece, say $U$. But the other nonempty relatively open piece $V$ must meet dense $Y$, a contradiction. Therefore **$\boxed{X\text{ is connected}}$**. This uses density, not an unproved path from the added vertical segment to the teeth.

## ↑ Ancestors (10)

1. [4B](../4b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
