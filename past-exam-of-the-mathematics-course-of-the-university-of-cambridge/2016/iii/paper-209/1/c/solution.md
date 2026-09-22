<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $h=h_n$ and $I=[t_0,t_0+h]$, restricting to meshes small enough that $t_0+h\leq1$. This discontinuous [indicator function](../../../../../../indicator-function.md) does not satisfy the hypothesis of part (b). Instead apply part (a) with $\|g_n\|_\infty=1/h$ and handle its two boundary cells directly.

Let $q_n(s)=g_n(t_{i-1})$ on each observation cell $[t_{i-1},t_i)$. Away from cells containing the two ends of $I$, $q_n=g_n$ almost everywhere. Even if an endpoint is itself an observation time, at most two cells contribute, and their total length is at most $2\Delta$. Thus the [quadrature error](../../../../../../quadrature-error.md) obeys

$$
B_n=\int_0^1(q_n-g_n)\sigma^2\,ds,\qquad
|B_n|\leq2\|\sigma^2\|_\infty\frac{\Delta}{h}.
$$

The fluctuation has [variance](../../../../../../variance-split.md) at most $2S\Delta/h^2$. Its zero [expected value](../../../../../../expected-value.md) gives

$$
\mathbb E\bigl(\widehat\Lambda_n(g_n)-\Lambda(g_n)\bigr)^2
\leq\frac{S}{h^2}(2\Delta+4\Delta^2)
\leq6S\frac{\Delta}{h^2},
$$

using $\Delta\leq1$.

<a id="1/c/image-only-the-two-endpoint-cells-contribute-to-the-window-quadrature-error"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-209-window-cells.png)

**[Figure 1](#1/c/image-only-the-two-endpoint-cells-contribute-to-the-window-quadrature-error). Only the two endpoint cells contribute to the window quadrature error**.

The remaining [bias](../../../../../../bias-of-an-estimator.md) is the difference between an interval average and the [spot variance](../../../../../../spot-variance.md). By the [Hölder continuity](../../../../../../holder-condition.md) of $\sigma^2$,

$$
A_h=\Lambda(g_n)-\sigma^2(t_0),\qquad
|A_h|\leq\frac1h\int_0^h C s^\beta\,ds
=\frac{C}{1+\beta}h^\beta.
$$

Retaining the centered fluctuation and bounding $(B_n+A_h)^2\leq2B_n^2+2A_h^2$ yields

$$
\mathbb E\bigl(\widehat\Lambda_n(g_n)-\sigma^2(t_0)\bigr)^2
\leq10S\frac{\Delta}{h^2}+2C^2h^{2\beta}.
$$

For $h=\Delta^{1/(2+2\beta)}$, both $\Delta/h^2$ and $h^{2\beta}$ equal $\Delta^{2\beta/(2\beta+2)}$. Therefore **$D_1=10$ and $D_2=2C^2$ satisfy both requested bounds**:

$$
\boxed{\mathbb E\bigl(\widehat\Lambda_n(g_n)-\sigma^2(t_0)\bigr)^2
\leq(10\|\sigma^4\|_\infty+2C^2)\Delta^{2\beta/(2\beta+2)}.}
$$

The constants are independent of the observation partition, $\sigma$, $t_0$ and $\beta$. The exponent follows from a [bias-variance tradeoff](../../../../../../bias-variance-tradeoff.md) for a shrinking window.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 209](../../../paper-209-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
