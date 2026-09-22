<h1 id="22f/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

First suppose $1\leq p<\infty$. Choose a subsequence so that

$$
\lVert f_{n_k}-f\rVert_p^p\leq2^{-k}.
$$

By [Tonelli theorem](../../../../../../../tonelli-theorem.md),

$$
\int_X\sum_{k=1}^\infty|f_{n_k}-f|^p\,d\mu
=\sum_{k=1}^\infty\lVert f_{n_k}-f\rVert_p^p
<\infty.
$$

Hence the sum inside the integral is finite almost everywhere, which forces $|f_{n_k}(x)-f(x)|\to0$ almost everywhere.

If $p=\infty$, choose representatives and remove the countable union of the null sets on which

$$
|f_n-f|>\lVert f_n-f\rVert_\infty.
$$

Outside that null set, norm convergence bounds the pointwise difference and the entire sequence converges to $f$. Thus in every case **an almost-everywhere convergent subsequence exists**, as stated in [Almost-everywhere convergent subsequence from Lp convergence](../../../../../../../almost-everywhere-convergent-subsequence-from-lp-convergence.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [22F](../../../22f.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
