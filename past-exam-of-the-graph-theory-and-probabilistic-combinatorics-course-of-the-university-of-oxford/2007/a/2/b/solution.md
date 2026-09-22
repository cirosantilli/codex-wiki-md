<h1 id="a/2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For an edge $e=uv$, colorings of $G-e$ divide into those giving $u,v$ different colors, counted by $p_G$, and those giving them the same color, counted by $p_{G/e}$. Parallel edges produced by contraction may be suppressed. Thus

$$
p_G(x)=p_{G-e}(x)-p_{G/e}(x).
$$

For an edgeless [graph](../../../../../graph-split.md) on $n\ge1$ vertices, $p_G=x^n$. Induct on the number of edges, allowing smaller vertex counts for contractions. If both smaller expansions have alternating nonnegative coefficients, the contraction's leading [degree](../../../../../degree-of-a-polynomial.md) is one lower, so subtracting it gives

$$
a_i(G)=a_i(G-e)+a_{i-1}(G/e),
$$

with absent coefficients interpreted as zero. Each coefficient remains nonnegative. Both terms have zero constant coefficient for nonempty graphs, so the resulting expansion is

$$
\boxed{p_G(x)=\sum_{i=0}^{n-1}(-1)^ia_ix^{n-i},\qquad a_i\ge0}.
$$

This induction simultaneously proves the counting function is a polynomial.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../split.md)
6. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
