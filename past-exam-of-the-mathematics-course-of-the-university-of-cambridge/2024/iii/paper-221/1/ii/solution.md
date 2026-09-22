<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For a [two-by-two contingency table](../../../../../../two-by-two-contingency-table.md), [Fisher's exact test](../../../../../../fisher-s-exact-test.md) conditions on both row totals and both column totals. Under the null of no association, the upper-left count $K$ then has the [hypergeometric distribution](../../../../../../hypergeometric-distribution.md)

$$
\mathbb P(K=k\mid\text{margins})
=\frac{\binom{c_1}{k}\binom{n-c_1}{r_1-k}}{\binom n{r_1}},
$$

where $r_1$ and $c_1$ are the first row and column totals. A one-sided p-value sums the appropriate hypergeometric tail; a common two-sided p-value sums the probabilities of all feasible tables no more likely under the null than the observed table. Because the conditional distribution is discrete, the p-value is [super-uniform random variable](../../../../../../super-uniform-random-variable.md) rather than generally exactly uniform.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 221](../../../paper-221-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
