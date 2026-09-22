<h1 id="1/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

**False.** The [Brownian motion produced by the Dambis-Dubins-Schwarz theorem need not be independent of its clock](../../../../../../../brownian-motion-produced-by-the-dambis-dubins-schwarz-theorem-need-not-be-independent-of-its-clock.md). Let $W$ be a standard [Brownian motion](../../../../../../../brownian-motion-split.md) and set

$$
M_t=\int_0^tW_s\,dW_s=\frac12(W_t^2-t),
\qquad
[M]_t=\int_0^tW_s^2ds.
$$

If the Brownian motion $B$ in $M_t=B_{[M]_t}$ were independent of the whole [quadratic variation](../../../../../../../quadratic-variation.md) process, then conditioning on $[M]$ would give $\mathbb E[M_t[M]_t]=\mathbb E[B_{[M]_t}[M]_t]=0$. Instead, the fourth-moment formula for a [bivariate normal distribution](../../../../../../../bivariate-normal-distribution.md) gives $\operatorname{Cov}(W_t^2,W_s^2)=2s^2$ for $s\leq t$, and hence

$$
\mathbb E[M_t[M]_t]=\frac12\int_0^t\operatorname{Cov}(W_t^2,W_s^2)ds=\int_0^ts^2ds=\frac{t^3}{3}>0.
$$

**Thus $B$ and $[M]$ are dependent.**

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 202](../../../../paper-202-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
