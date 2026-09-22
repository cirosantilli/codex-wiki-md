<h1 id="d/3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $G_N=\sum_{n=1}^N|f_n|$. These are nonnegative [measurable functions](../../../../../measurable-function.md) increasing to $G=\sum_{n=1}^\infty|f_n|$, possibly initially with value infinity. [Monotone convergence theorem](../../../../../monotone-convergence-theorem.md) gives

$$
\int_{\mathbb R}G=\lim_N\sum_{n=1}^N\int_{\mathbb R}|f_n|=K<\infty.
$$

An infinite value on a [set](../../../../../set-split.md) of [positive measure](../../../../../positive-measure.md) would force an infinite [integral](../../../../../integral-split.md). Thus $G$ is finite [almost everywhere](../../../../../almost-everywhere.md) and, after setting it to zero on its null exceptional [set](../../../../../set-split.md) if desired, is integrable.

Where $G$ is finite, the real [series](../../../../../series-mathematics.md) $\sum_n f_n$ is [absolutely convergent](../../../../../absolute-convergence.md). Define its sum to be $h$ there and zero on the exceptional [null set](../../../../../null-set.md). Measurability follows as an almost-everywhere limit of [partial sums](../../../../../partial-sum.md), and $|h|\le G$ [almost everywhere](../../../../../almost-everywhere.md) gives integrability. Every [partial sum](../../../../../partial-sum.md) is dominated by $G$, so [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) yields

$$
\boxed{\int_{\mathbb R}h=\lim_N\sum_{n=1}^N\int_{\mathbb R}f_n
=\sum_{n=1}^\infty\int_{\mathbb R}f_n.}
$$

In fact the [convergence](../../../../../convergence.md) is also in the integrable-function [norm](../../../../../norm.md):

$$
\left\|h-\sum_{n=1}^Nf_n\right\|_1
\le\sum_{n>N}\|f_n\|_1\longrightarrow0.
$$

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [D](../../../d.md)
4. [2005](../../../../2005-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
