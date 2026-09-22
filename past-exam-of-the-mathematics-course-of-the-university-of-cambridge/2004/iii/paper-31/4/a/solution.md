<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the stated [continuity](../../../../../../continuous-function.md) of the infinite-buffer and finite-buffer [queue workload](../../../../../../workload-of-a-queue.md) maps on the input path space. The [contraction principle for large deviations](../../../../../../contraction-principle-for-large-deviations.md) gives, at the same speed as the input sequence,

$$
\boxed{J(x)=\inf\{I(a):q(a)=x\},\qquad\bar J(x)=\inf\{I(a):\bar q(a)=x\}.}
$$

Empty fibers have [infimum](../../../../../../infimum.md) infinity. Both rates are good because they are continuous contractions of the [good rate function](../../../../../../good-rate-function.md) I. In particular, at speed L the infinite-buffer [queue workload](../../../../../../workload-of-a-queue.md) satisfies, for every Borel set E,

$$
-\inf_{E^\circ}J\leq\liminf_L L^{-1}\log\mathbb P(q(A^L)\in E)\leq\limsup_L L^{-1}\log\mathbb P(q(A^L)\in E)\leq-\inf_{\overline E}J,
$$

and the identical bounds with bars give the finite-buffer [queue workload](../../../../../../workload-of-a-queue.md) LDP. This states the entire principles, not just an informal tail approximation.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 31](../../../paper-31-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
