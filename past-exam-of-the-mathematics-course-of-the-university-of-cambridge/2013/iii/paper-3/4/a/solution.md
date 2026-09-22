<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A point is an element of $H$. A [duad](../../../../../../duad.md) is an unordered two-element subset. A [syntheme](../../../../../../syntheme.md) is a partition of $H$ into three [duads](../../../../../../duad.md), and a [total of synthemes](../../../../../../total-of-synthemes.md) is a collection of five [synthemes](../../../../../../syntheme.md) whose [duads](../../../../../../duad.md) partition all fifteen [duads](../../../../../../duad.md). In graph terms these are vertices, edges, [perfect matchings](../../../../../../perfect-matching.md) and [one-factorization](../../../../../../one-factorization.md) of $K_6$.

The first counts are $6$, $\binom62=15$, and

$$
\frac{6!}{2^3\,3!}=15
$$

[synthemes](../../../../../../syntheme.md). To count totals, first observe that two edge-disjoint [synthemes](../../../../../../syntheme.md) have union a six-cycle. Its complement in $K_6$ is a triangular prism: two triangles on alternate cycle vertices, joined by the three remaining cross edges. Its [perfect matchings](../../../../../../perfect-matching.md) are the matching using all three cross edges and three matchings using one cross edge each. The all-cross matching cannot be used in a factorization, because the remaining two odd triangles cannot be matched. The other three matchings partition the prism edges. Therefore **every pair of disjoint [synthemes](../../../../../../syntheme.md) extends to a unique total**.

Fix a [syntheme](../../../../../../syntheme.md) $s$. Each of its three [duads](../../../../../../duad.md) belongs to three [synthemes](../../../../../../syntheme.md). Inclusion-exclusion shows that $3\cdot3-3+1=7$ [synthemes](../../../../../../syntheme.md) share a [duad](../../../../../../duad.md) with $s$, including $s$ itself. Thus eight are disjoint from $s$. A total containing $s$ uses four of these, and each disjoint [syntheme](../../../../../../syntheme.md) determines exactly one such total. Hence $s$ belongs to $8/4=2$ totals. Counting incidences gives

$$
\boxed{\#\text{points}=6,\quad\#\text{duads}=15,\quad\#\text{synthemes}=15,\quad\#\text{totals}=15\cdot2/5=6.}
$$

Two different totals share at most one [syntheme](../../../../../../syntheme.md), by the unique-completion assertion. There are fifteen pairs of totals and fifteen [synthemes](../../../../../../syntheme.md) each belonging to two totals; consequently **each pair of totals has exactly one common [syntheme](../../../../../../syntheme.md)**. This incidence property drives the next construction.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
