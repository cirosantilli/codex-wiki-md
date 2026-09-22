<h1 id="d/d4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The partial sums $s_n=\sum_{k=1}^n a_k$ are nonnegative [measurable functions](../../../../../measurable-function.md) and increase to an extended-valued function $s$. By the [monotone convergence theorem](../../../../../monotone-convergence-theorem.md),

$$
\int_{\mathbb R}s(x)\,dx
=\lim_{n\to\infty}\sum_{k=1}^n\int_{\mathbb R}a_k(x)\,dx
=\sum_{k=1}^\infty\int_{\mathbb R}a_k(x)\,dx<\infty.
$$

A nonnegative function with finite [Lebesgue integral](../../../../../lebesgue-integral.md) cannot equal $+\infty$ on a set of positive measure: otherwise its [integral](../../../../../integral-split.md) would exceed $M$ times that measure for every $M>0$. Thus the [series](../../../../../series-mathematics.md) converges to a finite value almost everywhere. Redefine it to be zero on the exceptional [null set](../../../../../null-set.md) if a finite-valued representative is desired. The resulting function is [Lebesgue integrable](../../../../../integrability.md), with

$$
\boxed{\int\sum_{k=1}^\infty a_k=\sum_{k=1}^\infty\int a_k.}
$$

## ↑ Ancestors (13)

1. [B](../b.md)
2. [D4](../../d4.md)
3. [D](../../../d.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
