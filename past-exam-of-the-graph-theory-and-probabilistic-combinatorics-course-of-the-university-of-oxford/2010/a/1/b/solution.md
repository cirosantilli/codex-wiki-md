<h1 id="a/1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Induct on the number of edges, allowing coefficients outside the displayed degree range to be zero. An edgeless [graph](../../../../../graph-split.md) has $p_G(x)=x^n$, so its leading coefficient is $1$ and all others are zero. For an [edge](../../../../../edge-of-a-graph.md) $e$, write the alternating coefficients of $G-e$ as $b_i$ and those of the simplified contraction $G/e$ as $c_i$. The [deletion-contraction recurrence for the chromatic polynomial](../../../../../deletion-contraction-recurrence-for-the-chromatic-polynomial.md) gives

$$
p_G(x)=\sum_i(-1)^ib_i x^{n-i}-\sum_j(-1)^jc_j x^{n-1-j}
=\sum_i(-1)^i(b_i+c_{i-1})x^{n-i},
$$

with $c_{-1}=0$. Both smaller graphs have fewer edges, so [induction](../../../../../mathematical-induction.md) gives nonnegative coefficients $b_i,c_i$. Thus $a_i=b_i+c_{i-1}\geq0$. Moreover $a_0=b_0=1$ and

$$
a_1=b_1+c_0=(m-1)+1=m.
$$

For a [graph](../../../../../graph-split.md) with at least one [vertex](../../../../../vertex-graph-theory.md), $p_G(0)=0$, so the constant term vanishes. Therefore

$$
\boxed{p_G(x)=\sum_{i=0}^{n-1}(-1)^ia_i x^{n-i},\quad a_0=1,\quad a_1=m,\quad a_i\geq0.}
$$

In the one-[vertex](../../../../../vertex-graph-theory.md) case, the coefficient of $x^{n-1}$ is simply zero; this is the same $a_1=m=0$ convention beyond the written summation range.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../split.md)
6. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
