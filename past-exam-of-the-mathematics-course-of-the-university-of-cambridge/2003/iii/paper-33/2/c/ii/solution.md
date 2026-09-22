<h1 id="2/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Apply the two-variable [Itô formula](../../../../../../../ito-s-lemma.md) to $e^w\cos b$. The independent [Brownian motions](../../../../../../../brownian-motion-split.md) satisfy $[B,W]=0$, while the two diagonal second derivatives sum to zero. Consequently

$$
dY_t=e^{W_t}\cos B_t\,dW_t-e^{W_t}\sin B_t\,dB_t,\qquad [Y]_t=\int_0^te^{2W_s}\,ds.
$$

Thus $Y$ is a [continuous local martingale](../../../../../../../continuous-local-martingale.md), but **it is not Brownian motion**. Brownian motion from any fixed starting point has quadratic variation $t$. If the displayed bracket were identically $t$, differentiating its continuous density would force $e^{2W_t}=1$ for every $t$, hence $W_t=0$ identically, an event of probability zero. This is the [cosine-exponential Brownian local martingale](../../../../../../../cosine-exponential-brownian-local-martingale.md). Its initial value $Y_0=1$ is retained in the next part.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [Paper 33](../../../../paper-33-split.md)
5. [Iii](../../../../split.md)
6. [2003](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
