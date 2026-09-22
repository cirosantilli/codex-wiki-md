<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $u=0$ the assertion is immediate under the natural zero-vector convention. For $u\ne0$, the rows $a_r$ of $A$ are independent and $a_r^Tu/\lVert u\rVert_2$ is a centered unit-variance [sub-Gaussian random variable](../../../../../../sub-gaussian-distribution.md). Its centered square is [sub-exponential](../../../../../../subexponential-distribution-light-tailed.md). The corresponding Bernstein estimate, in the explicit [Rademacher Johnson–Lindenstrauss transform](../../../../../../rademacher-johnson-lindenstrauss-transform.md) form, is

$$
\mathbb P\left(\left|\frac1d\sum_{r=1}^d
\frac{(a_r^Tu)^2}{\lVert u\rVert_2^2}-1\right|\geq t\right)
\leq2e^{-dt^2/136},
\qquad0<t<1.
$$

Since the sum in the event is $\lVert Au\rVert_2^2/\lVert u\rVert_2^2$, this is the claimed inequality.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 205](../../../paper-205-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
