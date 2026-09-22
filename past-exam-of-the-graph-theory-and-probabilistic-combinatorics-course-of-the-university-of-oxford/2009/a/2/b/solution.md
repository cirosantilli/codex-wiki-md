<h1 id="a/2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Induct using the same [deletion-contraction recurrence for the chromatic polynomial](../../../../../deletion-contraction-recurrence-for-the-chromatic-polynomial.md). The edgeless [graph](../../../../../graph-split.md) has [polynomial](../../../../../polynomial-split.md) $x^n$, so its leading coefficient is one and the others are zero. All nonempty-vertex chromatic polynomials have zero constant term, since no coloring uses zero colors.

For an existing edge, write the alternating coefficient lists of the deletion and simplified contraction as $a_i'$ and $a_i''$. The contraction has $n-1$ vertices, so subtracting its [polynomial](../../../../../polynomial-split.md) changes its leading sign by one place. Thus

$$
a_i(G)=a_i'+a_{i-1}'',
$$

with nonexistent indices understood as zero. Both summands are nonnegative by [induction](../../../../../mathematical-induction.md). The leading coefficient is $a_0=1$, and the next is

$$
a_1=(m-1)+1=m.
$$

This proves the alternating expansion and **nonnegativity of every $a_i$**. The coefficient assertion for $a_1$ is relevant when $n\geq2$; the one-vertex [graph](../../../../../graph-split.md) simply has [polynomial](../../../../../polynomial-split.md) $x$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../split.md)
6. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
