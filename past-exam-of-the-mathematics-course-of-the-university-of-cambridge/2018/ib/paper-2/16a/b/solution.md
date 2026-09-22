<h1 id="16a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The homogeneous solutions $(C_1+C_2x)e^{-x}$ are not $2\pi$-periodic unless $C_1=C_2=0$, so there is a unique periodic solution. For a forcing term $a_n\cos(nx)$, a trial solution $A_n\cos(nx)+B_n\sin(nx)$ gives

$$
A_n=\frac{a_n(1-n^2)}{(1+n^2)^2},
\qquad
B_n=\frac{2na_n}{(1+n^2)^2}.
$$

Using the [Fourier series](../../../../../../fourier-series-split.md) from part (a), for which only odd $n$ occur and $a_n=-4/(\pi n^2)$, yields

$$
\boxed{
y(x)=\frac\pi2-\frac4\pi
\sum_{\substack{n\geq1\\n\text{ odd}}}
\frac{(1-n^2)\cos(nx)+2n\sin(nx)}{n^2(1+n^2)^2}.}
$$

The coefficients decay fast enough to differentiate the series twice term by term, verifying the equation and periodicity.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [16A](../../16a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
