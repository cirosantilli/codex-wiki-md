<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Under the corrected orthogonality hypothesis, the preceding [quadratic variation](../../../../../../quadratic-variation.md) calculation gives $[X]_t=A_t=\int_0^te^{2B_s}ds$. We justify the needed [infinite occupation time of one-dimensional Brownian motion](../../../../../../infinite-occupation-time-of-one-dimensional-brownian-motion.md), rather than inferring an infinite integral from recurrent visits alone.

Let $T_0=0$, and recursively let $S_n$ be the first exit of $B$ from $(-1,1)$ after $T_n$, and $T_{n+1}$ its first return to zero after $S_n$. [Recurrence of one-dimensional Brownian motion](../../../../../../recurrence-of-one-dimensional-brownian-motion.md) makes these [stopping times](../../../../../../stopping-time.md) finite [almost surely](../../../../../../almost-sure-convergence.md). The [Strong Markov property](../../../../../../strong-markov-property.md) shows that $D_n=S_n-T_n$ are [independent and identically distributed random variables](../../../../../../independent-and-identically-distributed-random-variables.md), each strictly positive. Choose $\varepsilon>0$ with $\mathbb P(D_n\geq\varepsilon)>0$. The [Borel-Cantelli lemma](../../../../../../borel-cantelli-lemmas.md) gives infinitely many such durations and hence $\sum_nD_n=\infty$ [almost surely](../../../../../../almost-sure-convergence.md). These intervals are disjoint, and $|B_s|\leq1$ on each, so

$$
\boxed{[X]_\infty=\int_0^\infty e^{2B_s}\,ds\geq e^{-2}\sum_{n=0}^\infty D_n=\infty\quad\text{almost surely}.}
$$

This proves the intended conclusion. Without the orthogonality correction, the printed setup gives instead the more general [quadratic variation](../../../../../../quadratic-variation.md) in the previous part; it does not justify identifying that quantity with $A$. The proof here is explicitly for the corrected setup.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
