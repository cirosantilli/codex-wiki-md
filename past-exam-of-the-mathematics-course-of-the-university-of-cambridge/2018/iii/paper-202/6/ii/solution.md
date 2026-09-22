<h1 id="6/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Take $X=Y=B$, a standard [Brownian motion](../../../../../../brownian-motion-split.md) with $B_0=0$. The [Itô formula](../../../../../../ito-s-lemma.md) and $\langle B\rangle_t=t$ give

$$
\boxed{\int_0^tB_s\circ dB_s=\frac12(B_t^2-t)+\frac12t=\frac12B_t^2.}
$$

If this nonnegative [stochastic process](../../../../../../stochastic-process-split.md), which starts from zero, were a [local martingale](../../../../../../local-martingale.md), question 4(i) would make it a [supermartingale](../../../../../../supermartingale.md) and force its [expectation](../../../../../../expected-value.md) to be at most zero. But $\mathbb E(B_t^2/2)=t/2>0$ for $t>0$. Hence **a [Stratonovich integral](../../../../../../stratonovich-integral.md) is in general not a [local martingale](../../../../../../local-martingale.md).**

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [6](../../6.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
