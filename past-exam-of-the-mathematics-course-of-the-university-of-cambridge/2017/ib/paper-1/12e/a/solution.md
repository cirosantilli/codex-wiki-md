<h1 id="12e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

If a nonempty subset $S\subset\mathbb R$ is not an interval, there are $a,b\in S$ and $c\notin S$ with $a<c<b$. The disjoint nonempty relatively open sets $S\cap(-\infty,c)$ and $S\cap(c,\infty)$ form a separation, so $S$ is not [connected](../../../../../../connected-space.md).

Conversely, suppose an interval $I$ had a separation into relatively open nonempty sets $A,B$. Choose $a\in A,b\in B$, interchanging the names if necessary so $a<b$. Put $c=\sup(A\cap[a,b])$. Because $B$ contains a relative neighbourhood of $b$, $c<b$; because $A$ contains a relative neighbourhood of $a$, $c>a$. Also $c\in[a,b]\subset I$. If $c\in A$, relative openness supplies points of $A$ just above $c$, contradicting the [supremum](../../../../../../supremum.md). If $c\in B$, a relative neighbourhood of $c$ excludes points of $A$ approaching $c$ from below, again contradicting the [supremum](../../../../../../supremum.md). Thus every interval is [connected](../../../../../../connected-space.md), including a singleton and unbounded or open intervals.

Take

$$
\boxed{K=\{0\}\cup\{1/n:n\ge1\}}.
$$

It is closed, because its only accumulation point is $0$ and that point is included, and bounded. The [Heine-Borel theorem](../../../../../../heine-borel-theorem.md) makes it [compact](../../../../../../compact-space.md). The [connected components](../../../../../../connected-component.md) of its complement are precisely

$$
(-\infty,0),\quad(1,\infty),\quad\left(\frac1{n+1},\frac1n\right)\quad(n\ge1).
$$

Each is an interval and therefore [connected](../../../../../../connected-space.md); none can be enlarged inside the complement across one of the intervening points of $K$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [12E](../../12e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
