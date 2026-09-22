<h1 id="2/b/ii/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $A_N=\sum_{n=1}^Na_n$, using the finite representatives from part (B). Then $A_N\to A$ [almost everywhere](../../../../../../almost-everywhere.md), and $|A_N|\leq S=\sum_n|a_n|$, where $S$ is integrable by part (A). The [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) gives

$$
\boxed{\int_E\sum_{n=1}^\infty a_n(x)\,dx
=\lim_{N\to\infty}\int_EA_N
=\sum_{n=1}^\infty\int_Ea_n(x)\,dx.}
$$

The numerical series on the right converges absolutely because $|\int_Ea_n|\leq\int_E|a_n|$ and the sum of these bounds is finite. Moreover,

$$
\|A-A_N\|_1\leq\sum_{n>N}\int_E|a_n|\longrightarrow0.
$$

Thus [integration of a series with summable L1 norms](../../../../../../integration-of-a-series-with-summable-l1-norms.md) also yields convergence of the partial sums in [L1 norm](../../../../../../l1-norm.md).

## ↑ Ancestors (14)

1. [C](../c.md)
2. [Ii](../../ii.md)
3. [B](../../../b.md)
4. [2](../../../../2.md)
5. [2017](../../../../../2017-split.md)
6. [Past exam of the integration course of the University of Oxford](../../../../../split.md)
7. [Integration course of the University of Oxford](../../../../../../integration-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
