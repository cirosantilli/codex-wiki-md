<h1 id="6/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write $Z_t=\int_0^te^{-B_s}d\widetilde B_s$, so $X_t=e^{B_t}Z_t$. Independence gives $\langle B,\widetilde B\rangle=0$, and [Itô formula](../../../../../../ito-s-lemma.md) yields

$$
dX_t=\frac12X_tdt+X_tdB_t+d\widetilde B_t.
$$

The martingale part has quadratic variation $(1+X_t^2)dt$, so on an enlarged description it equals $\sqrt{1+X_t^2}\,dW_t$. Thus $X$ is a weak solution of

$$
dU_t=\frac12U_tdt+\sqrt{1+U_t^2}\,dW_t,qquad U_0=0.
$$

On the other hand, another application of Itô's formula gives

$$
dY_t=\frac12Y_tdt+\cosh(B_t)dB_t
=\frac12Y_tdt+\sqrt{1+Y_t^2}\,dB_t.
$$

Both coefficients are [Lipschitz continuous](../../../../../../lipschitz-continuity.md), so [uniqueness in law](../../../../../../uniqueness-in-law.md) gives **$X$ and $Y$ the same law**.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [6](../../6.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
