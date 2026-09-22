<h1 id="2/b/ii/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $S_N=\sum_{n=1}^N|a_n|$. These are nonnegative measurable functions with $S_N\uparrow S=\sum_{n\geq1}|a_n|$. The [monotone convergence theorem](../../../../../../monotone-convergence-theorem.md) and linearity of the finite sum give

$$
\int_ES=\lim_{N\to\infty}\int_ES_N
=\sum_{n\geq1}\int_E|a_n|<\infty.
$$

Hence $S<\infty$ [almost everywhere](../../../../../../almost-everywhere.md): if $S=\infty$ on a set of positive measure, the integral would exceed every finite constant. Also each $a_n$ is finite almost everywhere, since its absolute integral is finite. Outside the union of these countably many [null sets](../../../../../../null-set.md), all terms are real and

$$
\boxed{\sum_{n=1}^\infty|a_n(x)|<\infty.}
$$

Thus the signed series converges absolutely almost everywhere, as asserted by [summable L1 norms imply almost-everywhere absolute convergence](../../../../../../summable-l1-norms-imply-almost-everywhere-absolute-convergence.md). Removing the common null set avoids any undefined $+\infty-\infty$ in signed partial sums.

## ↑ Ancestors (14)

1. [A](../a.md)
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
