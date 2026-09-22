<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $p(a)=P(Y_0\geq a)$; because $Y_0\sim N(0,1+1/(2d))$, $p(a)\to0$ as $a\to\infty$. Every [path in a graph](../../../../../../path-in-a-graph.md) of length $n$ contains, by a greedy selection, at least $n/M_d$ vertices at mutual [graph distance](../../../../../../distance-graph-theory.md) greater than two, where $M_d=|B_2(0)|$. The corresponding field values are jointly independent by part (a). Hence the probability that a fixed path lies in the superlevel set is at most

$$
p(a)^{n/M_d}.
$$

There are at most $(2d)^n$ length-$n$ paths from the origin. The [union bound](../../../../../../boole-s-inequality.md) therefore gives

$$
P(0\longleftrightarrow\partial B_n\text{ in }\{Y\geq a\})
\leq(2d)^np(a)^{n/M_d}.
$$

Choose a finite $a$ for which $(2d)p(a)^{1/M_d}<1$ and let $n\to\infty$. There is then no unbounded component through the origin, and translation invariance rules out an unbounded component anywhere almost surely. Thus the [critical threshold for level-set percolation](../../../../../../critical-threshold-for-level-set-percolation.md) satisfies $a_c(d)<\infty$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 226](../../../paper-226-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
